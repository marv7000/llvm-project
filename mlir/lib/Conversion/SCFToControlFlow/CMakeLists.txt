add_mlir_conversion_library(MLIRSCFToControlFlow
  SCFToControlFlow.cpp

  ADDITIONAL_HEADER_DIRS
  ${MLIR_MAIN_INCLUDE_DIR}/mlir/Conversion/SCFToControlFlow

  DEPENDS
  MLIRConversionPassIncGen

  LINK_LIBS PUBLIC
  MLIRArithDialect
  MLIRControlFlowDialect
  MLIRLLVMDialect
  MLIRSCFDialect
  MLIRSCFTransforms
  MLIRTransforms
  )
