
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

SET(CMAKE_C_FLAGS_RELEASE "-fPIC -Wall -Wno-strict-aliasing -O2")

SET(CMAKE_C_FLAGS_DEBUG "-g")

SET(CMAKE_BUILD_TYPE Release)

SET(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/CMakeModules/")

PROJECT(libcutil C)

enable_testing()

SET(serial "1.0.0")

SET(soserial "1")

ADD_SUBDIRECTORY(src)
ADD_SUBDIRECTORY(tests)


