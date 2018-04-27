cmake_minimum_required(VERSION 3.10)
project(RavenMongocxxExperiments)

set(CMAKE_CXX_STANDARD 11)

find_package(LIBMONGOCXX REQUIRED)
find_package(LIBBSONCXX REQUIRED)

include_directories(${LIBMONGOCXX_INCLUDE_DIR})
include_directories(${LIBBSONCXX_INCLUDE_DIR})

add_executable(${PROJECT_NAME}
        main.cpp
        src/RavenMongo.cpp src/RavenMongo.h
        )

#target_link_libraries(${PROJECT_NAME} ${LIBMONGOCXX_LIBRARIES})
#target_link_libraries(${PROJECT_NAME} ${LIBBSONCXX_LIBRARIES})