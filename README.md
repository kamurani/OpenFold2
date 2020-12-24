# Toy SE3 transformer
This example illustrates how SE3-transformer works on a really simple dataset.

## Data
I used code: https://github.com/pmocz/nbody-python to generate traces for particles subject to gravitational pull. 
The transformer should predict positions and velocities of particles at step __t+50__ using positions and velocities from step __t__.
To generate this dataset use the script __dataset/generate_dataset.py__

The dynamics looks like:
![Alt Text](dataset/anim.gif)

Energy is appriximatelly conserved:
![Alt Text](dataset/energy.png)

## Results
So far, the train/test results are:
phase | Loss (abs)
------| ---------
Train | 0.009
Test  | 0.112
