cmake_minimum_required(VERSION 3.5)

project(linkSlicerBlender)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/dentsoft-foundation/linkSlicerBlender")
set(EXTENSION_CATEGORY "Dentistry")
set(EXTENSION_CONTRIBUTORS "Patrick Moore, Georgi Talmazov (Dental Software Foundation)")
set(EXTENSION_DESCRIPTION "linkSlicerBlender")
set(EXTENSION_ICONURL "")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/StereoSlicer/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(slicer_module)

## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
