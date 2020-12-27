# Gaming-using-OpenCV

This is a basic face movement tracking that can convert face movement into keyboard commands like **UP - DOWN - LEFT  - RIGHT**. I used facial landmarks to detect face and get the nose out of it for better referencing. I have created two versions of it, v1 is using a fixed reference boundary which not work expected properly because we need to come at the same position after each movement. To save this I created V2 which uses position change with respect to the previous position. This is more dynamic and easy to control the moves. No need to set position again and again.

## movement-v1.py
In version1, I used a fixed reference boundary. If nose reference is out of boundary then I calculate the direction of movement. After getting direction I am converting it into keyboard commands using the keyboard library.


## Dependencies
This is the list of dependencies for running this application. 
 * **opencv**
 * **keyboard**


## How to use
1. Download or clone this repository.
2. Extract to some location.
3. First, run **```movement-v1.py```** <br>
4. open any online running game like Subway Surfers or Temple Run.
5. Start doing movements to play game. It will press up-down-left-right based on your movements.
