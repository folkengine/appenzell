cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

# create project
project(CPMPlaybook)

# ---- Executable ----
add_executable(CPMPlaybook main.cpp)

# ---- Dependencies ----
include(cmake/CPM.cmake)
CPMAddPackage("gh:nlohmann/json@3.11.3")

# ---- Link Dependencies ----
target_compile_features(CPMPlaybook PRIVATE cxx_std_17)
target_link_libraries(CPMPlaybook nlohmann_json::nlohmann_json)
