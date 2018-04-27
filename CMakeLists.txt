cmake_minimum_required(VERSION 3.10)
project(RavenMongocxxExperiments)

set(CMAKE_CXX_STANDARD 11)
find_package(LIBMONGOCXX REQUIRED)
find_package(LIBBSONCXX REQUIRED)

add_executable(RavenMongocxxExperiments
        main.cpp
        src/RavenMongo.cpp src/RavenMongo.h
        )