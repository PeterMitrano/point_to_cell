# Point To Cell [![Build Status](https://travis-ci.org/PeterMitrano/point_to_cell.svg?branch=master)](https://travis-ci.org/PeterMitrano/point_to_cell)

# The scripts
### point_to_cell

Subscribes to `/point_clicked`, which is published by rviz. Divides by resolution of the map as listed on the ros param server. This gives the indeces of the clicked cell in the global costmap.


### point_t_cost

Subscribes to `/point_clicked`, which is published by rviz. Divides by resolution of the map as listed on the ros param server. This gives the indeces of the clicked cell in the global costmap and also subscribes to the costmap, and gives the cost at the cell.

Note: This isn't a perfect match to what is in the costmap layers themselves because I can't figure out how costmap_2d maps from the 0-100 that OccupancyGrid gives to their 0-255. But it's close enough.

## test_cost

This is specific to demonstration_layer. It takes a cell location and feature vector and gives the cost under the current demo_layer.


