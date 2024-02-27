add_library(uuid)
add_library(${PROJECT_NAME}::uuid ALIAS uuid)

add_subdirectory(src)

