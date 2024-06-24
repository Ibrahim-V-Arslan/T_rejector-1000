# T_rejector-1000
**A Very Simple Neural Network to classify mouse trajectory data**

## Trajectory Rejector:
From a separate project I manually labeled 50k mouse trajectories as good or bad. Using this data
I quickly created a simple classifier to detect good or bad trials.
*(never been tested with external data)*

### Good Example:
![image](https://github.com/Ibrahim-V-Arslan/T_rejector-1000/assets/54143433/e0e6101d-9ffa-43f9-bd83-0ce35e536619)

### Bad Example:
![image](https://github.com/Ibrahim-V-Arslan/T_rejector-1000/assets/54143433/b0edb5f9-de38-4096-9994-1ade6f746dc4)

### Models:
**NN_base_model.hd5**: 91.7% Validation Accuracy

**NN_advanced_model.hd5**: 92.1% Validation Accuracy

**NN_power_model.hd5**: 92.3% Validation Accuracy


## Important Information:

1. trajectories are screen/pixel specific which was 1920*1080px
   
   a. if another screen is used coordinates would need to be converted to be in line with the above
   
3. Trajectories (almost) always have a starting point of y = -450, and  x = 0.
5. Trajectories end when they touch either one of the response boxes
   
   a. Red: y >= 390 and x >= 810
   
   b. Blue: y >= 390 and x <= -810:
