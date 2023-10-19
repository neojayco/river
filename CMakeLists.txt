## Dependends on CMake v3.25
cmake_minimum_required(VERSION 3.25)
## Generate it's under the project name 'river', written in CXX
project(river CXX)

## Include directory
include_directories(include)

## Crossplatform source files
list(APPEND
    river_SOURCES
    ""
)

## Get OS dependent source files
if (WIN32)
    list(APPEND
        river_SOURCES
        ""
    )
endif ()

add_library(${CMAKE_PROJECT_NAME} ${river_SOURCES})
