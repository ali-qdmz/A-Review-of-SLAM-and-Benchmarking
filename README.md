# 📌 SLAM Review and Benchmarking
**A repository for SLAM algorithm benchmarking in GPS-denied environments.**

This repository contains **benchmarking codes and evaluation results** for various SLAM algorithms tested under **GPS-denied and enclosed environments (EGD)**. The study investigates **vision-based, LiDAR-based, and LiDAR-vision fusion methods** for robotic infrastructure inspection.

---

## 💑 Publication
- 📝 **Title:** A Review of Simultaneous Localization and Mapping for the Robotic-Based Nondestructive Evaluation of Infrastructures
- 📚 **Journal:** Sensors
- 🔗 **[Read the Full Paper](https://www.mdpi.com/1424-8220/25/3/712)**

---

## 📂 Repository Structure
```
├── benchmark_scripts/    # Code for SLAM evaluation
│   ├── vins_mono.py
│   ├── orb_slam2.py
│   ├── lio_sam.py
│   ├── fast_lio2.py
│   ├── aloam.py
│   ├── final.py
│
├── datasets/             # Dataset files used for benchmarking
│   ├── mine_dataset/
│
├── results/              # Benchmarking results & visualizations
│   ├── cpu_usage.png
│   ├── ground_truth_trajectory.png
│   ├── aft_mapped_path.csv
│
├── docs/                 # Documentation
│   ├── methodology.md
│   ├── SLAM_algorithms_review.md
│
├── LICENSE
├── README.md             # Overview of the repository
```

---

<h3 style="color:blue;">🔹 SLAM Algorithms Evaluated</h3>

This study benchmarks the following **SLAM methods**:

| **Algorithm**  | **Type** | **Sensor Modality** |
|---------------|----------|--------------------|
| ORB-SLAM2     | Visual   | Monocular, Stereo, RGB-D |
| VINS-Mono     | Visual   | Monocular Camera IMU  |
| LIO-SAM       | LiDAR    | LiDAR + IMU       |
| Fast-LIO2     | LiDAR    | LiDAR + IMU       |
| A-LOAM        | LiDAR    | LiDAR + IMU       |
| LVI-SAM       | Fusion   | LiDAR + Camera + IMU |
| LINS          | LiDAR    | LiDAR + IMU       |
| LEGO-LOAM     | LiDAR    | LiDAR + IMU |
| SC-LEGO-LOAM  | LiDAR    | LiDAR + IMU |
| SC-FAST-LIO   | LiDAR    | LiDAR + IMU |
| F-LOAM        | LiDAR    | LiDAR + IMU |

---

## 📊 Results

<h3 style="color:green;">📌 Trajectory Error Comparison</h3>
The results include:
- **Accuracy Comparisons:** RMSE plots showing SLAM accuracy
- **Computational Resource Consumption:** Memory and CPU usage and runtime benchmarks
- **Visualizations:** 3D trajectory plots

### **Example Visualizations**
<p><span style="font-size:18px; font-weight:bold;">🔹 Accuracy Comparison:</span></p>

<div align="center">
<img src="results/lidar-accuracy.png" alt="LiDAR-based accuracy" width="400">
<img src="results/vision-accuracy.png" alt="Vision-based accuracy" width="400">
<img src="results/trans-err.png" alt="trans-err" width="400">
</div>


<p><span style="font-size:18px; font-weight:bold;">🔹 Dataset Collection Device:</span></p>

<div align="center">
<img src="datasets/device.png" alt="Accuracy Plot" width="400">
</div>


📌 **More detailed results can be found in the results section of the corresponding paper.**

---

## 🚀 How to Use This Repository
Since this repository **only contains benchmarking codes**, there are no installation steps required. However, to **reproduce the benchmarking results**, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/ali-qdmz/A-Review-of-SLAM-and-Benchmarking.git
   cd A-Review-of-SLAM-and-Benchmarking
   ```
2. Run the relevant SLAM benchmarking script:
   ```bash
   python benchmark_scripts/orb_slam2.py
   ```

## 📩 Contact
For any questions or collaboration opportunities, feel free to reach out:

👤 **Ali Ghadimzadeh Alamdari**  
📧 **[ali.ghadimzadeh@gmail.com]**  
🔗 **[[LinkedIn](https://www.linkedin.com/in/ali-ghadimzadeh-38b12217a/)]**  

---
