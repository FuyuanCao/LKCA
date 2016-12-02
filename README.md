#LKCA: A library of k-modes-type clustering algorithms

For the numerical data, methods of cluster analysis have been well-explored. As the categorical data lack of the inherent
geometric properties, the distance between objects cannot be defined naturally.
Therefore, the corresponding clustering model and its algorithm design
differentiate from that of the numerical data. In recent years, the problem of
clustering categorical data has attracted more attention. 

LKCA is a software toolbox for clustering
algorithms. It provides the open-source package for use in R that implements
the k-modes-type clustering algorithms for categorical data. The library is
designed to facilitate the development of the new algorithms in this direction
and make comparisons between the new methods and existing ones available. LKCA is
available from https://github.com/FuyuanCao/LKCA. The
LKCA library comes with a detailed documentation. The documentation downloaded
from https://github.com/FuyuanCao/LKCA/tree/master/manual
describes the setup and usage of the LKCA. All the functions and related data
are explained in detail.

The LKCA architecture is composed of four
modules, that is, the k-modes algorithm, the fuzzy k-modes algorithm, the
SV-k-modes algorithm and the fuzzy SV-k-modes algorithm. The four modules in
the LKCA architecture are designed independently, and all codes follow the R
standards.

In each module, LKCA provides three patterns
to cluster categorical data, including single-threaded, multi-threaded and
distributed computation. In the multi-threaded operation, it is provided with
multiple CPU to execute multiple threads at the same time, which equivalently
creates a set of functions running in parallel. Through the multi-thread
operation, it will improve the overall processing performance. In addition, by
using distributed computing technology, the task will be decomposed into a
number of small parts, and assigned to multiple computers for processing, which
can save the overall computing time, and greatly improve the computational
efficiency.

The implementation of the clustering algorithms depends on these sub functions, including the distance function,
finding cluster centers function, and initial cluster center selection function.


