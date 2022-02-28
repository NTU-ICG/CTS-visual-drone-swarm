# Collaborative Target Search with a Visual Drone Swarm: Adaptive Curriculum Embedded  Multi-stage Reinforcement Learning Approach

Code for the paper "Collaborative Target Search with a Visual Drone Swarm: Adaptive Curriculum Embedded  Multi-stage Reinforcement Learning Approach"


Instruction
1. Connect 


Programs List   
1. /Models/
      
    1.1. VisualDrone_single_drone.onnx: Trained neural network model file for single drone target search in ONNX format 

    1.2. VisualDrone_collaborative_drones.onnx: Trained neural network model file for collaborative two drones target search in ONNX format
2. /Control/

    2.1. single_drone_control.py: Python script file for controlling the single drone target search using the model in (1.1)      
    2.2. collaborative_two_drones_control.py: Python script file for controlling the collaborative two drones target search using the model in (1.2)    

System Requirement
1. Ubuntu 18.04 or 20.04
2. AMD architecture device

Dependencies and Software Requirements
1. ROS Melodic or Noetic
2. TelloPy library (https://github.com/hanyazou/TelloPy)
3. PyAV library (https://github.com/PyAV-Org/PyAV)
4. ONNX Runtime
5. Torchvision
6. OpenCV
7. PIL library
8. NumPy
