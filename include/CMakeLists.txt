configure_file(st_config.h.in st_config.h @ONLY)
set_directory_properties(PROPERTIES ADDITIONAL_MAKE_CLEAN_FILES st_config.h)
install(FILES ${CMAKE_CURRENT_BINARY_DIR}/st_config.h DESTINATION include)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/ DESTINATION include
    FILES_MATCHING PATTERN "*.h" PATTERN ".h.in" EXCLUDE)
