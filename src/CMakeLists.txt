add_executable(${PROJECT_NAME} 
	zlibpes.cpp
)

target_link_libraries(${PROJECT_NAME} ZLIB::ZLIB)

install(TARGETS ${PROJECT_NAME} DESTINATION ${CMAKE_INSTALL_PREFIX}/bin)
install(FILES ${_VCPKG_INSTALLED_DIR}/${VCPKG_TARGET_TRIPLET}/bin/zlib1.dll DESTINATION ${CMAKE_INSTALL_PREFIX}/bin)