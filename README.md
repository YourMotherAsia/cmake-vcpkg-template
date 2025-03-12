
# CMake + Vcpkg Template

This is a template for setting up CMake with Vcpkg, making it easier to manage C++ dependencies with Vcpkg.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)

## Installation
1. Clone the repository:
  ```bash
  git clone https://github.com/YourMotherAsia/cmake-vcpkg-template.git
  cd cmake-vcpkg-template
  ```
2. Initialize the submodules:
  ```bash
  git submoudle update --init
  ```
3. Bootstrap Vcpkg
  ```bash
  ./submodules/vcpkg/bootstrap-vcpkg.sh
  ```

4. Setup and build the project:
  ```bash
  cmake -B build/ -S . --preset default
  cmake --build build
  ```

## Usage
After building, you can link dependencies using CMake in your own projects. Example:
```cmake
find_package(Vcpkg REQUIRED)
```

## Contributing
Feel free to fork the repository, make improvements, and open pull requests.
