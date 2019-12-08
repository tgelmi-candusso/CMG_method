# Model to estimate seed dispersal distance using movement data (CMG method)
Seed dispersal distance (SDD) estimates using the CMG method (combination of movement data and gut passage). Here I describe the function I created to extract SDD estimates directly from chronologically ordered movement data, obtained through behavioral scan sampling or with tracking devices.
The function is called linear.distances() and it calculates the distance between each consecutive position recorded and the time interval between the two consecutive positions.
The data must be inchronological order, with time, day, month and year in separate columns. 
Time must be in "%H:%M" format.  "%H:%M:%S" can also be used, but then the code must be modified in line25 by deleting the # sign.
X and Y position of each recorded position must be given in UTM coordinates.
To complete the CMG method, daily linear distances provided by the function, should then be restricted to the specific gut passage time, or retention time of the plant species. This is provided at the end of the github file. 
The SDD estimates may then be used for estimating seed dispersal curves or else.
