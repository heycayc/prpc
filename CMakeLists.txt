
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
PROJECT(prpc)

SET(CMAKE_DEBUG_POSTFIX "d")

ADD_DEFINITIONS(-D_CRT_SECURE_NO_WARNINGS)

FIND_PACKAGE(Boost REQUIRED)
INCLUDE_DIRECTORIES(${Boost_INCLUDE_DIRS})
LINK_DIRECTORIES(${Boost_LIBRARY_DIRS})

# scanner.
ADD_SUBDIRECTORY(common)
ADD_SUBDIRECTORY(scanner)

