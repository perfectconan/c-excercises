add_library(displaylib
	window.cc window.h
	functions.cc functions.h
	sdlobject.cc sdlobject.h
	surface.cc surface.h
	surface3d.cc surface3d.h
	triangle.cc triangle.h
	rgb.h
	matrix.h
	cube.h
	vector2d.h
	vector3d.h
	pyramid.h
)
set_property(TARGET displaylib PROPERTY CXX_STANDARD 14)
target_link_libraries(displaylib SDL2)
target_include_directories(displaylib INTERFACE ..)
