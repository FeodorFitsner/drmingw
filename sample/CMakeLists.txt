force_debug ()

add_executable (sample
    sample.cpp
)
add_dependencies (sample exchndl_implib)
target_link_libraries (sample ${EXCHNDL_IMPLIB})

install (FILES sample.cpp DESTINATION sample)
install (FILES sample.mak DESTINATION sample RENAME Makefile)
