README: Virtual Rubik's Cube

Overview
The Virtual Rubik's Cube project simulates a 3D Rubik's Cube in Python, allowing users to interact with and solve it using a graphical interface. The cube can be manipulated with buttons for rotations, scrambled randomly, and even solved programmatically. It uses vpython for 3D rendering and the kociemba library for solving the cube.
![Rubix](https://github.com/user-attachments/assets/022d850f-e958-4ff6-94d5-fd62a3e52b2b)

Features
3D Rubik's Cube Visualization: Built using the vpython library.
Interactive Controls: Rotate cube faces using GUI buttons.
Scramble and Solve: Randomly scramble the cube and solve it programmatically.
Real-time Animations: Smooth face rotation animations.
Solution Finder: Utilizes the Kociemba two-phase algorithm to find an optimal solution for any cube state.
Files
cube.py
This file defines the Rubic_Cube class, which implements:

Cube Initialization: Sets up the cube with color-coded tiles and positions.
Rotations: Clockwise and counterclockwise rotations for all cube faces.
Scrambling: Randomly scrambles the cube.
Animation and Position Tracking: Handles smooth animations and tile positions during rotations.
User Controls: Provides button controls for rotation, scrambling, and solving.
solve_rubiccs_cube.py
This file provides:

Proximity Detection: Identifies the current position of tiles on the cube.
Color Detection: Maps cube tile colors to face labels.
Kociemba Solver Integration: Encodes the cube's current state and computes the solution using the kociemba library.
main.py
This file initializes and starts the cube:

Imports the Rubic_Cube class from cube.py.
Instantiates and runs the Rubik's Cube application.
Prerequisites
Before running the project, ensure you have the following installed:

Python 3.8 or later.
Required Python libraries:
vpython
numpy
kociemba
Install the dependencies using pip:

bash
Copy code
pip install vpython numpy kociemba
How to Run
Clone or download the repository.
Ensure all required dependencies are installed.
Run the application using:
bash
Copy code
python main.py
A graphical interface will appear with the Rubik's Cube.
Usage
Rotate Faces:

Buttons labeled with face names (F, R, B, L, U, D) allow clockwise rotations.
Buttons with a prime (F', R', etc.) perform counterclockwise rotations.
Scramble Cube:

Click the random_move button to scramble the cube randomly.
Solve the Cube:

Use the solution button to calculate the optimal solution.
Click solve it! to animate the solving process.
Controls
Button Label	Action
F	Rotate the front face clockwise.
F'	Rotate the front face counterclockwise.
R	Rotate the right face clockwise.
R'	Rotate the right face counterclockwise.
B	Rotate the back face clockwise.
B'	Rotate the back face counterclockwise.
L	Rotate the left face clockwise.
L'	Rotate the left face counterclockwise.
U	Rotate the top face clockwise.
U'	Rotate the top face counterclockwise.
D	Rotate the bottom face clockwise.
D'	Rotate the bottom face counterclockwise.
random_move	Scramble the cube randomly.
solution	Display the solution to the current state.
solve it!	Automatically solve the cube.
Dependencies
vpython: For 3D visualization.
numpy: For mathematical operations and transformations.
kociemba: For calculating the optimal solution to the cube.
Future Enhancements
Add keyboard shortcuts for more intuitive controls.
Save and load cube states for replaying sessions.
Improve UI with additional visual effects.
Add a tutorial mode to teach solving techniques.
Acknowledgments
Kociemba Algorithm: Used for computing optimal cube solutions.
VPython: For the 3D rendering and animation.
License
This project is open-source and distributed under the MIT License. Contributions and forks are welcome!
