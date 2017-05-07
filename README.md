# VINS-Mobile
## Monocular Visual-Inertial State Estimation for Mobile Augmented Reality

VINS-Mobile is a real-time visual-inertial-based augmentged reality system. This code implements an **initilization-free** **monocular** sliding window based **visual-inertial-loop** odometry, which is running on IOS devices in real time.

**Authors:** Peiliang LI, Tong QIN, Zhenfei YANG, Kejie QIU, and [Shaojie SHEN](https://scholar.google.com.hk/citations?user=u8Q0_xsAAAAJ&hl=en) from [HUKST UAV GROUP](http://uav.ust.hk/)

**Videos:**

**Related Papers:**
* **Monocular Visual-Inertial State Estimation for Mobile Augmented Reality**
* [**Robust Initialization of Monocular Visual-Inertial Estimation on Aerial Robots**](http://www.ece.ust.hk/~eeshaojie/iros2017tong.pdf)
* **Monocular Visual-Inertial State Estimation With Online Initialization and Camera-IMU Extrinsic Calibration**
* **Tightly-coupled monocular visual-inertial fusion for autonomous flight of rotorcraft MAVs**

## 1. Build

The code has been tested on macOS Sierra with Xcode 8.3.1 and iOS 10.2.1.

1.1 Install boost for macOS
```
	$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	$ brew install boost
```
1.2 Download specific opencv2.framework from [here](https://www.dropbox.com/sh/r28gjnue98ro1fa/AACiEH-HUdZxU4852_AytAPPa?dl=0)

1.3 Copy the opencv2.framework to VINS_ThirdPartyLib/opencv2.framework

1.4 Build and Run

## 2. Citing

If you use VINS-Mobile for academic work, please cite the following publication:

## 3. Acknowledgements

We use [ceres solver](http://ceres-solver.org/) for non-linear optimization and [DBow](https://github.com/dorian3d/DBoW2) for loop detection.

Thanks [Yang Liu](https://github.com/wandermyz) to contribute to this code.

## 4. Licence

The source code is released under [GPLv3](http://www.gnu.org/licenses/) licence.

Welcome to contribute to VINS-Mobile or ask any issues via Github or contacting Peiliang LI <pliap@connect.ust.hk> and Tong QIN <tong.qin@connect.ust.hk>.

For commercial purposes, please contact Shaojie SHEN <eeshaojie@ust.hk>