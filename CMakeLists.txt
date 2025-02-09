cmake_minimum_required(VERSION 3.5)
project(test-repo)

add_library(test-repo SHARED src/test_repo.c)
set_target_properties(test-repo PROPERTIES VERSION 1.0 SOVERSION 1)
install(TARGETS test-repo DESTINATION lib)
install(FILES src/test_repo.h DESTINATION include)
