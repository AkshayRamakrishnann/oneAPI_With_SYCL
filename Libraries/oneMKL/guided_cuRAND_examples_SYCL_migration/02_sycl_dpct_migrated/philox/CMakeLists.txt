add_executable(philox_lognormal philox_lognormal.cpp)
add_executable(philox_normal philox_normal.cpp)
add_executable(philox_poisson philox_poisson.cpp)
add_executable(philox_uniform philox_uniform.cpp)

target_link_libraries(philox_lognormal OpenCL sycl)
target_link_libraries(philox_normal OpenCL sycl)
target_link_libraries(philox_poisson OpenCL sycl)
target_link_libraries(philox_uniform OpenCL sycl)

add_custom_target(run_philox_lognormal philox_lognormal)
add_custom_target(run_philox_normal philox_normal)
add_custom_target(run_philox_poisson philox_poisson)
add_custom_target(run_philox_uniform philox_uniform)