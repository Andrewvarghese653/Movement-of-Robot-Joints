# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)

```
## Output
### 1. Generic Articulated Robot
<img width="833" alt="Screenshot 2023-11-18 at 11 44 54 AM" src="https://github.com/Andrewvarghese653/Movement-of-Robot-Joints/assets/145822115/2b5e22ab-446e-444d-8551-db37cc1c5958">

</br>
</br>
</br>
</br>

### 2. robot.driveJoints(0,0,0,0,0,0)
<img width="837" alt="Screenshot 2023-11-18 at 11 46 23 AM" src="https://github.com/Andrewvarghese653/Movement-of-Robot-Joints/assets/145822115/0ca7d946-093f-4dd6-8704-73b91e0e78ad">

</br>
</br>
</br>
</br>

### 3. Movement of Joint1
<img width="833" alt="Screenshot 2023-11-18 at 11 49 17 AM" src="https://github.com/Andrewvarghese653/Movement-of-Robot-Joints/assets/145822115/4dffade6-031a-4f8a-9ac8-73ed4ba10fff">

</br>
</br>
</br>
</br>

### 3. Movement of Joint2
<img width="831" alt="Screenshot 2023-11-18 at 11 50 09 AM" src="https://github.com/Andrewvarghese653/Movement-of-Robot-Joints/assets/145822115/13afe672-a2b1-4f9e-aa41-a82e89208fe0">

</br>
</br>
</br>
</br>

### 3. Movement of Joint3
<img width="830" alt="Screenshot 2023-11-18 at 11 51 01 AM" src="https://github.com/Andrewvarghese653/Movement-of-Robot-Joints/assets/145822115/86d8f788-b0e2-44ab-8f61-f30b1df3aef9">

</br>
</br>
</br>
</br>

## Result 
Thus the different robots joints are moved with the help of python list.


