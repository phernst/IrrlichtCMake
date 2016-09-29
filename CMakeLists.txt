cmake_minimum_required (VERSION 2.8.11)
project (Irrlicht)

set (VERSION_MAJOR 1)
set (VERSION_MINOR 8)
set (VERSION_RELEASE 4)

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE "Debug" CACHE STRING
      "Choose the type of build, options are: Debug Release
RelWithDebInfo MinSizeRel."
      FORCE)
endif(NOT CMAKE_BUILD_TYPE)

if (NOT BUILD_SHARED_LIBS)
	set (BUILD_SHARED_LIBS 0 CACHE BOOL "Build a shared library?")
endif (NOT BUILD_SHARED_LIBS)

include_directories (
  include
  source/Irrlicht/zlib
  source/Irrlicht/jpeglib
  source/Irrlicht/libpng
)

add_definitions (-DIRRLICHT_EXPORTS=1)

set (CMAKE_CXX_FLAGS "-Wall -pipe -fno-exceptions -fno-rtti -fstrict-aliasing" CACHE STRING "Flags used by the compiler during all build types." FORCE)

set (CMAKE_CXX_FLAGS_DEBUG "-g -D_DEBUG" CACHE STRING "Flags used by the compiler during debug builds." FORCE)
set (CMAKE_CXX_FLAGS_RELEASE "-fexpensive-optimizations -O3" CACHE STRING "Flags used by the compiler during release builds." FORCE)

set (CMAKE_C_FLAGS "-O3 -fexpensive-optimizations -DPNG_THREAD_UNSAFE_OK -DPNG_NO_MMX_CODE -DPNG_NO_MNG_FEATURES" CACHE STRING "Flags used by the compiler during all build types." FORCE)

if (BUILD_SHARED_LIBS)
  set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC" CACHE STRING "Flags used by the compiler during all build types." FORCE)
  set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fPIC" CACHE STRING "Flags used by the compiler during all build types." FORCE)
endif (BUILD_SHARED_LIBS)

# Linux specific options
if (${CMAKE_SYSTEM_NAME} MATCHES "Linux")
  include_directories (/usr/X11R6/include)

# OSX specific options
elseif (${CMAKE_SYSTEM_NAME} MATCHES "Darwin")
  include_directories (MacOSX /usr/X11R6/include)

# Windows specific options
elseif (WIN32)
  add_definitions (
    -DNO_IRR_COMPILE_WITH_DIRECTINPUT_JOYSTICK_
    -DNO_IRR_COMPILE_WITH_DIRECT3D_9_
    -DIRR_COMPILE_WITH_DX9_DEV_PACK
    -D__GNUWIN32__
    -D_WIN32
    -DWIN32
    -D_WINDOWS
    -D_MBCS
    -D_USRDLL
  )
  if (NOT BUILD_SHARED_LIBS)
    add_definitions (-D_IRR_STATIC_LIB_)
  endif (NOT BUILD_SHARED_LIBS)
  
endif (${CMAKE_SYSTEM_NAME} MATCHES "Linux")

add_subdirectory (source)
