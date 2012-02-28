##
## Author(s):
##  - Samuel MARTIN <smartin@aldebaran-robotics.com>
##
## Copyright (C) 2012 Aldebaran Robotics

qi_create_bin(XnSensorServer
  SRC *.cpp
  )
qi_use_lib(XnSensorServer
  dl
  pthread
  rt
  usb_1
  OpenNI
  XnCore
  XnFormats
  XnDDK
  XnDeviceSensorV2
  )
