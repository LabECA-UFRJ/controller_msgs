cmake_minimum_required(VERSION 3.0.2)
project(controller_msgs)

find_package(catkin REQUIRED COMPONENTS message_generation)

add_message_files(
  DIRECTORY msg
  FILES
  MotorSignal.msg
  Circle.msg
)

generate_messages()

catkin_package(CATKIN_DEPENDS message_runtime)
