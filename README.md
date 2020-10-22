         # Algorithm-Analysis
    Counting Operations
    
    Example - Compute the Sum of Positive Integers
    Compute the sum 1 + 2 + . . . + n for any positive integer n > 0
    • Three possible algorithms for solving this problem
    
    // Algorithm A
     long sum = 0;
     for (long i=1; i<=n; i++) {
       sum = sum + i;
     }

    // Algorithm B
     long sum = 0;
     for (long i=1; i<= n; i++) {
     for (long j=1; j<=i; j++) {
       sum = sum + 1;
        }
     }
     
     // Algorithm C
      long sum = 0;
      sum = n * (n + 1) / 2;
      
            Scenario
            
       Compare algorithm performance
                                    
     • Create a new Java project called Analysis and implement the class SumIntegers with methods sum_A(), sum_B() and sum_C() as implementations of the algorithms
     presented on the previous slide. Each method takes an int parameter n and returns the long sum of all integers <= n.
     • Call each method with parameter value 10000 and verify that they return the same result.
     • Now, add code to time the execution of each method and print out the execution time in
     anoseconds. Verify that there is a clear order in the execution speed of the algorithms
