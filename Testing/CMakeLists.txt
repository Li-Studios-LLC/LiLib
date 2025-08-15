file(GLOB_RECURSE SRCS *.cpp)
file(GLOB_RECURSE HDRS *.h)

add_executable(Testing)

target_sources(Testing PUBLIC ${SRCS} ${HDRS})
target_link_libraries(Testing PUBLIC LiLib)
target_include_directories(Testing PUBLIC ${PROJECT_SOURCE_DIR}/Src)