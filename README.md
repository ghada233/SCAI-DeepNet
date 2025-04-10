# GoalKeeper Action Prediction (Proof of Concept)

An AI system that suggests optimal goalkeeper dive directions during penalty kicks.

## What's Implemented

- **Object Detection**: YOLOv8 tracks ball and players in real-time video
- **Decision Engine**: Q-learning model processes positions to suggest dive direction (Left/Center/Right)
- **Web Interface**: Flask app displays predictions on processed video

## How It Works

1. Processes input video frame-by-frame
2. YOLOv8 detects:
   - Ball position (bounding box)
   - Kicker position
   - Goalkeeper position
3. Reinforcement learning model analyzes positions and suggests dive direction

## Requirements

- Python 3.8+
- OpenCV
- PyTorch
- Ultralytics (YOLOv8)
- Flask (for web interface)

