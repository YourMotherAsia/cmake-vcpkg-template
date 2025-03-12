#CMakeLists.txt (root)

cmake_minimum_required(VERSION 3.21)
project(MyProject)

find_package(fmt REQUIRED)

# Set the C++ standard
set(CMAKE_CXX_STANDARD 17)

# Define the sources for the main executable
set(
  CPP_TEMPLATE_SOURCES
  src/main.cpp
)

# Add the main executable
add_executable(main ${CPP_TEMPLATE_SOURCES})

# Link the necessary libraries
target_link_libraries(main PRIVATE ${LIBRARIES} fmt::fmt)

