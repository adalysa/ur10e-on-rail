cmake_minimum_required(VERSION 3.5)
project(toolpth_refinmnt_config)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

find_package(ament_cmake REQUIRED)
find_package(ur_description REQUIRED)

install(DIRECTORY launch urdf DESTINATION share/${PROJECT_NAME}/)
