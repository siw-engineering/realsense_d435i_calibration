# realsense_d435i_calibration
Intel real sense d435i calibration using kalibr 

## calibrating cameras
```
rosrun kalibr kalibr_calibrate_cameras --target /data/config/april_6x6.yaml --bag /data/d435i_7th.bag --models pinhole-equi --topics /camera/color/image_raw
```
## calibrating camera-imu
```
rosrun kalibr kalibr_calibrate_imu_camera --target /data/config/april_6x6.yaml --bag /data/d435i_7th.bag --cam /data/iter2/d435i_7th-camchain.yaml --imu /data/iter1/imu_d435i.yaml
```