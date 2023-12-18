# BSE_Optimization_Project


## Part 1 



## Part 2 



## Part 3

Yes, the fractional TSP (FTSP) solution will naturally force the continuous variables x to take on binary values in the optimal solution. While you declare x as continuous, the nature of the TSP problem and the constraints imposed on x will guide the optimization solver to find an optimal solution where the values of x become effectively binary.

In the TSP formulation, the variables x typically represent the decision of whether to include an edge in the tour. Since a city can only be visited once, the solution inherently enforces binary-like behavior on these variables, even if they are formally declared as continuous.

The optimization process will converge to a solution where x takes on values close to 0 or 1, effectively selecting or rejecting each edge in the tour. This is a characteristic of the TSP problem, and in practice, the continuous relaxation is often solved, and the resulting fractional values are then rounded to obtain a feasible integer solution.



This rounding behavior occurs because, in the optimal solution, it is not efficient to include an edge partially. It is generally more cost-effective to either include the edge entirely or exclude it from the tour. This binary-like behavior emerges naturally from the combinatorial structure of the TSP and the requirement that each city must be visited exactly once.

In practice, even though you declare the variables as continuous, the solution you obtain tends to have values very close to 0 or 1, effectively reproducing a binary solution. This allows for a seamless transition between the fractional relaxation and the integral (binary) solution.

## Part 4



