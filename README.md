# rob314

The hole project has this module but also an identification pipeline [insert link].

### Instalation using Catkin

This repository shall be cloned into [your catktin workspace]/src.

```
git clone https://github.com/arthur-ruback/husky_controller
cd ..
catkin_make 
```

### Use

##### Parameters configuration

The launchfile defined in *launch/pipeline.launch* contains the definition of several parameters.

- kd *[float]* : proportional gain in relation to linear speed

- kw *[float]* : proportional gain in relation to angular speed (rotation)

- target_distance *[float]* : goal distance to target

##### Subscribed topics:
- /cluster_center *[sensor_msgs/PointStamped]*

##### Published topics:
- /cmd_vel *[geometry_msgs/Twist]*

##### Execution

```
roslaunch husky_controller controller.launch
```

