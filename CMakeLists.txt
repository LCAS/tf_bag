cmake_minimum_required(VERSION 2.8.3)
project(tf_bag)

find_package(catkin REQUIRED)

catkin_python_setup()

catkin_package()


#############
## Install ##
#############

install(PROGRAMS
  scripts/tf_bag.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)


#############
## Testing ##
#############

## Add gtest based cpp test target and link libraries
# catkin_add_gtest(${PROJECT_NAME}-test test/test_tf_bag.cpp)
# if(TARGET ${PROJECT_NAME}-test)
#   target_link_libraries(${PROJECT_NAME}-test ${PROJECT_NAME})
# endif()

## Add folders to be run by python nosetests
# catkin_add_nosetests(test)
