# Shortest Paths in CW-Complexes
GAP algorithms for calculating shortest paths in regular CW-complexes

## Description: 

A variety of algorithms using Dijkstra's shortest path procedure for use with the HAP
package (Homology, Algorithms & Groups) for GAP.

1. **ShortestPathInGraph** Inputs a list of edges in a graph, a set of weights to be added to these edges
and the initial and terminal vertices in the desired path. The output is the length of the shortest path
and the edge-path.

2. **ShortestPathInRegularCWComplex** Inputs some regular CW-complex and the values of the initial
and terminal vertices in its 1-skeleton. The ouptut is the length of the shortest
path between the given points as well as the path itself.

3. **ShortestPathInUniversalCover** The input is a regular CW-complex as well as its fundamental
group, a vertex and a group element. The algorithm calculates the shortest path in the homotopy
class of loops corresponding to that group element in the universal cover.

## Requirements

Written using the GAP system for computer algebra (https://www.gap-system.org/)   
with the HAP package (http://hamilton.nuigalway.ie/Hap/www/index.html)

## Usage

Regular CW-complexes will have to be of the data type specified in HAP.
The fundamental group of such complexes (Y) can be computed with the following command:

gap> G:= FundamentalGroupOfRegularCWComplex(Y,"nosimplify");
