##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

add_definitions(-DXN_CORE_EXPORTS)
qi_create_lib(XnCore
  SRC *.h *.cpp
  )
qi_use_lib(XnCore
  dl
  pthread
  rt
  usb_1
  OpenNI
  )
qi_stage_lib(XnCore)
