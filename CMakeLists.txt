cmake_minimum_required(VERSION 2.8)
PROJECT(astroberry-server-artwork NONE)

set (VERSION_MAJOR 2)
set (VERSION_MINOR 0)
set (VERSION_RELEASE 0)

set(ARTWORK_DIR "/usr/share")

message("=========================================== $ENV{DESTDIR}/${BUILD_ROOT} ==============================================")

if (${CMAKE_SYSTEM_NAME} MATCHES "Linux")
        install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/astroberry-server-artwork DESTINATION ${ARTWORK_DIR})
endif()
