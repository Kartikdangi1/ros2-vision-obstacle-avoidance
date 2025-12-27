# ROS2 Vision-Based Obstacle Avoidance

A complete robotics project demonstrating vision-based obstacle detection and autonomous navigation using ROS2, YOLOv8, and Gazebo.

## Project Structure

```
ros2-vision-obstacle-avoidance/
├── src/my_awesome_robot/
│   ├── urdf/              # Robot URDF definitions
│   ├── launch/            # ROS2 launch files
│   ├── scripts/           # Python ROS2 nodes
│   ├── config/            # Configuration files
│   ├── package.xml        # ROS2 package metadata
│   └── CMakeLists.txt     # Build configuration
├── docs/                  # Documentation & demos
├── tests/                 # Unit tests
└── README.md
```

## Quick Start

### Build
```bash
colcon build
source install/setup.bash
```

### Run
```bash
# Full system with Gazebo + RViz
ros2 launch my_awesome_robot spawn_robot.launch.py

# In another terminal, start perception + control
ros2 launch my_awesome_robot all.launch.py
```

## Components

- **URDF Robot Definition**: Differential drive robot with camera
- **Perception Pipeline**: YOLOv8-based obstacle detection
- **Control System**: Obstacle avoidance navigation
- **Gazebo Simulation**: Warehouse environment
- **RViz Visualization**: Real-time state monitoring

## Tech Stack

- **ROS2 Humble**
- **Gazebo**
- **RViz2**
- **YOLOv8**
- **Python 3.10+**

---

**Status**: Week 1 - Project Setup  
**Last Updated**: $(date)
