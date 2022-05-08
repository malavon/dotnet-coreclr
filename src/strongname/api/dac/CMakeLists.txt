
include(${CLR_DIR}/dac.cmake)

add_library_clr(strongname_dac ${STRONGNAME_SOURCES})
if(FEATURE_PERFTRACING)
add_dependencies(strongname_dac eventing_headers)
endif()
