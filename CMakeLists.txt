
cmake_minimum_required(VERSION 2.8)

PROJECT(CreateGraph)

find_package(VTK REQUIRED)
include(${VTK_USE_FILE})

add_executable(CreateGraph MACOSX_BUNDLE CreateGraph)

if(VTK_LIBRARIES)
  target_link_libraries(CreateGraph ${VTK_LIBRARIES})
else()
  target_link_libraries(CreateGraph vtkHybrid vtkWidgets)
endif()
