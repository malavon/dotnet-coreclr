add_library_clr(unwinder_wks ${UNWINDER_SOURCES})
if(FEATURE_PERFTRACING)
add_dependencies(unwinder_wks eventing_headers)
endif()
