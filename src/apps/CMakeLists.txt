# Dependency libraries
#find_package(LIBRARY_NAME REQUIRED)

# tests
add_executable(app_scout_demo scout_demo/scout_demo.cpp)
target_link_libraries(app_scout_demo scoutbase)

add_executable(app_scout_discharge scout_demo/scout_discharge.cpp)
target_link_libraries(app_scout_discharge scoutbase)

if(BUILD_MONITOR)
    add_subdirectory(scout_monitor)
endif()