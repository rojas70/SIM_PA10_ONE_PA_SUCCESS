This is the first pivot approach trial that was succesful. 

It used 5 states
:
1) Approach
2) Rotation

3) Moment Alignment

4) Insertion

5) Mating



Params


PD Gains: original 


State 4: cancelation of experienced forces + CONST_FORCE=-1 in the z-direction to push down.



Transitions
State 1-2: 
- Upon contact


State 2-3: 
- Upon contact 
- Setting an 'afterContactDip' param = -0.003m.
- contactPos = currentPos + afterContactDip


State 3-4:
 - if position(2) is < contactPos


State 4-5: 
- If moments in all directions are less than 0.5, and
- There is further movement down, measured by zPosDifference<0.000001


Force Plot 

Statistics


The max and min values for the Force plot is: 1624.840000, -2776.830000

The max and min values for the Filtered Force plot is: 52.055700, -93.004300


The max and min values for the Moment plot is: 1825.110000, -294.554000

The max and min values for the Filtered Moment plot is: 58.138600, -27.085500
