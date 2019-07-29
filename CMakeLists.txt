cmake_minimum_required(VERSION 3.1.0)

project(simpleOpenCVMatToWayland)

list(APPEND CMAKE_PREFIX_PATH "D:\\opencv\\buildWhatEver\\install")

find_package(OpenCV REQUIRED)

add_executable(simpleOpenCVMatToWayland
	wayland-shm.cpp
	main.cpp
)

target_link_libraries(simpleOpenCVMatToWayland ${OpenCV_LIBS})