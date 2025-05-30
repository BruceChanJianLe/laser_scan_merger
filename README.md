# A ROS2 Laser Scan Merger

> A multithreaded laser scan merger, aims to be blazingly fast.
> This package merges up to 9 laser scans with approximate time filter.

![Image](https://github.com/user-attachments/assets/f521140c-4b02-4bea-b2de-64526983cb3d)

## Build

1. Create workspace
```bash
mkdir ls_ws/src -p
cd ls_ws/src
git clone https://github.com/BruceChanJianLe/laser_scan_merger.git --recurse-submodules
```

2. Install dependencies
```bash
cd ls_ws
rosdep install --from-paths src --ignore-src -r -y
colcon build --symlink-install
source install/setup.bash
```

## Usage

1. Run demo
```bash
ros2 launch dual_laser_merger demo_laser_merger.launch.py
```
