# Android IMU Digits Gesture Dataset

**🌐 Language:** [English](#) | [中文](README_zh.md)

## 📋 Dataset Description

The Android IMU Digits Gesture Dataset comprises time-series data of digits 0-9 hand gestures, collected from the IMU sensors (accelerometer, gyroscope, and magnetometer) of a OnePlus 7T smartphone. This dataset is suitable for gesture recognition, human-computer interaction (HCI), activity classification, and time-series analysis tasks using machine learning models.

### 🎯 Dataset information
- **Device**: OnePlus 7T
- **Sensor**: 9-axis IMU (accelerometer, gyroscope, and magnetometer)
- **Gestures**: Numbers0-9
- **Data format**: csv file
- **Total sample size**: 500 csv files
- **Sample size**: 0-9, 50 samples for each gesture, totaling 500 samples
- **Sample duration**: 5 seconds per sample
- **Acquisition Frequency**: ~100Hz
- **Hand**： Right-hand


### File naming format
`imu_complete_data_[Number]_[YYYYMMDD_HHmmss].csv`

Example：
- `imu_complete_data_0_20251106_211505.csv` - A gesture sample of the number 0
- `imu_complete_data_1_20251106_211432.csv` - A gesture sample of the number 1

### 📊 Data format
Each csv file contains the following:
- `session_id`: Session identifier
- `timestamp`: Timestamp (milliseconds)
- `label`: Gesture label (0-9)
- `quaternion_w, x, y, z`: Quaternion data
- `position_x, y, z`: Position data
- `accelerometer_x, y, z`: Accelerometer data
- `gyroscope_x, y, z`: Gyrosocope data
- `magnetometer_x, y, z`: Magnetometer data
- `linear_acceleration_x, y, z`: Linear acceleration data
- `gravity_x, y, z`: Gravity data

### 🗂️ Dataset Structure
Android-IMU-Digits-Gesture-Dataset/  
├── data/  
│ ├── imu_complete_data_0_20251106_211505.csv # Number 0 gesture data  
│ ├── imu_complete_data_1_20251106_212322.csv # Number 1 gesture data  
│ └── .../  
└── readme.md  
└── readme_zh.md