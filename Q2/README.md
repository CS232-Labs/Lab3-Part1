
## Lab 3 Problem Statement

### Question 2

You are required to write a MIPS assembly language program named `queryProcessing.s` that takes the following input:

- An integer `n`, followed by `n` **distinct elements**, each on a new line.
- An integer `q`, representing the number of queries followed by `q` numbers, each on a new line.

The program should process the queries in the order they are provided. For each query, if the queried number is present in the array of `n` elements, the program should output the count of elements in the array that are smaller than the queried number. However, if the queried number is not found in the array, the program should output -1. Each output number should be printed on a new line.

To run the program, the following command will be used:

```shell
spim -f queryProcessing.s < test_input_file_name.txt > test_output.txt
```

### Input Format

n

a<sub>1</sub>

a<sub>2</sub>

.

.

.

a<sub>n</sub>

q

p<sub>1</sub>

p<sub>2</sub>

.

.

.

p<sub>q</sub>


### OUTPUT FORMAT:
r<sub>1</sub>

r<sub>2</sub>

.

.

.

r<sub>q</sub>

Where r<sub>1</sub>, r<sub>2</sub>, …, r<sub>q</sub> are the responses of the q queries respectively.

**PLEASE TAKE NOTE OF THE FOLLOWING CONSTRAINTS:**
- 1 <= n <= 10,000
- 1 <= q <= 10,000

**TIME CONSTRAINTS:**
- The program must execute **within 5 seconds** for each test input on linux machines.
- Note that the naive approach of linearly iterating over the elements for each query won't pass all of the testcases due to this time constraint. 

**NOTE:**
- Don't worry about the top lines in the output that are printed by SPIM itself. We will take care of that.
- Make sure that your code is **well-commented**

**SAMPLE INPUT**
```shell
10
4
5
2
11
9
8
33
7
6
10
5
1
33
5
8
2
```


**SAMPLE OUTPUT**
```shell
-1
9
2
5
0
```
