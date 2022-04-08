# CMPS 2200 Reciation 6
## Answers

**Name:**____Will Rodman____


Place all written answers from `recitation-06.md` here for easier grading.







- **1b.**

qsort pivot comparison against a unsorted list: 

|     n |   qsort-fixed-pivot |   qsort-random-pivot |
|-------|---------------------|----------------------|
|    25 |               0.090 |                0.101 |
|    50 |               0.158 |                0.178 |
|   100 |               0.332 |                0.377 |
|   200 |               0.775 |                0.842 |
|   500 |               1.872 |                2.180 |
|  1000 |               4.208 |                4.656 |
|  2000 |               8.400 |                9.154 |
|  5000 |              19.666 |               22.471 |
| 10000 |              44.178 |               48.938 |
| 20000 |              93.022 |               96.976 |

The runtimes of the unsorted list closly converges to quicksorts average 
asymptotic bound of O(n*log(n)). The quicksort algorithum with a fixed pivot has better performance than the quicksort algorithum with a random pivot.

qsort pivot comparison against a sorted list: 

|     n |   qsort-fixed-pivot |   qsort-random-pivot |
|-------|---------------------|----------------------|
|    25 |               0.107 |                0.071 |
|    50 |               0.308 |                0.151 |
|   100 |               1.101 |                0.311 |
|   200 |               3.912 |                0.677 |
|   500 |              26.978 |                1.820 |
|  1000 |              91.842 |                3.728 |
|  2000 |             373.384 |                8.894 |
|  5000 |            2238.232 |               20.989 |
| 10000 |            8883.585 |               46.034 |
| 20000 |           35052.097 |              101.550 |

The runtimes of the unsorted list closly converges to quicksorts average 
asymptotic bound of O(n^2). The quicksort algorithum with a random pivot has better performance than the quicksort algorithum with a random pivot.

- **1c.**

qsort-fixed-pivot vs. tim_sort comparison against a unsorted list: 


|     n |   qsort-fixed-pivot |   tim_sort |
|-------|---------------------|------------|
|    25 |               0.081 |      0.002 |
|    50 |               0.159 |      0.003 |
|   100 |               0.358 |      0.007 |
|   200 |               0.736 |      0.015 |
|   500 |               2.180 |      0.040 |
|  1000 |               4.207 |      0.091 |
|  2000 |               8.037 |      0.166 |
|  5000 |              20.277 |      0.446 |
| 10000 |              43.577 |      1.001 |
| 20000 |              87.879 |      2.190 |

tim_sort vs qsort-random-pivot conpaison against a sorted list: 

|     n |   tim_sort |   qsort-random-pivot |
|-------|------------|----------------------|
|    25 |      0.002 |                0.096 |
|    50 |      0.001 |                0.183 |
|   100 |      0.002 |                0.402 |
|   200 |      0.002 |                0.822 |
|   500 |      0.004 |                2.100 |
|  1000 |      0.008 |                4.384 |
|  2000 |      0.015 |                9.425 |
|  5000 |      0.046 |               23.191 |
| 10000 |      0.083 |               47.035 |
| 20000 |      0.178 |               91.855 |