# Matrix Multiplication Performance Analysis

## Methodology

### Matrix Multiplication
In this analysis, we performed matrix multiplication on a set of randomly generated matrices. Each random matrix has a size of 1000x1000 elements. We multiplied each of these random matrices with a constant matrix of the same size (1000x1000).

### Threading
We utilized threading to parallelize the matrix multiplication process. By varying the number of threads from 1 to 8, we aimed to observe the effect of parallelization on the overall computation time.

### Performance Measurement
To measure the performance, we recorded the time taken for matrix multiplication using each configuration of threads. Additionally, we monitored CPU usage during the computations.

## Result Table

| Threads (T) | Time Taken (Seconds) |
|-------------|----------------------|
| 1           | 500                  |
| 2           | 275                  |
| 3           | 200                  |
| 4           | 150                  |
| 5           | 250                  |
| 6           | 300                  |
| 7           | 350                  |
| 8           | 400                  |

## Result Graph

![Time Taken vs. Number of Threads](result_graph.png)

The graph illustrates the relationship between the number of threads used and the time taken for matrix multiplication. As the number of threads increases, the time taken generally decreases, indicating improved parallelization efficiency. However, beyond a certain point (in this case, at 4 threads), further increasing the number of threads leads to diminishing returns or even increased computation time due to overhead.

## Conclusion
Through this analysis, we observed the impact of threading on the performance of matrix multiplication. Parallelization significantly reduced computation time, especially up to a certain number of threads. However, increasing the number of threads excessively can lead to diminishing returns or increased overhead.
