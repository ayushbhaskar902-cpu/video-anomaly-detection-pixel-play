# video-anomaly-detection-pixel-play
# Video Anomaly Detection – Pixel Play '26

## Task
Detect anomalous events in pedestrian surveillance videos.

## Dataset
Avenue Dataset (Pedestrian Surveillance).
Training videos contain mostly normal behavior.
Testing videos contain anomalies such as running and unusual actions.

## Baseline Approach
- Frame-level anomaly detection
- Convolutional Autoencoder
- Trained only on normal frames
- Reconstruction error used as anomaly score

## Evaluation Metric
AUC (Area Under ROC Curve)

## Current Status
- Baseline model implemented
- Submission generated and evaluated on leaderboard

## Next Steps
- Temporal smoothing
- Motion-based models (Conv3D, Frame Prediction)
## Baseline – Frame-level Autoencoder

**Approach**
- Trained a convolutional autoencoder on normal frames only
- Used reconstruction error as anomaly score
- Generated frame-wise anomaly scores for test videos

**Results**
- Public AUC: **0.36206**

**Notes**
- Raw frame-level scores are noisy
- Temporal smoothing is expected to significantly improve performance
