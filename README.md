# processed-kitti-lidar

This repository contains the lidar scans from the [Kitti Dataset](http://www.cvlibs.net/datasets/kitti). <br>
The dataset is presented in cylindrical coordinates as described in [(Caccia et al.)](https://arxiv.org/abs/1812.01180) <br>

Specifically, each scan has shape `(2, 40, 512)` where the first two channels are `d=\sqrt{x^2 + y^2}` and `z`. 
`40` is the number of full 360° scans (I cut it down from I think 61 iirc) and `512` is the number of points per scan. 

`NOTE:` about <1% of the scans are missing because the preprocessing failed on those. Use this dataset at your own risk
