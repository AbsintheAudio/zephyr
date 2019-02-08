cmake_minimum_required(VERSION 3.13.1)
macro(set_conf_file)
<<<<<<< HEAD
  if(EXISTS               ${APPLICATION_SOURCE_DIR}/boards/${BOARD}.conf)
=======
  if(EXISTS ${APPLICATION_SOURCE_DIR}/boards/${BOARD}.conf)
>>>>>>> master
    set(CONF_FILE "prj.conf ${APPLICATION_SOURCE_DIR}/boards/${BOARD}.conf")
  else()
    set(CONF_FILE "prj.conf")
  endif()
endmacro()

include($ENV{ZEPHYR_BASE}/cmake/app/boilerplate.cmake NO_POLICY_SCOPE)
<<<<<<< HEAD
project(led_ws2812)
=======
project(led_apa102)
>>>>>>> master

FILE(GLOB app_sources src/*.c)
target_sources(app PRIVATE ${app_sources})
