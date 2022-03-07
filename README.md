# Collaborative Target Search with a Visual Drone Swarm: Adaptive Curriculum Embedded  Multi-stage Reinforcement Learning Approach
### Code for the paper "Collaborative Target Search with a Visual Drone Swarm: Adaptive Curriculum Embedded  Multi-stage Reinforcement Learning Approach"

### Setup
1. Connect the computing center to the same network used by the OptiTrack Mocap Server. It is recommended that the ethernet cable is used for this connection to avoid using multiple wireless adapters.
2. Configure Motive application on the OptiTrack Mocap Server to stream data related to drones to address location `192.168.1.100`
3. Edit `sample.launch` default launch file of `vrpn_client_ros` (use `roscd vrpn_client_ros && cd launch` to navigate to the launch file) to change the IP address from localhost to `192.168.1.100`, used by the OptiTrack Mocap Server
4. Connect a DJI Tello Edu drone using wireless adapter directly or docker container (please refer to the extra instruction)

### Running Program
1. Navigate to the repository folder
2. `cd Control`
3. `python3 single_drone_control.py` for controlling a single drone or `python3 collaborative_two_drones_control.py`for controlling two drones using one computing device for each drone

### Programs List   
1. #### /Models/
    1.1. VisualDrone_single_drone.onnx: Trained neural network model file for single drone target search in ONNX format     
    1.2. VisualDrone_collaborative_drones.onnx: Trained neural network model file for collaborative two drones target search in ONNX format
2. #### /Control/
    2.1. single_drone_control.py: Python script file for controlling the single drone target search using the model in (1.1)      
    2.2. collaborative_two_drones_control.py: Python script file for controlling the collaborative two drones target search using the model in (1.2)    

### System Requirement
1. Ubuntu 18.04 or 20.04
2. AMD architecture device

### Dependencies and Software Requirements
1. ROS Melodic or Noetic
2. TelloPy library (https://github.com/hanyazou/TelloPy)
3. PyAV library (https://github.com/PyAV-Org/PyAV)
4. vrpn_client_ros ROS 1 Package (http://wiki.ros.org/vrpn_client_ros)
5. ONNX Runtime
6. Torchvision
7. OpenCV
8. PIL library
9. NumPy
