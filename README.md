# YOLO11 Epipolar Distance Lab

Final computer vision practice: YOLO11 object detection + epipolar geometry distance estimation, validated with iPhone LiDAR (RGB-D) across multiple distance ranges.

## Project contents
- `final-practice.ipynb`: main notebook with the full pipeline and analysis.
- `Final Practice.pdf`: assignment statement.
- `img/`: RGB sets and RGB-D (Polycam keyframes + depth/confidence).
- `datasets/`: training data (if needed).
- `yolo11*.pt`: pretrained YOLO11 weights used in the notebook.

## Requirements
- Python 3.9+
- JupyterLab / Jupyter Notebook
- OpenCV, NumPy, Matplotlib
- Ultralytics (YOLO)

## How to run
1. Open the notebook:
   ```bash
   jupyter lab
   ```
2. Run `final-practice.ipynb` from top to bottom.

## Export to PDF (optional)
If you want a PDF export:
- Install Pandoc and LaTeX (xelatex), then run:
  ```bash
  jupyter nbconvert --to pdf "final-practice.ipynb"
  ```

## Notes
- RGB-D validation uses iPhone LiDAR depth (Polycam keyframes).
- RGB-only distance uses epipolar geometry with an EXIF-based K approximation.
