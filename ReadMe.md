# Point To Cell [![Build Status](https://travis-ci.org/PeterMitrano/point_to_cell.svg?branch=master)](https://travis-ci.org/PeterMitrano/point_to_cell)

Subscribes to `/point_clicked`, which published PointStamped. Divides by resolution of the map as listed on the ros param server under `/move_base/global_costmap/resolution`. This gives the indeces of the clicked cell in the global costmap.
