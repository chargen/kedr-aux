set(executable_name "test_indent_param")
add_executable(${executable_name} test.cpp)

target_link_libraries(${executable_name} ${mist_name})

test_add_target(${executable_name})

add_test("core.indent_param" ${executable_name})