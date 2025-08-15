file(GLOB_RECURSE SRCS *.cpp)
file(GLOB_RECURSE HDRS *.h)

add_library(LiLib STATIC)

target_sources(LiLib PUBLIC ${SRCS} ${HDRS})
target_precompile_headers(LiLib PUBLIC pch.h)