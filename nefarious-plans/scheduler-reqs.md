> Note: Write information being prossesed to file to avoid overloading RAM
# Write Schedule 
Input
1. periods.csv
   > **Format:** | # of periods | transition time (mins) | day start-end  |
   > *Optional, add as many lines as nescessary* | period # | duration (mins) | day (as in A,B,C,etc.) |
   
   > Note: add lunch as a period
2. classes.csv
   > **Format:** | class id | class name | length (in periods) | periods availible (for block classes, only put starting period) | max. capacity | min. capacity (*optional*) |
   
   > Note: Each level (e.g. Math I and Math II) should be added as a seperate class
3. students.csv
   > | student id | student name | request 1 class id | request 1 priority | etc...
   > > Priorities:
   > > 0. Garenteed
   > > 1. First choice
   > > 2. Second choice
   > > 3. Third choice
   > > 4. alternate

Protocol
1. Validate inputed data
2. 
