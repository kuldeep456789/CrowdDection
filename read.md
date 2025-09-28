# Crowd Detection Project

This project provides real-time crowd detection, density analysis, and speed estimation using computer vision and deep learning. It leverages YOLOv8 for object detection and includes modules for analysis and tracking.

## Features
- Crowd detection using YOLOv8
- Density and speed analysis
- Video input support
- Modular code structure

## Project Structure
```
real-object/
├── app.py                  # Main application entry point
├── requirements.txt        # Python dependencies
├── yolov8n.pt              # YOLOv8 model weights
├── models/                 # Model-related code
│   ├── model.py
│   ├── serialization.py
│   ├── tasks.py
│   ├── yolov8n.pt
│   └── yolov8n.py
├── modules/                # Analysis, detection, and tracking modules
│   ├── analysis/
│   │   ├── density_analysis.py
│   │   └── speed_estimation.py
│   ├── detection/
│   │   └── crowd.py
│   └── tracking/
│       └── crowd.py
├── static/                 # Static files (e.g., video)
│   └── camera.mp4
└── read.md                 # Project documentation
```

## Installation
1. Clone the repository:
   ```sh
   git clone <repo-url>
   cd real-object
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
To run the main application:
```sh
python app.py
```

If you have a Streamlit dashboard (update the path if needed):
```sh
streamlit run dashboard/app.py
```

## Notes
- Ensure you have the YOLOv8 model weights (`yolov8n.pt`) in the correct directory.
- Place your input video in the `static/` folder or update the path in the code.

## Contributing
Feel free to open issues or submit pull requests for improvements.

---
For any questions, contact the project maintainer.
