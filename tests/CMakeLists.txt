add_executable(LogTest LogTest.cpp)
if(WIN32)
	target_link_libraries(LogTest limlog)
else()
	target_link_libraries(LogTest limlog pthread)
endif()