add_executable(TwAdvanced1 TwAdvanced1.cpp)
target_link_libraries(TwAdvanced1 AntTweakBar GLU glfw)

add_executable(TwSimpleGLFW TwSimpleGLFW.cpp)
target_link_libraries(TwSimpleGLFW AntTweakBar GLU glfw)

add_executable(TwSimpleGLUT TwSimpleGLUT.cpp)
target_link_libraries(TwSimpleGLUT AntTweakBar GLU glut)

add_executable(TwSimpleSDL TwSimpleSDL.cpp)
target_link_libraries(TwSimpleSDL AntTweakBar GLU SDL)

add_executable(TwString TwString.cpp)
target_link_libraries(TwString AntTweakBar glfw)

