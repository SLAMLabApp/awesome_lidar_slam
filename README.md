# Awesome SLAM
<p align="center">
  <img src="https://img.shields.io/badge/awesome-LiDAR%20SLAM-blue?logo=github" />
  <img src="https://img.shields.io/badge/contributions-welcome-brightgreen" />
  <img src="https://img.shields.io/badge/license-MIT-lightgrey" />
</p>
A curated list of LiDAR-SLAM resources.


## Awesome Evaluation Datasets

| Dataset | Year | LiDAR Type | GNSS | Camera | #Seq | Length | GT Map | GT Trajectory | Platform | Environment |
|:--|:--:|:--|:--:|:--:|:--:|:--:|:--:|:--:|:--|:--|
|  [**CarLA-LOC**](https://yuhang1008.github.io/CARLA-Loc_page/) [📄](https://arxiv.org/abs/2309.08909) | 2024 | Mechanical | ✓ | ✓ | 42 | 6.3km | simulated | simulated | car | rural, urban, diverse weather |
| [**MulRan**](https://sites.google.com/view/mulran-pr/dataset) [📄](https://ieeexplore.ieee.org/document/9197298) | 2020 | Mechanical | ✗ | ✗ | 4 | 41.2km | ✗ | <abbr title="Simultaneous Localization and Mapping">SLAM</abbr> | car | urban, long bridge |
| [**HeLiPR**](https://sites.google.com/view/heliprdataset) [📄](https://arxiv.org/abs/2309.14590) | 2024 | Mechanical + FMCW + MEMS | ✓ | ✗ | 10 | 164km | ✗ | <abbr title="Inertial Navigation System">INS</abbr> + LiDAR | car | urban, long bridge |
| [**Oxford Spires**](https://dynamic.robots.ox.ac.uk/datasets/oxford-spires/) [📄](https://arxiv.org/abs/2411.10546) | 2025 | Mechanical | ✗ | ✓ | 6 | 12.9km | <abbr title="Terrestrial Laser Scanner">TLS</abbr> | <abbr title="Terrestrial Laser Scanner">TLS</abbr> + <abbr title="Iterative Closest Point">ICP</abbr> | handheld | outdoor/indoor oxford |
| [**HILTI-Oxford (Challenge 22)**](https://hilti-challenge.com/dataset-2022.html) [📄](https://arxiv.org/pdf/2208.09825) | 2023 | Mechanical | ✗ | ✓ | 16 | ? | <abbr title="Global Navigation Satellite System">GNSS</abbr> + <abbr title="Inertial Navigation System">INS</abbr> + <abbr title="Ground Control Points">GCP</abbr> | <abbr title="Global Navigation Satellite System">GNSS</abbr> + <abbr title="Inertial Navigation System">INS</abbr> + <abbr title="Ground Control Points">GCP</abbr> | handheld | construction + oxford |
| [**HILTI Challenge 2023**](https://hilti-challenge.com/dataset-2023.html) [📄](https://arxiv.org/pdf/2404.09765) | 2023 | Mechanical | ✓ | ✓ | 15 | ? | <abbr title="Global Navigation Satellite System">GNSS</abbr> + <abbr title="Inertial Navigation System">INS</abbr> + <abbr title="Ground Control Points">GCP</abbr> | <abbr title="Global Navigation Satellite System">GNSS</abbr> + <abbr title="Inertial Navigation System">INS</abbr> + <abbr title="Ground Control Points">GCP</abbr> | handheld + robot | indoor, new construction, parking lot |
| [**KITTI**](https://www.cvlibs.net/datasets/kitti/eval_odometry.php) [📄](https://www.cvlibs.net/publications/Geiger2012CVPR.pdf) | 2012 | Mechanical | ✓ | ✓ | 22 | 39.2km | ✗ | <abbr title="Global Navigation Satellite System">GNSS</abbr> / <abbr title="Inertial Measurement Unit">IMU</abbr> | car | urban |
| [**NTU VIRAL**](https://ntu-aris.github.io/ntu_viral_dataset/) [📄](https://arxiv.org/pdf/2202.00379) | 2022 | Mechanical | ✗ | ✓ | 18 | 1.8km | ✗ | <abbr title="Laser Theodolite + Visual-Inertial Fusion">Laser Theodolite + VI Fusion</abbr> | drone | campus outdoor/indoor |
| [**YUTO MMS**](https://github.com/ausmlab/yutomms?tab=readme-ov-file) [📄](https://journals.sagepub.com/doi/10.1177/02783649241261079) | 2021 | Mechanical | ✓ | ✓ | 4 | 20.1km | ✗ | <abbr title="Real-Time Kinematic">RTK</abbr> | car | tilted Lidar, urban |
| [**Ford AV**](https://avdata.ford.com/) [📄](https://arxiv.org/abs/2003.07969) | 2020 | Mechanical | ✗ | ✓ | 24 | ? | <abbr title="Global Navigation Satellite System">GNSS</abbr> / <abbr title="Inertial Measurement Unit">IMU</abbr> | <abbr title="Global Navigation Satellite System">GNSS</abbr> / <abbr title="Inertial Measurement Unit">IMU</abbr> | car | multi-season |
| [**CADC**](http://cadcd.uwaterloo.ca/) [📄](https://arxiv.org/abs/2001.10117) | 2020 | Mechanical | ✓ | ✓ | 75 | 20km | ✗ | <abbr title="Real-Time Kinematic">RTK</abbr> | car | adverse conditions |
| [**BOREAS**](https://www.boreas.utias.utoronto.ca/#/) [📄](https://arxiv.org/abs/2203.10168) | 2023 | Mechanical | ✓ | ✓ | 45 | 350km | ✗ | <abbr title="Global Navigation Satellite System">GNSS</abbr> / <abbr title="Inertial Measurement Unit">IMU</abbr> / Encoder / <abbr title="Real-Time eXtended">RTX</abbr> | car | multi-season |
| [**VBR**](https://rvp-group.net/slam-dataset.html) [📄](https://arxiv.org/abs/2404.11322) | 2024 | Mechanical | ✓ | ✓ | 16 | 40.5km | <abbr title="Real-Time Kinematic">RTK</abbr> + LiDAR Bundle Adjustment | <abbr title="Real-Time Kinematic">RTK</abbr> + LiDAR Bundle Adjustment | handheld + car | urban, vegetation |
| [**M2DGR-Benchmark**](https://github.com/SJTU-ViSYS/M2DGR) [📄](https://arxiv.org/pdf/2112.13659) | 2021 | Mechanical | ✓ | ✓ | 36 | 10.7km | ✗ | <abbr title="Laser Tracker">Laser Tracker</abbr>, <abbr title="Motion Capture">MoCap</abbr>, <abbr title="Real-Time Kinematic">RTK</abbr> | wheeled robot | indoor/outdoor |
| [**UrbanNavDataset**](https://github.com/IPNL-POLYU/UrbanNavDataset) [📄](https://www.ion.org/publications/abstract.cfm?articleID=17895) | 2021 | Mechanical | ✓ | ✓ | 6 | 19.2km | ✗ | <abbr title="Global Navigation Satellite System">GNSS</abbr> / <abbr title="Inertial Navigation System">INS</abbr> | car | urban canyon |
| [**Tiers**](https://github.com/TIERS/tiers-lidars-dataset) [📄](https://arxiv.org/pdf/2203.03454v1) | 2022 | Mechanical + MEMS | ✗ | ✓ | 10 | ? | ✗ | <abbr title="Motion Capture">MoCap</abbr> / <abbr title="Simultaneous Localization and Mapping">SLAM</abbr> | wheeled robot | indoor, road, forest |
| [**FusionPortableV2**](https://fusionportable.github.io/dataset/fusionportable_v2/#various-platforms-and-scenarios) [📄](https://arxiv.org/abs/2404.08563) | 2024 | Mechanical | ✓ | ✓ | 27 | 38.7 km | <abbr title="Terrestrial Laser Scanner">TLS</abbr> | <abbr title="Real-Time Kinematic Global Navigation Satellite System">RTK-GNSS</abbr> / <abbr title="Laser Tracker">LT</abbr> | car, quadruped, UGV, handheld | diverse |
| [**Multi Lidar Multi UAV**](https://tiers.github.io/multi_lidar_multi_uav_dataset/) [📄](https://arxiv.org/pdf/2310.09165) | 2023 | Mechanical + MEMS | ✗ | ✓ | 25 | ? | ✗ | <abbr title="Motion Capture">MoCap</abbr> | drone | structure, unstructured, indoor |
| [**MARS-LVIG**](https://mars.hku.hk/dataset.html) [📄](https://journals.sagepub.com/doi/abs/10.1177/02783649241227968) | 2024 | MEMS | ✓ | ✓ | 22 | ? | ✗ | <abbr title="Real-Time Kinematic">RTK</abbr> | drone | airfield, island, rural town, valley |
| [**BotanicGarden**](https://github.com/robot-pesg/BotanicGarden) [📄](https://arxiv.org/abs/2306.14137) | 2024 | Mechanical + MEMS | ✓ | ✓ | 33 | 17.1km | <abbr title="Terrestrial Laser Scanner">TLS</abbr> | <abbr title="Terrestrial Laser Scanner">TLS</abbr> + <abbr title="Iterative Closest Point">ICP</abbr> | wheeled robot | garden |
| [**GEODE**](https://github.com/PengYu-Team/GEODE_dataset) [📄](https://arxiv.org/abs/2409.04961) | 2024 | Mechanical + MEMS | ✗ | ✓ | 46 | 64km | <abbr title="Terrestrial Laser Scanner">TLS</abbr> | <abbr title="Motion Capture">MoCap</abbr>, <abbr title="Laser Tracker">Laser Tracker</abbr>, <abbr title="Real-Time Kinematic">RTK</abbr> | handheld, UGV, sailboat, car | diverse degenerate |
| [**HK-MEMS**](https://github.com/RuanJY/HK_MEMS_Dataset) [📄](https://doi.org/10.22541/au.172542976.64204704/v1) | 2024 | Mechanical + MEMS| ✓ | ✓ | 26| 75km | ✗ | <abbr title="Real-Time Kinematic">RTK</abbr> + bus route + altitude | handheld, bus, robot | urban, degenerate, high-speed |
| [**DiTier++**](https://sites.google.com/view/diter-plusplus/) [📄](https://construction-robots.github.io/papers/66.pdf) | 2024 | Mechanical | ✓ | ✓ | 5 | 1.2km | <abbr title="Terrestrial Laser Scanner">TLS</abbr> | <abbr title="Terrestrial Laser Scanner">TLS</abbr> + <abbr title="Iterative Closest Point">ICP</abbr> | quadruped robot | unstructured, park |

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
<summary>MEMS + FNCW datasets</summary>

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




