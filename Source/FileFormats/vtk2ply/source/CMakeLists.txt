 
PROJECT(vtk2ply)
cmake_minimum_required(VERSION 2.6)
ADD_EXECUTABLE(vtk2ply vtk2ply.cxx ${source_files})
TARGET_LINK_LIBRARIES(vtk2ply ${VTK_LIBRARIES} )
INSTALL(TARGETS vtk2ply  RUNTIME DESTINATION .)
