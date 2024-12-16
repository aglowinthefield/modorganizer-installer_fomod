cmake_minimum_required(VERSION 3.16)

set(CMAKE_INSTALL_PREFIX ${MO2_INSTALLDIR})
project(installer_fomod)


if(DEFINED DEPENDENCIES_DIR)
	include(${DEPENDENCIES_DIR}/modorganizer_super/cmake_common/mo2.cmake)
else()
	include(${CMAKE_CURRENT_LIST_DIR}/../cmake_common/mo2.cmake)
endif()

add_subdirectory(src)
