cmake_minimum_required(VERSION 3.20)
project(RenodeBuild NONE)

add_custom_target(renode
    COMMAND bash "${CMAKE_SOURCE_DIR}/build.sh"
    WORKING_DIRECTORY "${CMAKE_SOURCE_DIR}"
    USES_TERMINAL
    VERBATIM
)
