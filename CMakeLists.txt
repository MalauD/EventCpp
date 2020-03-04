# CMakeList.txt : CMake project for EventCpp, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project (EventCpp VERSION 1.0.0)

# Add source to this project's executable.
add_library(EventCpp STATIC
    Source/Event/Event.hpp
    Source/Event/EventArgs.hpp
)

set_target_properties(EventCpp PROPERTIES LINKER_LANGUAGE CXX)

set_target_properties(EventCpp PROPERTIES VERSION ${PROJECT_VERSION})

# TODO: Add tests and install targets if needed.
