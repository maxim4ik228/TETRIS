cmake_minimum_required(VERSION 3.25)
project(untitled2)

set(CMAKE_CXX_STANDARD 17)

add_executable(untitled2 main.cpp GetWallKickData.hpp GetWallKickData.cpp Tetromino.cpp GetTetromino.cpp DrawText.cpp)


set(SFML_STATIC_LIBRARIES TRUE)
set(SFML_DIR C:/SFML/lib/cmake/SFML)
find_package(SFML COMPONENTS system window graphics audio network  REQUIRED)

include_directories(C:/SFML/include)
target_link_libraries(untitled2 sfml-system sfml-window sfml-graphics sfml-audio)
