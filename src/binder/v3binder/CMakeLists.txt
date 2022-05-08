add_library_clr(v3binder
    STATIC
    ${BINDER_SOURCES}
)

if(FEATURE_PERFTRACING)
add_dependencies(v3binder eventing_headers)
endif()
