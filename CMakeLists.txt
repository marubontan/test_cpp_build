# CMakeのバージョンを設定
cmake_minimum_required(VERSION 2.8)
# プロジェクト名と使用する言語を設定
project(test_cmake CXX)
add_library(hello hello.cpp)
# a.outという実行ファイルをmain.cppとhello.cppから作成
add_executable(a.out main.cpp hello.cpp)
target_link_libraries(a.out hello)

