project(Super4PCS)

set(Demo_Super4PCS_SRC
    ${CMAKE_CURRENT_SOURCE_DIR}/super4pcs_test.cc
)

add_executable(${PROJECT_NAME} ${Demo_Super4PCS_SRC})
target_link_libraries(${PROJECT_NAME} opengr_algo opengr_utils)
install( TARGETS ${PROJECT_NAME} RUNTIME DESTINATION bin  )
