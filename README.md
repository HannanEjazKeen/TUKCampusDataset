# Drive on Pedestrian Walk. TUK Campus Dataset

This github repository is build as an additional resource for a paper accepted in **2021 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS2021)**. The paper is titled as *"Drive on Pedestrian Walk. TUK Campus Dataset"*.

This work presents a novel campus dataset from the Technical University Kaiserslautern campus, recorded over a span of one year for an autonomous bus project.

John Deere’s Gator X855D is used for the work equipped with an inertial GPS navigation system, stereo cameras, monocular camera, and lidar sensors. For pedestrian safety during autonomous driving, the sensors are attached to capture the view of all four directions. Each sensor is calibrated with respect to the rear axle center of the vehicle and the intrinsic/extrinsic calibration values are provided.

Here is a short comparison to provide the novality of our dataset.

| Datasets        | Sensors           | Vehicle |  Large Scale |  Light Conditions |  Ground Truth |
| ------------- |:-------------------:|:-------:|:------------:|:-----------------:|:-------------:|
| [NCLT]()      | 3D Lidar, Omnidirectional Camera, IMU, RTK GPS | No | Yes | Yes | Yes |
| [KITTI]()     | 3D Lidar, 2x Stereo Systems, Inertial GPS      |   Yes | Yes | No | Yes |
| [Ford]()      | 3D Lidar, 2x Push Broom Lidar, Omnidirectional Camera, IMU, GPS     |  Yes | Spatially | No | No |
| [USYD]()      | Six cameras, 3D Lidar, GPS + IMU      |   Yes | Temporally | Yes | Yes |
| **TUK**       | 3D Lidar, 2x 2D Lidar, 2x Stereo Cameras, Omnidirectional Camera, IMU, 2x GPS     |  Yes | Yes | Yes | Yes |


The sensor configuration is provided in following image.

![alt text](https://github.com/HannanEjazKeen/TUKCampusDataset/blob/main/etc/sensor_configuration.png)


The hierarchy of the folders within the dataset is provided in the image below. Each sequence starts with *tuk* with sequence number.

![alt text](https://github.com/HannanEjazKeen/TUKCampusDataset/blob/main/etc/dataset_hierarchy.png)

This repository includes the following resources:

1. Calibration/Transformation of each sensor with respect to the rear axel of Gator. (calibration.xml)
2. Ground truth trajectories for each sequence in dataset. (ground_truth)
3. Sample data files files in the format of jpg and pcd. ([sample_data](https://github.com/HannanEjazKeen/TUKCampusDataset/tree/main/sample_data)). This folder also include sample labeled data.
4. Sample codes to read the .bin and .jpg files and draw trajectory for read-to-use purpose (codes)
5. Evaluation results over several algorithm ([evaluation](https://github.com/HannanEjazKeen/TUKCampusDataset/tree/main/evaluation))
6. Finally some resource from the paper is also available for citation purposes ([etc](https://github.com/HannanEjazKeen/TUKCampusDataset/tree/main/etc))

Our [group](https://agrosy.informatik.uni-kl.de/en/) has 20 years of experience in the field of autonomous mobile robotics. For further information, we keep updating our campus [dataset page](https://agrosy.informatik.uni-kl.de/en/research/data-sets/tuk-campus).
