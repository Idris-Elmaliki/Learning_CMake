cmake_minimum_required(VERSION 3.13)

add_subdirectory("thirdParty_Libraries/profilerLib")


project(main1)
set(CMAKE_CXX_STANDARD 17) # this sets our C++ version to C++ 17
add_executable(main1 "src/main.cpp") # The commands below are for linking include directories and libraries 
target_include_directories(main1 PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include/") 
target_link_libraries(main1 PRIVATE profilerLib) # Note: For libraries, this isn't enough, we must also have another CMakeLists for the libraries themselves 
