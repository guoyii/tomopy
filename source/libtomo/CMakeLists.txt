add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/misc)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/prep)
add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/recon)
if(TOMOPY_USE_MKL)
    add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/gridrec)
endif()
if(TOMOPY_USE_OPENCV OR TOMOPY_USE_CUDA)
    add_subdirectory(${CMAKE_CURRENT_LIST_DIR}/accel)
endif()
