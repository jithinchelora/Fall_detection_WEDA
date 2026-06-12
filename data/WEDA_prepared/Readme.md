# WEDA_prepared Dataset

## Source
WEDA (Wrist-worn Edge Device Accelerometer) fall detection dataset.  
Original: (https://github.com/joaojtmarques/WEDA-FALL)

## Preprocessing
- Segmented into 3s windows at 100Hz (300 samples per window)
- Two classes: `fall/` and `notfall/`
- Processed using Edge Impulse pipeline

## Structure
WEDA_prepared/
├── fall/        # Accelerometer windows containing fall events
└── notfall/     # Accelerometer windows with normal activities

## Sensor Details
- Axes: X, Y, Z accelerometer
- Gravity axis: Z (~9.8 m/s² at rest)
- Sampling rate: 100Hz
- Window size: 3s (300 samples)

## Notes
- Quick wrist jerks can occasionally trigger false positives
- Dataset aligned to match Modulino Movement Sensor axis orientation on Arduino UNO Q
