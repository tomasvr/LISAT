link_directories(${CMAKE_BINARY_DIR}/controllers/footbot_lisat)
set(lisat_loop_functions_SOURCES lisat_loop_functions.cpp)

add_library(lisat_loop_functions MODULE ${lisat_loop_functions_SOURCES})
target_link_libraries(lisat_loop_functions
  footbot_lisat
  argos3core_simulator
  argos3plugin_simulator_dynamics2d
  argos3plugin_simulator_entities
  argos3plugin_simulator_footbot
  argos3plugin_simulator_genericrobot
  argos3plugin_simulator_media)