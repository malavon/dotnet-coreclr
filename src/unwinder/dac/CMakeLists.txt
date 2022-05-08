include(${CLR_DIR}/dac.cmake)

add_definitions(-DFEATURE_NO_HOST)

add_library_clr(unwinder_dac ${UNWINDER_SOURCES})
if(FEATURE_PERFTRACING)
add_dependencies(unwinder_dac eventing_headers)
endif()
