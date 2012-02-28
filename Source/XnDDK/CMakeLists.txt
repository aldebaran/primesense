##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

add_definitions(-DXN_DDK_EXPORTS)
qi_create_lib(XnDDK
  SRC *.h *.cpp
  )
qi_use_lib(XnDDK
  dl
  pthread
  rt
  usb_1
  OpenNI
  XnCore
  XnFormats
  )
qi_stage_lib(XnDDK)
