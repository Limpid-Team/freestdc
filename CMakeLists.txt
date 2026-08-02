project(freestdc VERSION 0.0.1)

# Setup basic build settings
enable_language(ASM)

# Library
add_library(freestdc STATIC)

target_include_directories(freestdc SYSTEM BEFORE PUBLIC ${PROJECT_SOURCE_DIR}/include)

add_subdirectory(include)
add_subdirectory(src)
