add_library(${PROJECT_NAME})
add_library(${PROJECT_NAME}::${PROJECT_NAME} ALIAS ${PROJECT_NAME})
target_sources(${PROJECT_NAME}
  PUBLIC
  FILE_SET HEADERS
  TYPE HEADERS
  FILES
    all-io.h
    # TODO add all others headers here
)
# If .c implementation sources were added to the target, this is not needed.
set_target_properties(${PROJECT_NAME} PROPERTIES LINKER_LANGUAGE C)
