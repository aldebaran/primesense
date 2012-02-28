##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

add_definitions(-DXN_DEVICE_EXPORTS)
qi_create_lib(XnDeviceFile
  SRC *.h *.cpp
  )
qi_use_lib(XnDeviceFile
  dl
  pthread
  rt
  usb_1
  OpenNI
  XnCore
  XnFormats
  XnDDK
  )
qi_stage_lib(XnDeviceFile)
