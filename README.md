# Acml_lidarloc
Acml自适应定位和lidar_loc定位两种方法。/There are two methods: ACML Adaptive Positioning and Lidar_loc Positioning.
使用步骤
编译
cd ~/catkin_ws
catkin_make
修改Launch文件，替换AMCL

<node pkg="jie_ware" type="lidar_loc" name="lidar_loc" >
    <param name="base_frame" value="base_footprint" />
    <param name="laser_frame" value="laser" />
</node>
运行修改后的Launch文件
roslaunch jie_ware lidar_loc_test.launch 

