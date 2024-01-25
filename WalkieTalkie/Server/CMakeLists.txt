cmake_minimum_required(VERSION 3.12)

project(ServerApp)

set(CMAKE_CXX_STANDARD 11)

add_executable(ServerApp ServerMain.cpp)

link_directories(/home/kpit/Downloads/Walkie-Talkie/Server/api)
 
target_link_libraries(ServerApp PRIVATE
    /home/kpit/Downloads/Walkie-Talkie/Server/lib/libServerSocket.so
    pthread
)