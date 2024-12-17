> Note: Write information being prossesed to file to avoid overloading RAM
# Write Schedule 
## Input
- periods.csv
   > **Format:** | # of periods | transition time (mins) | day start-end  |
   > *Optional, add as many lines as nescessary* | period # | duration (mins) | day (as in A,B,C,etc.) |
   
   > Note: add lunch as a period
- classes.csv
   > **Format:** | class id | class name | length (in periods) | periods availible (for block classes, only put starting period) | max. capacity | min. capacity (*optional*) |
   
   > Note: Each level (e.g. Math I and Math II) should be added as a seperate class
- students.csv
   > | student id | student name | request 1 class id | request 1 priority | etc...
   > > Priorities:
   > > 0. Garenteed 
   > > 1. First choice
   > > 2. Second choice *optional*
   > > 3. Third choice *optional*
   > > 4. alternate
   > > *priorites at the same level will be chosen randomly*

## Protocol
1. Validate inputs
2. Identify periods
3. Assign students with priotity 0 classes
4. For first period, identify any classes with minimum student requirements. Assign students based on their priotity level
5. Assign students to classes based on their priority
*if more students are at a priority than availible seats, students will be chosen randomly*
6. repeat for each period 2-5

## Output
schedule.csv
| Student id | period 1 class id | period 2 class id | ...

---

# Print schedule

## Input 
- Periods .csv
- schedule .csv from **Write Schedule** 
- Mode input (write all or write specific)

## Protocol
1. Validate inputs
2. Identify Periods
3. Create ZIP archive for output
| all | specific |
|---|---|
| 4. Print   |  |
