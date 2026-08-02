file(GLOB SRC *.c *.asm *.s *.S)
file(GLOB HEADERS *.h)

target_sources(freestdc PRIVATE ${SRC} ${HEADERS})
add_subdirectory("fstdc-utils")

install(FILES ${HEADERS} DESTINATION include/)
