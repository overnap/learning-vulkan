cmake_minimum_required(VERSION 3.21)
project(learning_vulkan)

set(CMAKE_CXX_STANDARD 20)

include_directories("C:/VulkanSDK/1.2.198.1/Include")
include_directories("C:/lib/glm")
include_directories("C:/lib/glfw/include")

link_directories("C:/VulkanSDK/1.2.198.1/Lib")
link_directories("C:/lib/glfw/lib-mingw-w64")

add_executable(learning_vulkan main.cpp)
target_link_libraries(learning_vulkan glfw3 vulkan-1)