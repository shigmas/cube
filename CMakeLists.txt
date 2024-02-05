cmake_minimum_required(VERSION 3.20)

project(cube LANGUAGES CXX)

find_package(Qt6 REQUIRED COMPONENTS Core Gui Widgets OpenGLWidgets)

qt_standard_project_setup()

qt_add_executable(cubeApp
  mainwidget.cpp mainwidget.h
  geometryengine.cpp geometryengine.h
  main.cpp
  shaders.qrc
  textures.qrc
)

qt_add_resources(cubeApp "cubeApp"
  PREFIX "/"
  FILES "vshader.glsl" "fshader.glsl" "cube.png"
)
  

target_link_libraries(cubeApp PRIVATE Qt6::Core Qt6::Gui Qt6::Widgets Qt6::OpenGLWidgets)
