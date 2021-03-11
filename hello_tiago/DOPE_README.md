# Dope demo:

    1. Launch ```roslaunch hello_tiago dope_demo.launch```
    2. Launch ```rosrun look_to_point look_to_point```
    3. Launch ```roslaunch dope dope.launch```

    In the gazebo env you can add ycb models from the hello_tiago package on a table.
    Point the camera to the table with ```rosrun look_to_point look_to_point"``` Make sure the object you want to detect are known to dope, craker or soupecan is a good start. If the objects are close enough to the camera, dope will publish them on /dope/rgb_points you can view this with ```rosrun image_view image_view image:=/dope/rgb_points```

# Dope todo:

    add local dope config file somewhere and link it to when calling the dope roslaunch. Currentyl the path to the camera info inside the vanilla config file is pointing to the wrong topic name. Need to change this before runing dope with tiago.
