include_directories(${LLVM_INCLUDE_DIR})

set ( CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -D__STDC_LIMIT_MACROS=1 -D__STDC_CONSTANT_MACROS=1" )

add_library (SPATarget YicesBackend/YicesBackend.cpp
YicesBackend/XorElimination.cpp SMT12Backend.cpp AnteaterInstNamer.cpp)

