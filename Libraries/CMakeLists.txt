if(WIN32)
    set(GLDEMO_EXE WIN32)
    set(GLDEMO_LIBS mingw32 libgldemo_static opengl32 glu32)
else()
    set(GLDEMO_EXE "")
    set(GLDEMO_LIBS libgldemo_static Xxf86vm rt Xext X11 GL GLU)
endif()

add_subdirectory(FileHandler)
add_subdirectory(libgldemo)
add_subdirectory(libvitaboy)
