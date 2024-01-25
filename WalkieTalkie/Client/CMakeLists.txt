cmake_minimum_required(VERSION 3.12)

project(ClientApp)

set(CMAKE_CXX_STANDARD 11)

add_executable(ClientApp ClientMain.cpp)

link_directories(/home/kpit/Downloads/Walkie-Talkie/Client/api)
 
target_link_libraries(ClientApp PRIVATE
    /home/kpit/Downloads/Walkie-Talkie/Client/lib/libClientSocket.so
    pthread
)