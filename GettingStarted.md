# Getting Started #
The file `ferrari.cpp` demonstrates how the FERRARI Index can be used. The respective executable `ferrari` can be used to run experiments with different configurations and data sets. The following table provides an overview over the possible command line parameters.

# Overview over Command Line Parameters #

| **Flag** | **Argument** | **Description** |
|:---------|:-------------|:----------------|
| `-g`     | 

&lt;FILENAME&gt;

 | file containing graph (directed, acyclic) |
| `-q`     | 

&lt;FILENAME&gt;

 | file containing queries |
| `-k`     | 

&lt;INTEGER&gt;

 | size constraint on the index (max. _nk_ intervals) |
| `-L`     | -            | use local space budget (per node) |
| `-G`     | -            | use global space budget |
| `-s`     | 

&lt;INTEGER&gt;

 | number of seeds to use for pruning |

# Example #
In order to run the reachability queries from the file `queries.q` for the index variant FERRARI-L on the graph specified in the file `arxiv.gr`, with a space restriction of at most 2 intervals per node as well as using 32 seed nodes for pruning, execute

```
# ./ferrari -g arxiv.gr -q queries.q -k 2 -s 32 -L
```