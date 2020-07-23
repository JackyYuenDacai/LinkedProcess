cmake_minimum_required(VERSION 3.13)
#project name
project(LinkedProcess)

#head file path
INCLUDE_DIRECTORIES(
    src/include
)

#source directory 
aux_source_directory(src DIR_SRCS)

#set environment variable
set(SRC
    ${DIR_SRCS}
)
#set extern libraries
set(LIBRARIES

)
add_library(linked ${DIR_SRCS})
#add link library
target_link_libraries(linked ${LIBRARIES})