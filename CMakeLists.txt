cmake_minimum_required(VERSION 2.8.9)

project(RTThermometry)

#-----------------------------------------------------------------------------
set(EXTENSION_NAME RTThermometry)
set(EXTENSION_HOMEPAGE "http://www.slicer.org/slicerWiki/index.php/Documentation/4.3/Extensions/RTThermometry")
set(EXTENSION_CATEGORY "IGT")
set(EXTENSION_CONTRIBUTORS "Laurent Chauvin (BWH)")
set(EXTENSION_DESCRIPTION "This is an example of extension bundling a loadable module")
set(EXTENSION_ICONURL "http://viewvc.slicer.org/viewvc.cgi/Slicer4/trunk/Extensions/Testing/RTThermometry/RTThermometry.png?revision=21746&view=co")
set(EXTENSION_SCREENSHOTURLS "http://wiki.slicer.org/slicerWiki/images/4/42/Slicer-r19441-RTThermometry-screenshot.png")

#-----------------------------------------------------------------------------
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
add_subdirectory(RTThermometry)

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
