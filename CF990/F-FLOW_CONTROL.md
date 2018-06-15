
# F. Flow Control
 
## Problem Description (Paraphrased)


## Initial Observations
- Max flow problem ?
 
## Ideas 

- can i use a greedy approach so that for each pipe try whatever setting fullfils the condition on the junction it's coming from ? 


## Review

### Understanding the problem 

- What is the Unknown ? 
the pipe settings f1,..fm to use so that all specified constraints are satisfied 

- What are the data ? 
n: number of junctions
m: number of pipes 
s[i]: Incoming - Outcoming for junction i (if < 0 => received, if > 0 => transfered)
pipe[i]: (xi, yi) describing pipe i that connects junction xi with yi

- What is the condition ? 
all s[i] constraints must be satisfied (i'm not sure if s[i] is an at least value and more can be received/transfered)

- Is it possible to satisfy the condition ? if so when ? 
depends on the input. 
but is there a way to conclude possible or not ? is it possible only if the sum of s[i] values is 0 ? it seems to be from the examples 
and its a set of pipes where all junctions are wired and nothing goes outside of the set of pipes so it has be 0.

- Draw a figure 
https://ibb.co/h3YXAJ

- Suitable notation 
for a solution to be  possible sum (s[i]) for 1 <= i <= n must be = 0

if s[i] < 0 => sum(outgoing edges values from junction i) should be >= |s[i]|
if s[i] > 0 => sum(incoming edges values to junction i) should be >= s[i]

- what are the various parts of the condition ? 


### Key Points and Observations:
- I'm thinking it's about constructing a graph such that the edges have certain values so that a set of constraints on the graph are satisfied 

- it is possible to satisfy all constraints only if the sum of s[i] values is 0 so we can check that at the start 

#### Questions asked 
- can i make any observation that must be true ? like must the sum of all flowing things from the pipes be 0 ?

### Problem Solving Techniques Used:

### Problem Classification / Tags:

### Learning Points:

### Related Problems:

