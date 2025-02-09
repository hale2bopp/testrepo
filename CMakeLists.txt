cmake_minimum_required(VERSION 3.5)
project(testrepo)

add_library(testrepo SHARED src/test_repo.c)
set_target_properties(testrepo PROPERTIES VERSION 1.0 SOVERSION 1)
install(TARGETS testrepo DESTINATION lib)
install(FILES src/test_repo.h DESTINATION include)
