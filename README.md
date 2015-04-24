

Dependencies
============

Python packages
---------------

* numpy
* scipy
* matplotlib
* h5py
* pp (Parallel Processing)
* Biopython
* pymongo
* mirnylib (https://bitbucket.org/mirnylab/mirnylib)
* networkx

Other software
--------------

* bowtie2

How to use
==========

* Make sure you have read/write/execute permission on the main folder and all its subfolders.
* Run main.py
* Choose output folder
* Load a fasta genome
* Build bowtie index (bowtie path must be specified in the advanced options or a bowtie folder must be in the main folder)
* Load fastq paired-end read files
* Load restriction enzyme (or manually type in the site sequence)
* Check advanced parameters and tweak if needed
* Align and wait for *ready for computation* terminal output (this may take a while)
* Click on **Pyramid** to proceed to the visualizer (visualizer may also be directly summoned by running main_window.py)
* Load data and browse to the inside of a folder named *analysis* within the output folder
* Build pyramid (this may take a while) and load it
* Visualize using options as needed

Advanced
========

Visualizer options
------------------

* When building a pyramid, the *sparsity filter* will remove bins whose total contact count is too low. 
* Saturation threshold can be either absolute (fixed number), relative (percentile, append % at the end) or auto-adjusted depending on the needed rendering.
* Matrices can be manually loaded "raw" (from a text file) and binned, but no genome information will be displayed.
* "Kb binning" will regroup bins such that the total length of each bin is closest to 10kb.
* The norm called *sparsity* is an alias for fragment-wise order 1 normalization.
