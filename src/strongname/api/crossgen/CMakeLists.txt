include(${CLR_DIR}/crossgen.cmake)

add_library_clr(strongname_crossgen ${STRONGNAME_SOURCES})
if(FEATURE_PERFTRACING)
add_dependencies(strongname_crossgen eventing_headers)
endif()
