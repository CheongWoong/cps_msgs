# cps_msgs
cps_msgs

## Build Instructions
```
# Clone the repo in your ROS workspace directory
cd ~/ros_workspace/src
git clone https://github.com/CheongWoong/cps_msgs.git

# Catkin build
cd ~/ros_workspace
catkin_make
source ./devel/setup.bash
```

## Test
```
# Test if built success
rosmsg show cps_msgs/EstimatedOdom
```

## Example Use (Python)
```
from cps_msgs.msg import EstimatedOdom
estimated_odom = EstimatedOdom()
```
