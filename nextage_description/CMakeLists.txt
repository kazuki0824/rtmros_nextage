cmake_minimum_required(VERSION 3.5)
project(nextage_description)


find_package(ament_cmake REQUIRED)
install(DIRECTORY models urdf www DESTINATION share/${PROJECT_NAME})

ament_package()

