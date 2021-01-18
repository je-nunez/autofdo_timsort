
# WIP

This project is a *work in progress*. The implementation is *incomplete* and
subject to change. The documentation can be inaccurate.

# Some measures

This is on the `./benchmarks/bench.cpp` program provided by the
[gfx::timsort library](https://github.com/timsort/cpp-TimSort).

The third column is the results after compiling with
`c++ ... -DNDEBUG -O2 -fauto-profile=<profile-results-fname>.gcov ...`
(c++ GCC version 10.2.1):

       # Size of the sequences to sort in all samples: 100000
        
       RANDOMIZED SEQUENCE
        
       [int]
       timsort          0.704184       0.703736     99.936%
        
       [std::string]
       timsort          2.544316       2.837484    111.522%
        
        
       REVERSED SEQUENCE
        
       [int]
       timsort          0.008871       0.006347     71.548%
        
       [std::string]
       timsort          0.125144       0.122707     98.056%
        
        
       SORTED SEQUENCE
       [int]
       timsort          0.005605       0.004806     85.744%
        
       [std::string]
       timsort          0.113677       0.123705    108.821%


