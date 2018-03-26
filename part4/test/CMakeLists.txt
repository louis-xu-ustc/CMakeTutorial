add_executable(part4test Test.cc)
target_link_libraries(part4test part4library)
set_target_properties(part4test PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
set_target_properties(part4test PROPERTIES OUTPUT_NAME part4test${BUILD_POSTFIX})
