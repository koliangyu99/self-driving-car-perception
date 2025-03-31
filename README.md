# Self-Driving Car Perception Module

An autonomous perception system for self-driving cars that performs lane detection, object recognition, and distance estimation. Built using PyTorch, YOLOv5, OpenCV, and CARLA simulator.

## 🚘 Features

- 🛣️ **Lane Detection**: Real-time lane line detection using OpenCV and NumPy.
- 🧠 **Object Detection**: Trained YOLOv5 on the KITTI dataset to detect vehicles, pedestrians, and traffic signs with 87% mAP.
- 📏 **Distance Estimation**: Calculated object depth using stereo camera data and Open3D.
- 🏙️ **Simulation**: Tested the system in urban driving scenarios with CARLA.
- 📊 **Visualization**: Used Matplotlib and Open3D to render perception outputs.

## 🛠️ Tech Stack

- **Computer Vision**: OpenCV, Open3D
- **Deep Learning**: PyTorch, YOLOv5
- **Simulation**: CARLA
- **Visualization**: Matplotlib, Open3D
- **Dataset**: KITTI

## 🧪 Training

```bash
# Clone YOLOv5
git clone https://github.com/ultralytics/yolov5
cd yolov5

# Install dependencies
pip install -r requirements.txt

# Train on KITTI dataset
python train.py --img 640 --batch 16 --epochs 50 --data kitti.yaml --weights yolov5s.pt
