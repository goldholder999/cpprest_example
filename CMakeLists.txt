cmake_minimum_required (VERSION 3.8)

project ("hello-cpprest")
if(DEFINED ENV{VCPKG_ROOT} AND NOT DEFINED CMAKE_TOOLCHAIN_FILE)
  set(CMAKE_TOOLCHAIN_FILE "$ENV{VCPKG_ROOT}/scripts/buildsystems/vcpkg.cmake"
      CACHE STRING "")
endif()
find_package(cpprestsdk CONFIG REQUIRED)
add_subdirectory ("hello-cpprest")
add_subdirectory ("test2")
