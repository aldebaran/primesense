##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

add_definitions(-DXN_FORMATS_EXPORTS)
qi_create_lib(XnFormats
  SRC *.h *.cpp
  )
qi_use_lib(XnFormats
  dl
  jpeg
  pthread
  rt
  usb_1
  OpenNI
  XnCore
  )
qi_stage_lib(XnFormats)
