# CMakeList.txt : CMake project for midiToolbox, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("seq2mid")

# Add source to this project's executable.
add_executable (seq2mid "decode.h" "dir_emu.h" "seq2mid.c" "decode0.c")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET seq2mid PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
