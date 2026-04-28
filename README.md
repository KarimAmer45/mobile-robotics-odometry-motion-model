# Odometry Motion Model

Odometry-based probabilistic motion models from mobile robotics. The implementation covers inverse odometry, likelihood evaluation, posterior grid visualization, and sampling-based pose propagation.

## Run

```bash
python - <<'PY'
import numpy as np
import ex3

u = [[0.0, 0.0, 0.0], [0.5, 0.0, np.pi / 2]]
pose = [2.0, 3.0, 0.0]
alpha = [1.0, 1.0, 0.01, 0.01]
print(ex3.sample_motion_model(pose, u, alpha))
PY
```
