## quux plug-in

## create and install a shared library that can plug into shadow
add_shadow_plugin(shadow-plugin-quux quux.c)
target_link_libraries(shadow-plugin-quux)
install(TARGETS shadow-plugin-quux DESTINATION plugins)

## create and install an executable that can run outside of shadow
add_executable(quux quux.c)
target_link_libraries(quux)
install(TARGETS quux DESTINATION bin)
