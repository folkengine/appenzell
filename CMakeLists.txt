cmake_minimum_required(VERSION 3.29 FATAL_ERROR)

# create project
project(Appenzell)

set(CMAKE_CXX_STANDARD 17)  # Replace 14 with your desired C++ version
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# ---- Executable ----
add_executable(Appenzell main.cpp)

# ---- Dependencies ----
include(cmake/CPM.cmake)
CPMAddPackage("gh:nlohmann/json@3.11.3")
CPMAddPackage("gh:PortAudio/portaudio@19.7.0")
CPMAddPackage("gh:libsndfile/libsndfile#72f6af15e8f85157bd622ed45b979025828b7001")



# CPMAddPackage("gh:EVerest/everest-cmake@0.1.0")
# CPMAddPackage("gh:US-JOET/libocpp#folkengine/add_1.6_validate_and_add_profile_tests")

# ---- Link Dependencies ----
target_compile_features(CPMPlaybook PRIVATE cxx_std_17)
target_link_libraries(CPMPlaybook nlohmann_json::nlohmann_json)
