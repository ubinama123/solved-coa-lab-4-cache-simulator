Download Link: https://assignmentchef.com/product/solved-coa-lab-4-cache-simulator
<br>
Cache performance is important for system performance. In this lab, you are asked to simulate cache behaviors by C/C++ style cache simulators. By this training, you would understand the performance difference between different cache architectures.

2. Basic Problem

You should trace the memory addresses in your single cycle CPU in lab 3. The supplied files are described as follows:

<h2>           a. “lab4_test_data.txt” –</h2>

The file is a 3-dimensional matrix multiplication program, which is the input of your CPU. You can find the explanation of the code in “lab4_test_data_assembly.pdf”.

<h2>           b. “Instruction_Memory.v” –</h2>

We enlarge the instruction file from the previous lab so that it can fit the input size of “lab4_test_data.txt”.

<h2>           c. “TestBench.v” –</h2>

A verilog testbench, please refer to it and then modify your CPU to get the memory traces when the program is running (make sure the registers or wires in your CPU is named correctly so that it can be correctly called by “TestBench.v”). After running the program, you will get two output files, “ICACHE.txt” and “DCACHE.txt”. These two files are the simply the memory traces of ICACHE (instruction cache) and DCACHE (data cache) respectively.

<h2>           d. “direct_mapped_cache.cpp” –</h2>

A simple cache simulator. You should modify this simulator so that it can output the miss rate of the cache. (Hint: see pdf of chapter 5 in page 4.) Please take the file “ICACHE.txt” and “DCACHE.txt” that are produced by the CPU, as inputs of the simulator and then run it. First, change the parameters (cache size or block size) when you do the simulation. Then draw a graph as the following example and describe the reason of rise and fall of the lines in the report. (Please separate ICACHE from DCACHE)




<h1>3. Advanced Problem</h1>

LRU stands for Least-Recently Used, which is a replacement policy of choosing the one unused for the longest time. In this problem, you have to implement an n-way set-associative cache simulator using LRU (by C/C++, refer to the supplied file “direct_mapped_cache.cpp”). Please name this new simulator as “direct_mapped_cache_lru.cpp”. Set block size = 64 bytes. Then input the file “LU.txt” and “RADIX.txt” that are the memory trace from two benchmarks to the simulator. Please draw a graph as the following example and describe the reason of rise and fall of the lines in the report. (Please separate the discussion of LU and RADIX). Also, please compute the total bits (including tags and one valid bit) required for each cache, and show them by table (like following table) or plot the figure.

<h1></h1>