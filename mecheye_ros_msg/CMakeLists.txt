cmake_minimum_required(VERSION 3.0.2)
project(mecheye_ros_msg)

find_package(catkin REQUIRED std_msgs sensor_msgs message_generation genmsg)

add_service_files(
  DIRECTORY
  srv
  FILES
  Set2DExposureTime.srv
  Set2DROI.srv
  Set2DSharpenFactor.srv
  Set2DToneMappingEnable.srv
  Set3DExposure.srv
  Set3DGain.srv
  Set3DROI.srv
  SetCloudOutlierFilterMode.srv
  SetCloudSmoothMode.srv
  SetCurrentUserSet.srv
  SetDepthRange.srv
  SetFringeContrastThreshold.srv
  SetFringeMinThreshold.srv
  SetLaserSettings.srv
  AddUserSet.srv
  CaptureColorMap.srv
  CaptureColorPointCloud.srv
  CaptureDepthMap.srv
  CapturePointCloud.srv
  Connect.srv
  DeleteUserSet.srv
  DeviceInfo.srv
  Disconnect.srv
  Get2DExpectedGrayValue.srv
  Get2DExposureMode.srv
  Get2DExposureSequence.srv
  Get2DExposureTime.srv
  Get2DROI.srv
  Get2DSharpenFactor.srv
  Get2DToneMappingEnable.srv
  Get3DExposure.srv
  Get3DGain.srv
  Get3DROI.srv
  GetAllUserSets.srv
  GetCloudOutlierFilterMode.srv
  GetCloudSmoothMode.srv
  GetCurrentUserSet.srv
  GetDepthRange.srv
  GetDeviceList.srv
  GetFringeContrastThreshold.srv
  GetFringeMinThreshold.srv
  GetLaserSettings.srv
  SaveAllSettingsToUserSets.srv
  Set2DExpectedGrayValue.srv
  Set2DExposureMode.srv
  Set2DExposureSequence.srv
)

generate_messages(
  DEPENDENCIES
  std_msgs
  sensor_msgs
)

catkin_package(CATKIN_DEPENDS std_msgs sensor_msgs message_runtime)
