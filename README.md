## EGCM-EVIO: Real-Time Stereo Event-Inertial Odometry via Event-Guided Feature Extraction and Confidence-Masked Time Surface


### Introduction
EGCM-EVIO is a real-time stereo event-inertial odometry system, deployed on Jetson AGX Orin. EGCM-EVIO proposes Confidence-Masked Time Surface (CM-TS), which suppresses noisy pixels, and Event-Guided Feature Extraction (EGFE) that replaces generic feature extractors. The proposed system achieves consistently competitive performance compared with SOTA methods.

### Datasets Used
To support the research community, we would like to share the bag files used in the manuscripts.
#### Modified DSEC
[DSEC](https://dsec.ifi.uzh.ch/) is a stereo camera dataset in driving scenarios that contains data from two monochrome event cameras and two global shutter color cameras. Because the format of dataset is h5, so we convert all the sequences into bagfiles, including 3 topics: ```/davis/left/events```, ```/davis/right/events```, and ```/imu0```

<div align="center">

| Sequence Name 	|Size | Drive Link| 
|---	|---	|---	|
|**Zurich City 04**| 1.82 GB |[4a](https://drive.google.com/file/d/1dhYyisATuG61OgGmmS2qSNCxyRPLMI0M/view?usp=sharing) |
|<br/>| 0.73 GB| [4b](https://drive.google.com/file/d/1AJgBIFN_TW1LXB598rAyz9I86ToPnFSY/view?usp=sharing) | 
|<br/>| 2.16 GB | [4c](https://drive.google.com/file/d/12_nU93v_42qhwIZtxpNhha4JtE6V9kt5/view?usp=sharing) | 
|<br/>| 1.84 GB| [4d](https://drive.google.com/file/d/1YGMcO4LVIDh_8rZlqtdvfLCYi467INVJ/view?usp=sharing) | 
|**Zurich City 09**| 0.92 GB |[9b](https://drive.google.com/file/d/1IzQZjAiO5vCVDUH3PI7LXKbCt2rw_iEi/view?usp=sharing) |
|**Zurich City 11**| 0.73 GB |[11a](https://drive.google.com/file/d/1L0GXYvQteJfV_EhySC6FDu_T1Bq2a1Jl/view?usp=sharing) |
|<br/>| 4.55 GB |[11b](https://drive.google.com/file/d/1qwTkWYvQ5bgIxxAxjnFxU0kERdBG3ckr/view?usp=sharing) |

</div>


#### Modified VECtor
[VECtor](https://star-datasets.github.io/vector/): "VECtor: A Versatile Event-Centric Benchmark for Multi-Sensor SLAM". We merge the left, right and IMU rosbag into one single bag. The type of event message has been changed from propheesee to dvs message. Bagfiles include 3 topics: ```/davis/left/events```, ```/davis/right/events```, and ```/imu0```.

<div align="center">

| Sequence Name 	|Size | Drive Link| 
|---	|---	|---	|
|**VECtor Dataset**| 0.29 GB |[robot_normal](https://drive.google.com/file/d/1It0ohU3WmZAtO9OaY-f2e88Wm3YEeGcz/view?usp=sharing) |
|<br/>| 1.83 GB |[sofa_normal](https://drive.google.com/file/d/1d_ke4uW-weZNs3mjPPV8DSCXmUtE520c/view?usp=sharing) |
|<br/>| 1.13 GB |[desk_normal](https://drive.google.com/file/d/1Hh-Xz3ECak_OvI2xQtYR8BJordsEs9Sd/view?usp=sharing) |
|<br/>| 1.34 GB |[hdr_normal](https://drive.google.com/file/d/12m4SczbE81O1nlfLMOxyf3b-AmMjwRkT/view?usp=sharing) |

</div>
