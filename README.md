# SLAM Introduction
SLAM is the process by which a mobile robot generates a map of the environment and at the same time uses this map to compute its own location. It is a well-suited solution for precise and robust mapping and localization in many applications including mobile robotics, self-driving cars, unmanned aerial
vehicles, or autonomous underwater vehicles.

# Overview 
Generate an initial map of the environment and extract it from the sensors to obtain
initial information about the environment.The home position of the mobile robot is the
starting point, and then the surrounding landmarks are calculated and extracted according to the generated map and environmental information, and then it begins to move.
The mobile robot begins to move and recursively executes the mapping and positioning
process during the movement, extracts a new map of the surrounding environment and
updates the knowledge of the mobile robot.
The new landmark will be observed and extracted based on the newly extracted map
of the surrounding environment of the new mobile robot location.The mobile robot will
try to associate the newly observed reference point with the previously viewed reference
point. When a new reference point is observed, it is used to update the new position of
the mobile robot. The mobile robot navigates the environment according to the received
update information. The navigation plan changes every time the mobile robot receives
new information.

# Algorithm
![Algorithm Flowchart](https://user-images.githubusercontent.com/66781243/133230865-92a4a169-d406-4d87-ae6f-484b06f70cde.png)

