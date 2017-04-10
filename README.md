# PixyTracker
This is a java adaptation of [FRC 2240's Pixy CMUcam5 usb interface](https://github.com/FRC2240/Vision-2017). It uses the JNI to interface with it.

### Current status of project
- I have built libpixyusb, libusb, libboost_thread, libboost_system, and libboost_chrono for PixyTracker to use. Initially when trying to do this, cmake couldn't find the boost libraries. To fix this, I upgraded /usr/share/cmake-2.8/Modules/FindBoost.cmake to [this upgraded version](https://gitlab.kitware.com/cmake/cmake/raw/9bb8ac8ed28811f6097233b1065b71833a017c0f/Modules/FindBoost.cmake)
- I still need to get WPILib to build so that it can be included with PixyTracker so PixyTracker in turn can be compiled for use through the JNI.
