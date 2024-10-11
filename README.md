# OCR Model Conversion from GPU to CPU

## Project Overview

This project demonstrates the conversion of an OCR model from GPU to CPU, using EasyOCR. It focuses on optimizing performance by balancing **accuracy** and **FPS (Frames Per Second)**. The conversion process employs techniques such as **frame skipping** and **batch processing** to ensure the CPU can handle OCR tasks efficiently without sacrificing too much accuracy.

## Key Features

- **GPU-Based OCR Model**: Efficient processing with high FPS and high accuracy.
- **CPU-Based OCR Model**: Optimized for CPU performance using frame-skipping, while maintaining acceptable accuracy.
- **Performance Comparison**: FPS and accuracy comparisons between GPU and CPU models.

## Screenshots

### Accuracy Comparison

![Accuracy Comparison](./screenshots/accuracy_comparison.png)

- **GPU Model**: Processes every frame with high accuracy.
- **CPU Model**: Maintains accuracy despite skipping frames.

### FPS Comparison

![FPS Comparison](./screenshots/fps_comparison.png)

- **GPU Model**: High FPS with minimal lag.
- **CPU Model**: FPS boost due to frame-skipping technique.

## Optimization Techniques

1. **Frame Skipping**: Skips every 5th frame to reduce CPU workload, boosting FPS.
2. **Batch Processing**: Processes frames in batches to increase throughput.
3. **Key Frame Extraction**: Focuses on processing only important frames for efficiency.

## Strategies to Maintain Accuracy and FPS

- **Threshold Adjustments**: Filters low-confidence text predictions.
- **Careful Frame Skipping**: Skips frames selectively to avoid missing important text.
- **Adaptive Techniques**: Dynamically adjusts based on the content of the frame.

## Conclusion

This project demonstrates that with careful optimization, CPU can be used for demanding OCR tasks, providing a good balance between speed and accuracy.
