configure_file(version.hpp.in ${MY_PROJECT_GENERATED_INCLUDEDIR}/my_project/version.hpp @ONLY)

add_library(MyProject INTERFACE)
add_library(MyProject::MyProject ALIAS MyProject)
target_include_directories(MyProject INTERFACE $<BUILD_INTERFACE:${MY_PROJECT_GENERATED_INCLUDEDIR}>)
