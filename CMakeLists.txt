project(swagger-ui)
cmake_minimum_required(VERSION 2.8.12)

install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/api
	DESTINATION share/griffin/www/docs
)

include(CPackConfig.cmake)
