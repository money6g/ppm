ppm
===

Prediction by Partial Matching data compression algorithm minimal implementation (no GUI provided).

http://en.wikipedia.org/wiki/Prediction_by_partial_matching

Implemented by René Puchinger in 2007, revised in 2013.

**The algorithm itself may be patented, therefore only academic usage is recommended.**

Installation and Usage
----------------------

1. After cloning the Git repo, navigate to src/ folder.
2. To compile, run 
    
    g++ -o ppm *.cpp
	
3. Usage:

    ppm [c|d] input_file output_file
	
Example:

    ppm c book.txt book.ppm
    ppm d book.ppm book-orig.txt

Benchmark
---------

A sample book in text format is available in the test-data/ folder. The algorithm may process arbitrary data, though.

Compression results of several compression applications (default settings) for the file book.txt:

Original size: 1 344 739 bytes

Compressed by ZIP: 490 883 bytes
Compressed by 7-Zip: 386 768 bytes
Compressed by BZ2: 349 584 bytes
Compressed by **PPM**: 323 934 bytes
