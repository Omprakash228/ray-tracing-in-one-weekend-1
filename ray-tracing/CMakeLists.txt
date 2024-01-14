# CMakeList.txt : CMake project for ray-tracing, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (ray-tracing "main.cpp"  "vec3/vec3.h" "color/color.h" "ray/ray.h" "hittable/hittable.h" "sphere/sphere.h" "hittable/hittable_list.h" "constants/constants.h" "interval/interval.h" "camera/camera.h" "material/material.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET ray-tracing PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
