cmake_minimum_required(VERSION 3.5)
project(test-repo)

add_library(test-repo SHARED src/test_repo.c)

install(TARGETS test-repo DESTINATION lib)
install(FILES src/test_repo.h DESTINATION include)
