find_library(PTHREAD_LIBRARY pthread)


rosbuild_add_executable(print_scans print_scans.cpp)
#target_link_libraries(pthread)
target_link_libraries(print_scans ${PTHREAD_LIBRARY})

rosbuild_add_executable(time_scans time_scans.cpp)
#target_link_libraries(pthread)
target_link_libraries(time_scans ${PTHREAD_LIBRARY})

rosbuild_add_executable(log_scans log_scans.cpp)
#target_link_libraries(pthread)
target_link_libraries(log_scans ${PTHREAD_LIBRARY})
