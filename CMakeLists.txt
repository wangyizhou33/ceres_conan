cmake_minimum_required(VERSION 3.15)
project(ceres)

find_package(ceres REQUIRED)

add_executable(helloworld helloworld.cc)
target_link_libraries(helloworld PRIVATE Ceres::ceres)

add_executable(robust_curve_fitting robust_curve_fitting.cc)
target_link_libraries(robust_curve_fitting PRIVATE Ceres::ceres)

add_executable(iteration_callback_example iteration_callback_example.cc)
target_link_libraries(iteration_callback_example PRIVATE Ceres::ceres)
