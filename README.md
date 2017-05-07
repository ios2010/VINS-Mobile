# VINS-Mobile
## Monocular Visual-Inertial State Estimator on Mobile Phones

VINS-Mobile is a real-time monocular visual-inertial state estimator developed by members of the HKUST Aerial Robotics Group. It runs on compatible iOS devices, and provides localization services for augmented reality (AR) applications. It is also tested for state estimation and feedback control for autonomous drones. VINS-Mobile uses sliding window optimization-based formulation for providing high-accuracy visual-inertial odometry with automatic initialization and failure recovery. The accumulated odometry errors are corrected in real-time using global pose graph SLAM. An AR demonstration is provided to showcase its capability.

**Authors:** Peiliang LI, Tong QIN, Zhenfei YANG, Kejie QIU, and [Shaojie SHEN](http://www.ece.ust.hk/ece.php/profile/facultydetail/eeshaojie) from [HKUST Aerial Robotics Group](http://uav.ust.hk/)

**Videos:**

**Related Papers:**
* [**Monocular Visual-Inertial State Estimation for Mobile Augmented Reality**](http://www.ece.ust.hk/~eeshaojie/ismar2017peiliang.pdf), *P.Li et al (submitted to ISMAR 2017)*
* [**Robust Initialization of Monocular Visual-Inertial Estimation on Aerial Robots**](http://www.ece.ust.hk/~eeshaojie/iros2017tong.pdf), *T.Qin et al (submitted to IROS 2017)*
* [**Monocular Visual-Inertial State Estimation With Online Initialization and Camera-IMU Extrinsic Calibration**](http://ieeexplore.ieee.org/document/7463059/), *Z.Yang et al (T-ASE 2017)*

## 1. Build

The code has been tested on macOS Sierra with Xcode 8.3.1 and compatible with iOS 10.2.1 on iPhone7 Plus.

1.1 Install boost for macOS
```
	$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	$ brew install boost
```
1.2 Download specific opencv2.framework from [here](https://www.dropbox.com/sh/r28gjnue98ro1fa/AACiEH-HUdZxU4852_AytAPPa?dl=0)

1.3 Copy the opencv2.framework to VINS_ThirdPartyLib/opencv2.framework

1.4 Build and Run

1.5 Compatible devices

	iPhone7 Plus, iPhone7, iPhone6s Plus, iPhone6s
	
if you use it with non-plus devices, you may need to modify the UI size at Main.storyboard for adapatering with your screen.

## 2. Citing

If you use VINS-Mobile for academic work, please cite the following publication:

## 3. Acknowledgements

We use [ceres solver](http://ceres-solver.org/) for non-linear optimization and [DBow](https://github.com/dorian3d/DBoW2) for loop detection.

Thanks [Yang Liu](https://github.com/wandermyz) to contribute to this code.

## 4. Licence

The source code is released under [GPLv3](http://www.gnu.org/licenses/) licence.

Welcome to contribute to VINS-Mobile or ask any issues via Github or contacting Peiliang LI <pliap@connect.ust.hk> and Tong QIN <tong.qin@connect.ust.hk>.

For commercial purposes, please contact Shaojie SHEN <eeshaojie@ust.hk>
