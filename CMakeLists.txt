project(freestdc VERSION 0.0.1)

# Setup basic build settings
enable_language(ASM)

include_directories(BEFORE SYSTEM ${PROJECT_SOURCE_DIR}/include)

# Library
add_library(freestdc STATIC)

add_subdirectory(include)
add_subdirectory(src)
