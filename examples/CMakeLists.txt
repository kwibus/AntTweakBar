
set(LIBS AntTweakBar)
if (${CMAKE_SYSTEM_NAME} MATCHES "Linux") 
    LIST (APPEND LIBS X11) 
endif()

add_executable(TwAdvanced1 TwAdvanced1.cpp)
target_link_libraries(TwAdvanced1 ${LIBS} GLU glfw)

add_executable(TwSimpleGLFW TwSimpleGLFW.cpp)
target_link_libraries(TwSimpleGLFW ${LIBS} GLU glfw)

add_executable(TwSimpleGLUT TwSimpleGLUT.cpp)
target_link_libraries(TwSimpleGLUT ${LIBS} GLU glut)

add_executable(TwSimpleSDL TwSimpleSDL.cpp)
target_link_libraries(TwSimpleSDL ${LIBS} GLU SDL)

add_executable(TwString TwString.cpp)
target_link_libraries(TwString ${LIBS} glfw)

