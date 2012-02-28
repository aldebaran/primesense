##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

add_definitions(-DXN_DEVICE_EXPORTS)
qi_create_lib(XnDeviceSensorV2
  SRC *.h *.cpp
  )
qi_use_lib(XnDeviceSensorV2
  dl
  pthread
  rt
  usb_1
  OpenNI
  XnCore
  XnFormats
  XnDDK
  )
qi_stage_lib(XnDeviceSensorV2)
