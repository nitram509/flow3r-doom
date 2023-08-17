idf_component_register(
    SRCS
        GAMMATBL.c 
        SINETABL.c 
        TANGTABL.c 
        TANTOANG.c
    INCLUDE_DIRS
        .
        ./include
)

target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-error)