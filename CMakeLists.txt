cmake_minimum_required(VERSION 3.30)
project(SubjectIcons)

set(CMAKE_CXX_STANDARD 26)

set(ICON_FILES
        ${CMAKE_SOURCE_DIR}/icons.rc
)

set(RC_FILE
        ${CMAKE_SOURCE_DIR}/version.rc)

add_library(SubjectIcons SHARED library.cpp ${RC_FILE} ${ICON_FILES})
