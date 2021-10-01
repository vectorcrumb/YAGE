cmake_minimum_required(VERSION 3.4)
project(YAGE)

set(CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/modules/" ${CMAKE_MODULE_PATH})

# Add Corrade as a subproject
add_subdirectory(external/corrade EXCLUDE_FROM_ALL)

# Add Magnum as a subproject, enable GLFWApplication
set(CMAKE_PREFIX_PATH ${PROJECT_SOURCE_DIR}/external/glfw-3.3.4.bin.WIN64 ${CMAKE_PREFIX_PATH})
set(WITH_GLFWAPPLICATION ON)
add_subdirectory(external/magnum EXCLUDE_FROM_ALL)

add_subdirectory(src)
