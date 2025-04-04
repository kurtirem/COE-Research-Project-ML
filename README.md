# COE_Group3 Abaqus-Nanoindentation-Project
## Welcome to the Abaqus Nanoindentation Project. This README.md file contains information on how one can start running multiple Abaqus test runs simultaneously. 
Author: Youngbin Pyo, Irem Kurt

### The following project can be done using two different approaches. The first option is implementing a loss function and ML algorithm to predict several points on the force-displacement curve explained in Stage 3-1. The second approach is to use iterative calibration using a direct regression model shown in Stage 3-2.

![image](https://github.com/user-attachments/assets/a7f3f967-92ec-4c79-a69f-667f7cc583ec)

![image](https://github.com/user-attachments/assets/71135a75-8508-4238-8b34-a071bf8e21ea)


### The current files are set for experiments onto DP1000 grains 1441, 2744, and 3198 (please update this if you use a new material).
- The configurations for the simulation can be changed in configs/global_config.xlsx
* The parameters can be found in the paramInfo directory
+ The parameter settings and FD curve data points can be found in files inside the results folder
- The simulation directory contains templates and additional generated files for all the simulations that have been executed
* The targets directory contains data points on the aimed target curve
+ The template directory contains file sets needed for each independent simulation

All simulations can be run using the pipeline.py file.
```
python3 pipeline.py
```

# Acknowledgments
Special acknowledgments to Rongfei Juan for her invaluable support throughout the entire process. Her continuous feedback, guidance, and provision of essential simulation templates have significantly contributed to the success of this project. We extend our sincere gratitude for their collaborative spirit and assistance.

Special thanks to Binh for providing invaluable assistance in resolving the challenges associated with pushing large data files to GitHub.

Gratitude to Professor Junhe Lian for their outstanding efforts in organizing and facilitating the course.
