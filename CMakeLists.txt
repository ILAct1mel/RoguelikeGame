cmake_minimum_required(VERSION 3.22)
project(GenNEtZzUPDFINAL)

set(CMAKE_CXX_STANDARD 14)

set(SDL2_INCLUDE_DIR C:/SDL2/SDL2-2.0.22/include)
set(SDL2_LIB_DIR C:/SDL2/SDL2-2.0.22/lib/x64)


include_directories(${SDL2_INCLUDE_DIR})
link_directories(${SDL2_LIB_DIR})

add_executable(GenNEtZzUPDFINAL main.cpp Camera.cpp Camera.h FLOOR.cpp FLOOR.h Map.cpp Map.h Sprite.cpp Sprite.h Player.h Eternity.h Player.cpp Eternity.cpp Warrior.cpp Warrior.h fly.cpp fly.h TypeEnemy.cpp TypeEnemy.h Rat.cpp Rat.h FatEnemy.cpp FatEnemy.h)

target_link_libraries(${PROJECT_NAME} SDL2main SDL2 SDL2_image SDL2_mixer SDL2_ttf)