include_directories(${CMAKE_CURRENT_SOURCE_DIR})
include_directories(${CMAKE_CURRENT_BINARY_DIR})

add_library(st_menu st_menu.c st_menu_styles.c unicode.c)
target_link_libraries(st_menu ${NCURSESW_LIBRARIES} ${UNISTRING_LIBRARIES})

install(TARGETS st_menu RUNTIME DESTINATION bin
    ARCHIVE DESTINATION lib LIBRARY DESTINATION lib)

