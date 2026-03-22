# Bottlenecks

This program finds edges in a network such that if the capacity of these edges increases so does the maximum flow. 

## Libraries used:

The script uses the networkx and matplotlib libray. Hence will need these to be installed. Run: 
- \pip instal networkx
- \pip instal matplotlib

## How to use:

- 2 Main functions Solve_single(Network,Source,Sink) and Solve_multi(Network,Source,Sink):
- Both have same input : network is a digraph in a networkx object examples of these are at the bottem of the python script, source and sink are nodes in the network.
- Solve_single(Network,Source,Sink) output : A list with 2 objects: 1st being set(original network max flow), 2nd being a set of single bottle neck edge with the increase upper bound, (to what value the capacities can improve the max flow).   
- Solve_multi(Network,Source,Sink) output : A list with 2 objects: 1st being the max flow of the origonal networks, 2nd being a list of sets containing edges (bottlenecks) and an intergral value (to what value the capacities can improve the max flow)

- Max_flow:
Input is Max_flow(Network,Source,Sink) returning 3 objects:

 [v max flow value , set of nodes (Network partition) , dictionary of the flow network]

 ## Once run:
Two Networks will appear, G and H, H being more complicated. These are found at the bottom and are examples of the different networks the solver will accept.
**!! When using Breaker or H nodes s and t are stored as strings 's' and 't'!! you must use the syntax Solve_multi(H,'s','t')** 

