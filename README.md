# PredRNN-PyTorch Video Task

This project processes video frames, segments fingers, and trains a PredRNN-lite model for video prediction.

## Folder Structure
- `frames_5fps/` - Extracted frames from input video
- `output/` - Preprocessed frames (cropped, denoised, resized)
- `masks/` - Binary masks for finger segmentation
- `segmented/` - Color-segmented finger images
- `predrnn_outputs/` - Model outputs and samples

## Main Steps
1. **Frame Extraction**: Extract frames from `.mp4` video at 5 fps.
2. **Preprocessing**: Crop, denoise, and resize frames to standard size.
3. **Segmentation**: Generate masks and segmented images for fingers.
4. **Training**: Train PredRNN-lite on processed frames or masks.

## Requirements
- Python 3.8+
- PyTorch
- OpenCV
- Pillow
- NumPy

## Usage
See `initial.ipynb` for step-by-step instructions and code.

## Notes
- Large folders and video files are ignored in version control via `.gitignore`.
- Adjust paths and parameters as needed for your dataset.
