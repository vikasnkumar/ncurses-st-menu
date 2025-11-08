include_directories(${CMAKE_CURRENT_SOURCE_DIR})
include_directories(${CMAKE_CURRENT_BINARY_DIR})

add_executable(demo demo.c)
target_link_libraries(demo st_menu ${NCURSESW_LIBRARIES} ${UNISTRING_LIBRARIES})

add_executable(simple simple.c)
target_link_libraries(simple st_menu ${NCURSESW_LIBRARIES} ${UNISTRING_LIBRARIES})

add_executable(simple2 simple2.c)
target_link_libraries(simple2 st_menu ${NCURSESW_LIBRARIES} ${UNISTRING_LIBRARIES})

