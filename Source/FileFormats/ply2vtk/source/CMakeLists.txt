
PROJECT(ply2vtk)
cmake_minimum_required(VERSION 2.6)
ADD_EXECUTABLE(ply2vtk ply2vtk.cxx ${source_files})
TARGET_LINK_LIBRARIES(ply2vtk ${VTK_LIBRARIES} )
INSTALL(TARGETS ply2vtk  RUNTIME DESTINATION .)
