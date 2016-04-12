Data from snap assembly work in simulation with the PA10 Robot. Successful and failed trials are included. This data was used in the 2012. Location: Tsukuba, Japan. Dates: 2012

This data contains: (i) Manipulation data and (ii) RCBHT State estimation data, and then there are two global folders. 

(i) Manipulation Data
Angles: Current Joint Angles (7 DoF) Format: time th1 th2 ... th7

CartPos: EndEffector Cartesian Position Format: time x y z r p y

Torques: Wrench data wrt the tool. No gravity compensation. Format: time Fx Fy Fz Mx My Mz

State: State Transition Time Vector. Format: time

(ii) RCBHT Information

- Segments:
contains information about how the original FT data is segmented by a regression fit for all 6 FT axes. Data include: iteration, average magnitude value, maximum magnitude value, minimum magnitude value, start time, finish time, gradient value, and gradient lable.

- Composites:
contains information of how neighboring segments are combined (though affected by MC filtering rules) for all 6 FT axes. Data include iteration, MC label, avg val across segments, root-mean-square value across segments, amplitude value across segments, gradient labels for both segments, start, end, avg time for both segments.

- llBehaviors:
- contains information of how neighboring actions are combined (though affected by LLB filtering rules) for all 6 FT axes. Data is kept in file (.txt) format and also in matlab format (.mat) and include the following info: iteration, llb label, avg. val for mc1 & mc2, avg val for combination of mc1&2, same for rms value and amplitude value, mc label 1 and 2, time they start and finish respectively, and the average time for both of them.
