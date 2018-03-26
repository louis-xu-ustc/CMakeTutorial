add_library(part4library SHARED Library.cc)
set_target_properties(part4library PROPERTIES LIBRARY_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/lib)
set_target_properties(part4library PROPERTIES OUTPUT_NAME part4library${BUILD_POSTFIX})

#include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
