<h1 align="center" style="font-size:2.5em;">Awesome SLAM</h1>
<p align="center">
  <img src="https://img.shields.io/badge/awesome-LiDAR%20SLAM-blue?logo=github" />
  <img src="https://img.shields.io/badge/contributions-welcome-brightgreen" />
  <img src="https://img.shields.io/badge/license-MIT-lightgrey" />
</p>
A curated list of LiDAR-SLAM resources. 

## Contents

1. [Awesome LiDAR SLAM Algorithms](#awesome-lidar-slam-algorithms)
2. [Awesome SLAM Evaluation Datasets](#awesome-slam-evaluation-datasets)
3. [Awesome SLAM Tools](#awesome-slam-tools)
   - [Visualization Tools](#visualization-tools)
   - [SLAM Frameworks](#slam-frameworks)
   - [Evaluation Tools](#evaluation-tools)
   - [Calibration Tools](#calibration-tools)
   - [Solver Libraries](#solver-libraries)
4. [Awesome SLAM Learning Resources](#awesome-slam-learning-resources)
   - [Free E-Books](#free-e-books)
   - [Free Courses](#free-courses)
5. [Awesome SLAM Research Groups](#awesome-slam-research-groups)


## Awesome LiDAR SLAM Algorithms

| Name | Stars | ROS | ROS2 | Paper |
|:--|:--:|:--:|:--:|:--:|
| [**KISS-ICP**](https://github.com/PRBonn/kiss-icp) | [![GitHub stars](https://img.shields.io/github/stars/PRBonn/kiss-icp.svg?style=social&label=Star&maxAge=2592000)](https://github.com/PRBonn/kiss-icp) |  | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://arxiv.org/abs/2203.03749) |
| [**LIO-SAM**](https://github.com/TixiaoShan/LIO-SAM) | [![GitHub stars](https://img.shields.io/github/stars/TixiaoShan/LIO-SAM.svg?style=social&label=Star&maxAge=2592000)](https://github.com/TixiaoShan/LIO-SAM) | ![ROS 1](https://img.shields.io/badge/ROS%201-blue?logo=ros&logoColor=white) | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://github.com/TixiaoShan/LIO-SAM/blob/master/config/doc/paper.pdf) |
| [**FAST-LIO**](https://github.com/hku-mars/FAST_LIO) | [![GitHub stars](https://img.shields.io/github/stars/hku-mars/FAST_LIO.svg?style=social&label=Star&maxAge=2592000)](https://github.com/hku-mars/FAST_LIO) | ![ROS 1](https://img.shields.io/badge/ROS%201-blue?logo=ros&logoColor=white) | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://github.com/hku-mars/FAST_LIO/blob/main/doc/Fast_LIO_2.pdf) |
| [**GLIM**](https://github.com/koide3/glim) | [![GitHub stars](https://img.shields.io/github/stars/koide3/glim.svg?style=social&label=Star&maxAge=2592000)](https://github.com/koide3/glim) | ![ROS 1](https://img.shields.io/badge/ROS%201-blue?logo=ros&logoColor=white) | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://arxiv.org/abs/2407.20465) |
| [**MOLA**](https://github.com/MOLAorg/mola) | [![GitHub stars](https://img.shields.io/github/stars/MOLAorg/mola.svg?style=social&label=Star&maxAge=2592000)](https://github.com/MOLAorg/mola) |  | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://www.sciencedirect.com/science/article/pii/S0921889024001349?via%3Dihub) |
| [**DLIO**](https://github.com/vectr-ucla/direct_lidar_inertial_odometry) | [![GitHub stars](https://img.shields.io/github/stars/vectr-ucla/direct_lidar_inertial_odometry.svg?style=social&label=Star&maxAge=2592000)](https://github.com/vectr-ucla/direct_lidar_inertial_odometry) | ![ROS 1](https://img.shields.io/badge/ROS%201-blue?logo=ros&logoColor=white) | ![ROS 2](https://img.shields.io/badge/ROS%202-blue?logo=ros&logoColor=white) | [📄](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/vizzo2023ral.pdf) |



## Awesome SLAM Evaluation Datasets
| Dataset | Paper | Year | LiDAR Type | Sensors | #Seq | Length | GT Map | GT Trajectory | Platform | Environment |
|:--|:--|:--:|:--|:--|:--:|:--:|:--:|:--:|:--|:--|
| [**CarLA-LOC**](https://yuhang1008.github.io/CARLA-Loc_page/) | [📄](https://arxiv.org/abs/2309.08909) | 2024 | Mech. | 🛰️📷 | 42 | 6.3km | simulated | simulated | car | rural, urban, diverse weather |
| [**MulRan**](https://sites.google.com/view/mulran-pr/dataset) | [📄](https://ieeexplore.ieee.org/document/9197298) | 2020 | Mech. |  | 4 | 41.2km | ✗ | SLAM | car | urban, long bridge |
| [**HeLiPR**](https://sites.google.com/view/heliprdataset) | [📄](https://arxiv.org/abs/2309.14590) | 2024 | Mech. + FMCW + MEMS | 🛰️ | 10 | 164km | ✗ | INS + LiDAR | car | urban, long bridge |
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) | [📄](https://arxiv.org/abs/2411.10546) | 2025 | Mech. | 📷 | 6 | 12.9km | TLS | TLS + ICP | handheld | outdoor/indoor oxford |
| [**HILTI-Challenge 2022**](https://hilti-challenge.com/dataset-2022.html) | [📄](https://arxiv.org/pdf/2208.09825) | 2023 | Mech. | 📷 | 16 | ? | GNSS + INS + GCP | GNSS + INS + GCP | handheld | construction + oxford |
| [**HILTI Challenge 2023**](https://hilti-challenge.com/dataset-2023.html) | [📄](https://arxiv.org/pdf/2404.09765) | 2023 | Mech. | 🛰️📷 | 15 | ? | GNSS + INS + GCP | GNSS + INS + GCP | handheld + robot | indoor, new construction, parking lot |
| [**KITTI**](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) | [📄](https://www.cvlibs.net/publications/Geiger2012CVPR.pdf) | 2012 | Mech. | 🛰️📷 | 22 | 39.2km | ✗ | GNSS / IMU | car | urban |
| [**NTU VIRAL**](https://ntu-aris.github.io/ntu_viral_dataset/) | [📄](https://arxiv.org/pdf/2202.00379) | 2022 | Mech. | 📷 | 18 | 1.8km | ✗ | Laser Theodolite + VI Fusion | drone | campus outdoor/indoor |
| [**YUTO MMS**](https://github.com/ausmlab/yutomms?tab=readme-ov-file) | [📄](https://journals.sagepub.com/doi/10.1177/02783649241261079) | 2021 | Mech. | 🛰️📷 | 4 | 20.1km | ✗ | RTK | car | tilted Lidar, urban |
| [**Ford AV**](https://avdata.ford.com/) | [📄](https://arxiv.org/abs/2003.07969) | 2020 | Mech. | 📷 | 24 | ? | GNSS / IMU | GNSS / IMU | car | multi-season |
| [**CADC**](http://cadcd.uwaterloo.ca/) | [📄](https://arxiv.org/abs/2001.10117) | 2020 | Mech. | 🛰️📷 | 75 | 20km | ✗ | RTK | car | adverse conditions |
| [**BOREAS**](https://www.boreas.utias.utoronto.ca/#/) | [📄](https://arxiv.org/abs/2203.10168) | 2023 | Mech. | 🛰️📷 | 45 | 350km | ✗ | GNSS / IMU / Encoder / RTX | car | multi-season |
| [**VBR**](https://rvp-group.net/slam-dataset.html) | [📄](https://arxiv.org/abs/2404.11322) | 2024 | Mech. | 🛰️📷 | 16 | 40.5km | RTK + LiDAR Bundle Adjustment | RTK + LiDAR Bundle Adjustment | handheld + car | urban, vegetation |
| [**M2DGR-Benchmark**](https://github.com/SJTU-ViSYS/M2DGR) | [📄](https://arxiv.org/pdf/2112.13659) | 2021 | Mech. | 🛰️📷 | 36 | 10.7km | ✗ | Laser Tracker, MoCap, RTK | wheeled robot | indoor/outdoor |
| [**UrbanNavDataset**](https://github.com/IPNL-POLYU/UrbanNavDataset) | [📄](https://www.ion.org/publications/abstract.cfm?articleID=17895) | 2021 | Mech. | 🛰️📷 | 6 | 19.2km | ✗ | GNSS / INS | car | urban canyon |
| [**Tiers**](https://github.com/TIERS/tiers-lidars-dataset) | [📄](https://arxiv.org/pdf/2203.03454v1) | 2022 | Mech. + MEMS | 📷 | 10 | ? | ✗ | MoCap / SLAM | wheeled robot | indoor, road, forest |
| [**FusionPortableV2**](https://fusionportable.github.io/dataset/fusionportable_v2/#various-platforms-and-scenarios) | [📄](https://arxiv.org/abs/2404.08563) | 2024 | Mech. | 🛰️📷 | 27 | 38.7 km | TLS | RTK-GNSS / LT | car, quadruped, UGV, handheld | diverse |
| [**Multi Lidar Multi UAV**](https://tiers.github.io/multi_lidar_multi_uav_dataset/) | [📄](https://arxiv.org/pdf/2310.09165) | 2023 | Mech. + MEMS | 📷 | 25 | ? | ✗ | MoCap | drone | structure, unstructured, indoor |
| [**MARS-LVIG**](https://mars.hku.hk/dataset.html) | [📄](https://journals.sagepub.com/doi/abs/10.1177/02783649241227968) | 2024 | MEMS | 🛰️📷 | 22 | ? | ✗ | RTK | drone | airfield, island, rural town, valley |
| [**BotanicGarden**](https://github.com/robot-pesg/BotanicGarden) | [📄](https://arxiv.org/abs/2306.14137) | 2024 | Mech. + MEMS | 🛰️📷 | 33 | 17.1km | TLS | TLS + ICP | wheeled robot | garden |
| [**GEODE**](https://github.com/PengYu-Team/GEODE_dataset) | [📄](https://arxiv.org/abs/2409.04961) | 2024 | Mech. + MEMS | 📷 | 46 | 64km | TLS | MoCap, Laser Tracker, RTK | handheld, UGV, sailboat, car | diverse degenerate |
| [**HK-MEMS**](https://github.com/RuanJY/HK_MEMS_Dataset) | [📄](https://doi.org/10.22541/au.172542976.64204704/v1) | 2024 | Mech. + MEMS | 🛰️📷 | 26 | 75km | ✗ | RTK + bus route + altitude | handheld, bus, robot | urban, degenerate, high-speed |
| [**DiTier++**](https://sites.google.com/view/diter-plusplus/) | [📄](https://construction-robots.github.io/papers/66.pdf) | 2024 | Mech. | 🛰️📷 | 5 | 1.2km | TLS | TLS + ICP | quadruped robot | unstructured, park |

**Legend:** 🛰️ GNSS, 📷 Camera


<!--
### Datasets by Platform

<details>
<summary> Car-mounted datasets</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|
|  [**CarLA-LOC**](https://yuhang1008.github.io/CARLA-Loc_page/) [📄](https://arxiv.org/abs/2309.08909) | 2024 | Mechanical | ✓ | ✓ | 42 | 6.3km | simulated | simulated | rural, urban, diverse weather |
| [**MulRan**](https://sites.google.com/view/mulran-pr/dataset) [📄](https://ieeexplore.ieee.org/document/9197298) | 2020 | Mechanical | ✗ | ✗ | 4 | 41.2km | ✗ | SLAM | urban, long bridge |
| [**HeLiPR**](https://sites.google.com/view/heliprdataset) [📄](https://arxiv.org/abs/2309.14590) | 2024 | Mechanical + FMCW + MEMS | ✓ | ✗ | 10 | 164km | ✗ | INS + LiDAR | urban, long bridge |
| [**KITTI**](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) [📄](https://www.cvlibs.net/publications/Geiger2012CVPR.pdf) | 2012 | Mechanical | ✓ | ✓ | 22 | 39.2km | ✗ | GNSS/IMU | urban |
| [**YUTO MMS**](https://github.com/ausmlab/yutomms?tab=readme-ov-file) [📄](https://journals.sagepub.com/doi/10.1177/02783649241261079) | 2021 | Mechanical | ✓ | ✓ | 4 | 20.1km | ✗ | RTK | tilted Lidar, urban |
| [**Ford AV**](https://avdata.ford.com/) [📄](https://arxiv.org/abs/2003.07969) | 2020 | Mechanical | ✗ | ✓ | 24 | ? | GNSS/IMU | GNSS/IMU | multi-season |
| [**CADC**](http://cadcd.uwaterloo.ca/) [📄](https://arxiv.org/abs/2001.10117) | 2020 | Mechanical | ✓ | ✓ | 75 | 20km | ✗ | RTK | adverse conditions |
| [**BOREAS**](https://www.boreas.utias.utoronto.ca/#/) [📄](https://arxiv.org/abs/2203.10168) | 2023 | Mechanical | ✓ | ✓ | 45 | 350km | ✗ | GNSS/IMU/Encoder/RTX | multi-season |
| [**UrbanNavDataset**](https://github.com/IPNL-POLYU/UrbanNavDataset) [📄](https://www.ion.org/publications/abstract.cfm?articleID=17895) | 2021 | Mechanical | ✓ | ✓ | 6 | 19.2km | ✗ | GNSS/INS | urban canyon |

</details>

<details>
<summary>Handheld datasets</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) [📄](https://arxiv.org/abs/2411.10546) | 2025 | Mechanical | ✗ | ✓ | 6 | 12.9km | TLS | TLS + ICP | outdoor/indoor oxford |
| [**HILTI-Oxford (Challenge 22)**](https://hilti-challenge.com/dataset-2022.html) [📄](https://arxiv.org/pdf/2208.09825) | 2023 | Mechanical | ✗ | ✓ | 16 | ? | GNSS/INS + GCP | GNSS/INS + GCP | construction + oxford |
| [**HILTI Challenge 2023**](https://hilti-challenge.com/dataset-2023.html) [📄](https://arxiv.org/pdf/2404.09765) | 2023 | Mechanical | ✓ | ✓ | 15 | ? | GNSS/INS + GCP | GNSS/INS + GCP | indoor, new construction, parking lot |

</details>

<details>
<summary>Drone datasets</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|
| [**NTU VIRAL**](https://ntu-aris.github.io/ntu_viral_dataset/) [📄](https://arxiv.org/pdf/2202.00379) | 2022 | Mechanical | ✗ | ✓ | 18 | 1.8km | ✗ | Laser Theodolite + VI Fusion | campus outdoor/indoor |
| [**MARS-LVIG**](https://mars.hku.hk/dataset.html) [📄](https://journals.sagepub.com/doi/abs/10.1177/02783649241227968) | 2024 | MEMS | ✓ | ✓ | 22 | ? | ✗ | RTK | airfield, island, rural town, valley |
| [**Multi Lidar Multi UAV**](https://tiers.github.io/multi_lidar_multi_uav_dataset/) [📄](https://arxiv.org/pdf/2310.09165) | 2023 | Mechanical + MEMS | ✗ | ✓ | 25 | ? | ✗ | MoCap | structure, unstructured, indoor |
</details>

<details>
<summary>Mixed datasets</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Platform | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|:--|
| [**VBR**](https://rvp-group.net/slam-dataset.html) [📄](https://arxiv.org/abs/2404.11322) | 2024 | Mechanical | ✓ | ✓ | 16 | 40.5km | RTK + LiDAR Bundle Adjustment | RTK + LiDAR Bundle Adjustment | handheld + car | urban, vegetation |
| [**M2DGR-Benchmark**](https://github.com/SJTU-ViSYS/M2DGR) [📄](https://arxiv.org/pdf/2112.13659) | 2021 | Mechanical | ✓ | ✓ | 36 | 10.7km | ✗ | Laser Tracker, MoCAP, RTK | wheeled robot | indoor/outdoor |
| [**Tiers**](https://github.com/TIERS/tiers-lidars-dataset) [📄](https://arxiv.org/pdf/2203.03454v1) | 2022 | Mechanical + MEMS | ✗ | ✓ | 10 | ? | ✗ | MoCap/SLAM | wheeled robot | indoor, road, forest |
| [**FusionPortableV2**](https://fusionportable.github.io/dataset/fusionportable_v2/#various-platforms-and-scenarios) [📄](https://arxiv.org/abs/2404.08563) | 2024 | Mechanical | ✓ | ✓ | 27 | 38.7km | TLS | RTK-GNSS/LT | car, quadruped, UGV, handheld | diverse |
| [**BotanicGarden**](https://github.com/robot-pesg/BotanicGarden) [📄](https://arxiv.org/abs/2306.14137) | 2024 | Mechanical + MEMS | ✓ | ✓ | 33 | 17.1km | TLS | TLS+ICP | wheeled robot | garden |
| [**GEODE**](https://github.com/PengYu-Team/GEODE_dataset) [📄](https://arxiv.org/abs/2409.04961) | 2024 | Mechanical + MEMS | ✗ | ✓ | 46 | 64km | TLS | MoCap, Laser Tracker, RTK | handheld, UGV, sailboat, car | diverse degenerate |
| [**HK-MEMS**](https://github.com/RuanJY/HK_MEMS_Dataset) [📄](https://doi.org/10.22541/au.172542976.64204704/v1) | 2024 | Mechanical + MEMS| ✓ | ✓ | 26| 75km | ✗ | RTK + bus route + altitude | handheld, bus, robot | urban, degenerate, high-speed |
| [**DiTier++**](https://sites.google.com/view/diter-plusplus/) [📄](https://construction-robots.github.io/papers/66.pdf) | 2024 | Mechanical | ✓ | ✓ | 5 | 1.2km | TLS | TLS + ICP | quadruped robot | unstructured, park |
</details>

### Datasets by LiDAR Type
<details>
<summary>Mechanical LiDAR datasets</summary>

| Dataset | Year | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| [**CarLA-LOC**](https://yuhang1008.github.io/CARLA-Loc_page/) [📄](https://arxiv.org/abs/2309.08909) | 2024 | ✓ | ✓ | 42 | 6.3km | simulated | simulated | rural, urban, diverse weather |
| [**MulRan**](https://sites.google.com/view/mulran-pr/dataset) [📄](https://ieeexplore.ieee.org/document/9197298) | 2020 | ✗ | ✗ | 4 | 41.2km | ✗ | SLAM | urban, long bridge |
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) [📄](https://arxiv.org/abs/2411.10546) | 2025 | ✗ | ✓ | 6 | 12.9km | TLS | TLS + ICP | outdoor/indoor oxford |
| [**HILTI-Oxford (Challenge 22)**](https://hilti-challenge.com/dataset-2022.html) [📄](https://arxiv.org/pdf/2208.09825) | 2023 | ✗ | ✓ | 16 | ? | GNSS/INS + GCP | GNSS/INS + GCP | construction + oxford |
| [**HILTI Challenge 2023**](https://hilti-challenge.com/dataset-2023.html) [📄](https://arxiv.org/pdf/2404.09765) | 2023 | ✓ | ✓ | 15 | ? | GNSS/INS + GCP | GNSS/INS + GCP | indoor, new construction, parking lot |
| [**KITTI**](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) [📄](https://www.cvlibs.net/publications/Geiger2012CVPR.pdf) | 2012 | ✓ | ✓ | 22 | 39.2km | ✗ | GNSS/IMU | urban |
| [**NTU VIRAL**](https://ntu-aris.github.io/ntu_viral_dataset/) [📄](https://arxiv.org/pdf/2202.00379) | 2022 | ✗ | ✓ | 18 | 1.8km | ✗ | Laser Theodolite + VI Fusion | campus outdoor/indoor |
| [**YUTO MMS**](https://github.com/ausmlab/yutomms?tab=readme-ov-file) [📄](https://journals.sagepub.com/doi/10.1177/02783649241261079) | 2021 | ✓ | ✓ | 4 | 20.1km | ✗ | RTK | tilted Lidar, urban |
| [**Ford AV**](https://avdata.ford.com/) [📄](https://arxiv.org/abs/2003.07969) | 2020 | ✗ | ✓ | 24 | ? | GNSS/IMU | GNSS/IMU | multi-season |
| [**CADC**](http://cadcd.uwaterloo.ca/) [📄](https://arxiv.org/abs/2001.10117) | 2020 | ✓ | ✓ | 75 | 20km | ✗ | RTK | adverse conditions |
| [**BOREAS**](https://www.boreas.utias.utoronto.ca/#/) [📄](https://arxiv.org/abs/2203.10168) | 2023 | ✓ | ✓ | 45 | 350km | ✗ | GNSS/IMU/Encoder/RTX | multi-season |
| [**VBR**](https://rvp-group.net/slam-dataset.html) [📄](https://arxiv.org/abs/2404.11322) | 2024 | ✓ | ✓ | 16 | 40.5km | RTK + LiDAR Bundle Adjustment | RTK + LiDAR Bundle Adjustment | urban, vegetation |
| [**M2DGR-Benchmark**](https://github.com/SJTU-ViSYS/M2DGR) [📄](https://arxiv.org/pdf/2112.13659) | 2021 | ✓ | ✓ | 36 | 10.7km | ✗ | Laser Tracker, MoCap, RTK | wheeled robot | indoor/outdoor |
| [**UrbanNavDataset**](https://github.com/IPNL-POLYU/UrbanNavDataset) [📄](https://www.ion.org/publications/abstract.cfm?articleID=17895) | 2021 | ✓ | ✓ | 6 | 19.2km | ✗ | GNSS/INS | urban canyon |
| [**FusionPortableV2**](https://fusionportable.github.io/dataset/fusionportable_v2/#various-platforms-and-scenarios) [📄](https://arxiv.org/abs/2404.08563) | 2024 | ✓ | ✓ | 27 | 38.7km | TLS | RTK-GNSS/LT | diverse |
| [**DiTier++**](https://sites.google.com/view/diter-plusplus/) [📄](https://construction-robots.github.io/papers/66.pdf) | 2024 | ✓ | ✓ | 5 | 1.2km | TLS | TLS + ICP | unstructured, park |
</details>


<details>
<summary>MEMS + FMCW datasets</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| [**HeLiPR**](https://sites.google.com/view/heliprdataset) [📄](https://arxiv.org/abs/2309.14590) | 2024 | Mechanical + FMCW + MEMS | ✓ | ✗ | 10 | 164km | ✗ | INS + LiDAR | urban, long bridge |
| [**Tiers**](https://github.com/TIERS/tiers-lidars-dataset) [📄](https://arxiv.org/pdf/2203.03454v1) | 2022 | Mechanical + MEMS | ✗ | ✓ | 10 | ? | ✗ | MoCap/SLAM | indoor, road, forest |
| [**Multi Lidar Multi UAV**](https://tiers.github.io/multi_lidar_multi_uav_dataset/) [📄](https://arxiv.org/pdf/2310.09165) | 2023 | Mechanical + MEMS | ✗ | ✓ | 25 | ? | ✗ | MoCap | structure, unstructured, indoor |
| [**MARS-LVIG**](https://mars.hku.hk/dataset.html) [📄](https://journals.sagepub.com/doi/abs/10.1177/02783649241227968) | 2024 | MEMS | ✓ | ✓ | 22 | ? | ✗ | RTK | airfield, island, rural town, valley |
| [**BotanicGarden**](https://github.com/robot-pesg/BotanicGarden) [📄](https://arxiv.org/abs/2306.14137) | 2024 | Mechanical + MEMS | ✓ | ✓ | 33 | 17.1km | TLS | TLS+ICP | garden |
| [**GEODE**](https://github.com/PengYu-Team/GEODE_dataset) [📄](https://arxiv.org/abs/2409.04961) | 2024 | Mechanical + MEMS | ✗ | ✓ | 46 | 64km | TLS | MoCap, Laser Tracker, RTK | diverse degenerate |
| [**HK-MEMS**](https://github.com/RuanJY/HK_MEMS_Dataset) [📄](https://doi.org/10.22541/au.172542976.64204704/v1) | 2024 | Mechanical + MEMS| ✓ | ✓ | 26| 75km | ✗ | RTK + bus route + altitude | urban, degenerate, high-speed |
</details>


### Datasets by Ground-Truth Map Availability
<details>
<summary>Datasets with Ground Truth Map data</summary>

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) [📄](https://arxiv.org/abs/2411.10546) | 2025 | Mechanical | ✗ | ✓ | 6 | 12.9km | TLS | TLS + ICP | outdoor/indoor oxford |
| [**HILTI-Oxford (Challenge 22)**](https://hilti-challenge.com/dataset-2022.html) [📄](https://arxiv.org/pdf/2208.09825) | 2023 | Mechanical | ✗ | ✓ | 16 | ? | GNSS/INS + GCP | GNSS/INS + GCP | construction + oxford |
| [**HILTI Challenge 2023**](https://hilti-challenge.com/dataset-2023.html) [📄](https://arxiv.org/pdf/2404.09765) | 2023 | Mechanical | ✓ | ✓ | 15 | ? | GNSS/INS + GCP | GNSS/INS + GCP | indoor, new construction, parking lot |
| [**VBR**](https://rvp-group.net/slam-dataset.html) [📄](https://arxiv.org/abs/2404.11322) | 2024 | Mechanical | ✓ | ✓ | 16 | 40.5km | RTK + LiDAR Bundle Adjustment | RTK + LiDAR Bundle Adjustment | urban, vegetation |
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) [📄](https://arxiv.org/abs/2411.10546) | 2025 | Mechanical | ✗ | ✓ | 6 | 12.9km | TLS | TLS + ICP | outdoor/indoor oxford |
| [**FusionPortableV2**](https://fusionportable.github.io/dataset/fusionportable_v2/#various-platforms-and-scenarios) [📄](https://arxiv.org/abs/2404.08563) | 2024 | Mechanical | ✓ | ✓ | 27 | 38.7km | TLS | RTK-GNSS/LT | diverse |
| [**BotanicGarden**](https://github.com/robot-pesg/BotanicGarden) [📄](https://arxiv.org/abs/2306.14137) | 2024 | Mechanical + MEMS | ✓ | ✓ | 33 | 17.1km | TLS | TLS+ICP | garden |
| [**GEODE**](https://github.com/PengYu-Team/GEODE_dataset) [📄](https://arxiv.org/abs/2409.04961) | 2024 | Mechanical + MEMS | ✗ | ✓ | 46 | 64km | TLS | MoCap, Laser Tracker, RTK | diverse degenerate |
| [**DiTier++**](https://sites.google.com/view/diter-plusplus/) [📄](https://construction-robots.github.io/papers/66.pdf) | 2024 | Mechanical | ✓ | ✓ | 5 | 1.2km | TLS | TLS + ICP | unstructured, park |
</details>

-->


## Awesome SLAM Tools

### Visualization Tools
   |  |  |  |  |
   |:--|:--:|:--:|:--:|
   |[**RViz2**](https://docs.ros.org/en/kilted/Tutorials/Intermediate/RViz/RViz-User-Guide/RViz-User-Guide.html) | [![GitHub stars](https://img.shields.io/github/stars/ros2/rviz.svg?style=social&label=Star&maxAge=2592000)](https://github.com/ros2/rviz) | 3D visualization tool for ROS2.|
   |[**Gazebo**](http://gazebosim.org/) |[![GitHub stars](https://img.shields.io/github/stars/gazebosim/gz-sim.svg?style=social&label=Star&maxAge=2592000)](https://github.com/gazebosim/gz-sim) | Robot simulation tool that integrates with ROS and ROS2.
   |[**Open3D**](http://www.open3d.org/) |[![GitHub stars](https://img.shields.io/github/stars/isl-org/Open3D.svg?style=social&label=Star&maxAge=2592000)](https://github.com/isl-org/Open3D) | Library for 3D data processing and visualization.
   |[**CloudCompare**](https://cloudcompare.org/) |[![GitHub stars](https://img.shields.io/github/stars/CloudCompare/CloudCompare.svg?style=social&label=Star&maxAge=2592000)](https://github.com/CloudCompare/CloudCompare) | 3D point cloud and mesh processing software.
   |[**Polyscope**](https://polyscope.run/) |[![GitHub stars](https://img.shields.io/github/stars/nmwsharp/polyscope.svg?style=social&label=Star&maxAge=2592000)](https://github.com/nmwsharp/polyscope) | A C++ library for 3D visualization with Python bindings.

   ### Evaluation Tools
   | |  |  |
   |:--|:--:|:--|
   | [**KITTI Evaluation Toolkit**](http://www.cvlibs.net/datasets/kitti/eval_odometry.php) |  | Official evaluation toolkit for KITTI odometry benchmark. |
   | [**Evo**](https://github.com/MichaelGrupp/evo) | [![GitHub stars](https://img.shields.io/github/stars/MichaelGrupp/evo.svg?style=social&label=Star&maxAge=2592000)](https://github.com/MichaelGrupp/evo) | Evaluation tool for 3D SLAM algorithms. |

   ### Calibration Tools
   | | |  |
   |:--|:--:|:--|
   | [**camera_calibration**](https://github.com/puzzlepaint/camera_calibration) | [![GitHub stars](https://img.shields.io/github/stars/puzzlepaint/camera_calibration.svg?style=social&label=Star&maxAge=2592000)](https://github.com/puzzlepaint/camera_calibration/) | Accurate geometric camera calibration. |
   | [**kalibr**](https://github.com/ethz-asl/kalibr) | [![GitHub stars](https://img.shields.io/github/stars/ethz-asl/kalibr.svg?style=social&label=Star&maxAge=2592000)](https://github.com/ethz-asl/kalibr/) | Multi-camera, visual-inertial and rolling shutter camera calibration toolbox. |
   | [**mrcal**](http://mrcal.secretsauce.net) | [![GitHub stars](https://img.shields.io/github/stars/dkogan/mrcal.svg?style=social&label=Star&maxAge=2592000)](https://github.com/dkogan/mrcal/) | Toolkit for camera calibration and more. |

   ### Least Squares Solver Libraries
   |  |  |  |
   |:--|:--:|:--|
   | [**Ceres solver**](http://ceres-solver.org) | [![GitHub stars](https://img.shields.io/github/stars/ceres-solver/ceres-solver.svg?style=social&label=Star&maxAge=2592000)](https://github.com/ceres-solver/ceres-solver) | C++ library for modeling and solving large, complicated optimization problems. |
   | [**g2o**](https://github.com/RainerKuemmerle/g2o) | [![GitHub stars](https://img.shields.io/github/stars/RainerKuemmerle/g2o?style=social&label=Star&maxAge=2592000)](https://github.com/RainerKuemmerle/g2o) | C++ framework for optimizing graph-based nonlinear error functions. |
   | [**GTSAM**](https://gtsam.org/) | [![GitHub stars](https://img.shields.io/github/stars/borglab/gtsam?style=social&label=Star&maxAge=2592000)](https://github.com/borglab/gtsam) | C++ library for factor graphs and Bayes networks optimizations towards SLAM, VO and SFM. |


 ## Awesome SLAM Learning Resources
### Free E-Books
- [**SLAM for Dummies**](https://dspace.mit.edu/bitstream/handle/1721.1/119149/16-412j-spring-2005/contents/projects/1aslam_blas_repo.pdf) by BC Williams: A beginner-friendly tutorial that introduces the SLAM problem, focusing on Kalman Filters and the mathematical foundations of SLAM.
- [**SLAM Handbook**](https://github.com/SLAM-Handbook-contributors/slam-handbook-public-release/blob/main/main.pdf) by Various Authors: A comprehensive guide to SLAM techniques and applications.
- [**Handbook of Robotics: Simultaneous Localization and Mapping**](https://users.dimi.uniud.it/~antonio.dangelo/Robotica/2018/helper/Handbook-SLAM.pdf) by Sebastian Thrun and John J. Leonard: A comprehensive chapter from the "Handbook of Robotics" that delves into the theory and applications of SLAM, including probabilistic methods and real-world challenges.

### Free Courses
- [**SLAM Course Video Lectures by Cyrill Stachniss**](https://www.youtube.com/playlist?list=PLgnQpQtFTOGQrZ4O5QzbIHgl3b1JHimN): A series of video lectures covering the fundamentals and advanced topics in SLAM.
- [**Online Training – Mobile Robotics**](https://www.ipb.uni-bonn.de/online-training-robotics/index.html): A comprehensive online course on mobile robotics, including SLAM techniques, offered by the University of Bonn.

## Awesome SLAM Research Groups
- [**Autonomous Systems Lab (ASL), ETH Zurich**](https://asl.ethz.ch/): A leading research group focusing on autonomous systems, including SLAM and robotics.
- [**Robotics and Perception Group, University of Zurich**](https://rpg.ifi.uzh.ch/): A research group specializing in computer vision, SLAM, and robotics.
- [**Computer Vision and Geometry Group, ETH Zurich**](https://cvg.ethz.ch/): A research group focusing on computer vision, 3D reconstruction, and SLAM.
- [**HKU-MARS Lab**](https://mars.hku.hk/): A research lab at the University of Hong Kong focusing on mobile robotics and SLAM.
- [**Autonomous Intelligent Systems (AIS) Group, Bonn University**](https://ais.uni-bonn.de/): A research group focusing on autonomous systems, including SLAM and robotics.
- [**Oxford Robotics Institute**](https://ori.ox.ac.uk/): A research institute at the University of Oxford specializing in robotics and computer vision.
- [**KAIST Urban Robotics Lab**](https://urobot.kaist.ac.kr/): A research lab at KAIST focusing on urban robotics and SLAM.
