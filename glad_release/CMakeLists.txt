add_library(glad src/glad.c)

set_property(TARGET glad PROPERTY C_STANDARD 99)

target_include_directories(glad PUBLIC include)

target_link_libraries(glad)
