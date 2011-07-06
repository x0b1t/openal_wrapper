cmake_minimum_required(VERSION 2.8)

project( openal_wrapper )

add_definitions(
   -Wall 
   -Wextra
   -pedantic 
   #-Werror 
   #-std=c99
   #-DNDEBUG
)

if( !WIN32 )

include_directories(
    /usr/include/
)

endif()

add_executable( openal_wrapper
   src/main.cpp
)
