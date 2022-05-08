add_library_clr(strongname_wks ${STRONGNAME_SOURCES})
if(FEATURE_PERFTRACING)
add_dependencies(strongname_wks eventing_headers)
endif()
