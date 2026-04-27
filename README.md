### Traffic Video Analysis Framework

Welcome to the Traffic Video Processing tool. This project is a modular Python framework designed for high-performance vehicle detection and tracking. It leverages specialized **UVH-26 research model weights** integrated with the YOLOv11 architecture, optimized for Google Colab environments with GPU acceleration.

#### Key Features

*   **UVH-26 Integration**: Utilizing specialized research weights for high-accuracy vehicle identification in diverse traffic scenarios.
*   **Advanced Tracking**: Integrated support for both ByteTrack and BoTSORT algorithms, configurable via a simple settings dictionary.
*   **Smoothed Trajectories**: Implements a 30-frame deque buffer and 5-frame moving average smoothing to visualize vehicle paths without jitter.
*   **Dynamic Visuals**: Automatic color-coding for vehicle classes with track ID persistence and automated memory cleanup for inactive objects.
*   **Data Intelligence**: Captures detailed metadata including frame indices, confidence scores, bounding box coordinates, and smoothed centroids (cx, cy).
*   **Export Ready**: Generates both an annotated video for visual review and a comprehensive Excel spreadsheet for further data analysis.

#### How to Use

1.  **Installation**: Run the setup cell to install the Ultralytics library.
2.  **Configuration**: Adjust the CONFIG dictionary in the Main Execution Block to set your confidence thresholds, tracker type, and frame range.
3.  **Paths**: Ensure your UVH-26 weight file (e.g., UVH-26-MV-YOLOv11-S.pt) and .mp4 video file are uploaded to the /content directory.
4.  **Run**: Execute the processing cell. Once finished, you can use the provided download cell to retrieve your results.
