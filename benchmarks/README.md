
# Benchmarking

- I decided to run extensive compilation CPU tests before and after switching the faster prosessors. Following result rows show an average of 3 back-to-back runs.
- Ambient temperature during both tests was around 25°C.
- No BIOS settings adjusted after switch. Should run another test suite after adjustments.

## Benchmarks used:

### Phoronix Test Suite
http://www.phoronix-test-suite.com/

### Nench
https://github.com/n-st/nench

## Before CPU upgrade 


<img width="424" alt="E5606compile" src="https://user-images.githubusercontent.com/41569318/118366409-c938ad00-b5a8-11eb-9cf7-e31ff0499568.PNG">

## After X5675 installation


<img width="423" alt="X5675compile" src="https://user-images.githubusercontent.com/41569318/118366410-cb9b0700-b5a8-11eb-8834-d86bd1e04390.PNG">

More detailed results:
https://openbenchmarking.org/result/2105152-HA-IBMX3400X94



## Apache Webserver benchmark
```
 Apache Benchmark 2.4.29
    Static Web Page Serving
    Requests Per Second > Higher Is Better
    2 x Intel Xeon E5606 - mgadrmfb - IBM 69Y4356 . 5919.34 |===============================================================================================================================

    Apache Benchmark 2.4.29
    Static Web Page Serving
    Requests Per Second > Higher Is Better
    2 x Intel Xeon X5675 - mgadrmfb - IBM 69Y4356 . 7926.72 |===============================================================================================================================
```


