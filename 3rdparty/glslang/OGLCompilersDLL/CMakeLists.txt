set(SOURCES InitializeDll.cpp InitializeDll.h)

add_library(OGLCompiler STATIC ${SOURCES})
set_property(TARGET OGLCompiler PROPERTY FOLDER glslang)
set_property(TARGET OGLCompiler PROPERTY POSITION_INDEPENDENT_CODE ON)

if(WIN32)
    source_group("Source" FILES ${SOURCES})
endif(WIN32)
