# Copyright 2023 Michael Fabian 'Xaymar' Dirks <info@xaymar.com>

################################################################################
# Bootstrap
################################################################################
cmake_minimum_required(VERSION 3.26)
project(TonStream)
list(APPEND CMAKE_MESSAGE_INDENT "[${PROJECT_NAME}] ")
define_plugin(
	NAME ${PROJECT_NAME}
)

# Search Paths
list(APPEND CMAKE_MODULE_PATH
	"${CMAKE_CURRENT_SOURCE_DIR}/cmake/modules"
	"${CMAKE_CURRENT_SOURCE_DIR}/cmake"
)

################################################################################
# Dependencies
################################################################################

# set(Boost_USE_STATIC_LIBS ON)
# set(Boost_USE_STATIC_RUNTIME ON)
# find_package(Boost REQUIRED)
# target_link_libraries(${PROJECT_NAME} PRIVATE
# 	Boost::boost
# )

################################################################################
# Finish
################################################################################
setup_target(${PROJECT_NAME})
