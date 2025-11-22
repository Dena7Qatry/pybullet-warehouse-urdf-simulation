# PyBullet Virtual Warehouse Scene with Custom URDF Models

## Overview
A static virtual warehouse scene built in PyBullet using custom URDF files. The simulation features a two-wheel robot surrounded by warehouse objects, captured from three different camera angles. Implemented in Google Colab using DIRECT mode for headless rendering.

## Environment Setup

### Robot Model
Custom two-wheel robot implemented in URDF:
- **Base Link**: Box-shaped chassis
- **Wheels**: Two cylindrical wheels (continuous joints)
- Properties: Visual, collision, and inertial definitions included

### Warehouse Objects
Four custom URDF models created:
1. **Cylinder Pillar**: Vertical support structure
2. **Wall**: Rectangular barrier
3. **Table**: Flat horizontal surface
4. **Crate**: Storage box

Total objects in scene: 7 static objects

### Scene Configuration
- **Ground Plane**: Loaded at z=0
- **Gravity**: -9.807 m/s² (Earth gravity)
- **Layout**: Warehouse-style arrangement
- **Robot Positions Tested**: 
  - Center position
  - Back-left position
  - Right position

## Camera Configuration
Images captured using PyBullet's `getCameraImage()`:
- **Resolution**: 640 × 480 pixels
- **Yaw Angle**: 45°
- **Pitch Angle**: -30°
- **Roll Angle**: 0°
- **Rendering**: All models visible in every viewpoint

## Results
Three camera viewpoints captured:
1. **View 1**: Front-facing perspective
2. **View 2**: Side angle view
3. **View 3**: Elevated overhead view

All objects and robot visible in each frame, demonstrating complete scene coverage.

## Technical Details

### PyBullet DIRECT Mode
Headless rendering mode suitable for:
- Google Colab environments
- Batch processing
- Automated testing
- No GUI overhead

## Future Enhancements
- Dynamic object interactions
- Robot motion simulation
- Sensor integration (LIDAR, cameras)
- Path planning demonstrations
- Real-time control interface
