set(SOURCES
    ApiServer.h ApiServer.cpp
)

add_library(apicore ${SOURCES})
target_link_libraries(apicore PRIVATE ethcore devcore ethminer-buildinfo Boost::filesystem jsoncpp_lib_static)
target_include_directories(apicore PRIVATE ..)
