project(ProbeNormals)
cmake_minimum_required(VERSION 2.8)
add_executable(ProbeNormals ProbeNormals.cxx)
TARGET_LINK_LIBRARIES(ProbeNormals ${ITK_LIBRARIES})
INSTALL(TARGETS ProbeNormals RUNTIME DESTINATION .)

add_executable(ComputeMeanNormals ComputeMeanNormals.cxx)
TARGET_LINK_LIBRARIES(ComputeMeanNormals ${ITK_LIBRARIES} tinyxml)
INSTALL(TARGETS ComputeMeanNormals RUNTIME DESTINATION .)

add_executable(GenerateNormalFeaFiles GenerateNormalFeaFiles.cxx)
TARGET_LINK_LIBRARIES(GenerateNormalFeaFiles ${ITK_LIBRARIES} tinyxml fim_v4 vgl vgl_algo)
INSTALL(TARGETS GenerateNormalFeaFiles RUNTIME DESTINATION .)
