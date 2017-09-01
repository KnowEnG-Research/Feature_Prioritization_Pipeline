# Verification directory files are benchmark result files
The Makefile in the test directory contains the targets, needed to build the **Feature Prioritization Pipeline** benchmarks.
For estimating base memory requirements use the above heuristic _feature_prioritization_p_memory_estimator.xlsx_


* Follow the instructions on the **Feature Prioritization Pipeline** landing page to set up the environment:
```
    cd Feature_Prioritization_Pipeline/test
    make env_setup
```
### 1. Run the single drug small data test
```
    make run_small_data_pearson
```

* Compare the results with files in directory: **TEST_1_results_pearson/**

* The local result files will be in **run_dir/results/** 

### 2. Run the multi-drug samll data test **test/Makefile**

```
    make run_small_data_multidrug_pearson
```
* Results will match **data/verification/TEST_1_multidrug_results_pearson/** (when unzipped)

### The file **feature_prioritization_runtime_memory.xlsx** is a development tool for estimating memory in different environments
