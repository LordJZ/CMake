
set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_BUILD_INTERFACE_INCLUDES ON)

add_library(libA SHARED libA.cpp)
target_link_libraries(libA LINK_PUBLIC Qt4::QtCore)
generate_export_header(libA)
