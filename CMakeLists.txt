project(Tess2)
cmake_minimum_required(VERSION 2.8)

include_directories (include)
add_subdirectory (src)

install (DIRECTORY include/ DESTINATION include FILES_MATCHING PATTERN "*.h")