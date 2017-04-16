# extended_kalman_filter_python
An Extended Kalman Filter (that uses a constant velocity model) in Python.
This EKF fuses LIDAR and RADAR sensor readings to estimate location (x,y) and velocity (vx, vy).

### Source layout

1. `main.py` - Can run the tracker.
2. `tracker.py` - Instance that tracks and uses EKF to predict and update state.
3. `efk.py` - EKF implementation lives here.
4. `utils.py` - Helper methods.

### Package requirements

1. pandas
2. numpy


### To run the filter

`python main.py`

```
Started Tracker for sample-laser-radar-measurement-data-1.txt
estimations count:  1224
measurements count:  1224
RMSE:  [[ 0.06516487  0.06053792  0.53321165  0.5441927 ]]
Metric:  [0.08, 0.08, 0.6, 0.6]
RMSE PASSED metric


Started Tracker for sample-laser-radar-measurement-data-2.txt
estimations count:  200
measurements count:  200
RMSE:  [[ 0.18549633  0.19030227  0.47675529  0.80446808]]
Metric:  [0.2, 0.2, 0.5, 0.85]
```
