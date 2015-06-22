set(LLVM_LINK_COMPONENTS
  ${LLVM_TARGETS_TO_BUILD}
  DebugInfo
  MC
  MCDisassembler
  Object
  Support
  )

add_llvm_tool(llvm-rop
  llvm-rop.cpp
  COFFDump.cpp
  ELFDump.cpp
  MachODump.cpp
  )
