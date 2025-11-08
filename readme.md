# Android IMU Digits Gesture Dataset

## 📋 数据集描述

这是一个使用OnePlus 7T手机IMU传感器采集的手势数字姿势数据集。数据集包含0-9数字手势的IMU传感器数据，适用于手势识别、动作分类等机器学习任务。

### 基本信息
- **总样本数**: 500个CSV文件
- **手势类别**: 数字0-9
- **每个数字样本数**: 50个
- **采集时长**: 每个样本5秒
- **采样频率**: ~100Hz
### 🎯 数据集特点
- **设备**: OnePlus 7T
- **传感器**: 9轴IMU（加速度计、陀螺仪、磁力计）
- **数据格式**: CSV文件
- **样本数量**: 0-9 每个手势50个样本 总共500个样本
- **采集频率**: ~100Hz
- **样本时长**: 每个样本5秒

### 文件命名格式
`imu_complete_data_[数字]_[时间戳].csv`

示例：
- `imu_complete_data_0_20251106_211505.csv` - 数字0的手势样本
- `imu_complete_data_1_20251106_211432.csv` - 数字1的手势样本

### 📊 数据格式
每个CSV文件包含以下列：
- `session_id`: 会话标识符
- `timestamp`: 时间戳（毫秒）
- `label`: 手势标签（0-9）
- `quaternion_w, x, y, z`: 四元数数据
- `position_x, y, z`: 位置数据
- `accelerometer_x, y, z`: 加速度计数据
- `gyroscope_x, y, z`: 陀螺仪数据
- `magnetometer_x, y, z`: 磁力计数据
- `linear_acceleration_x, y, z`: 线性加速度
- `gravity_x, y, z`: 重力数据

### 🗂️ 文件结构
Android-IMU-Digits-Gesture-Dataset/
├── data/
│ ├── imu_complete_data_0_20251106_211505.csv # 数字0手势数据
│ ├── imu_complete_data_1_20251106_212322.csv # 数字1手势数据
│ └── .../
└── readme.md