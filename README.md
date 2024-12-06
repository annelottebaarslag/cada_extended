# cada_extended
We extend the CADA algorithm with Label Propagation and Walktrap and experiment with different graphs with varying node size, mu, maximum degree, power law exponent for the degree distribution and power law exponent for the community size distribution

## Setting up
Start by downloading the needed libraries by running the first cell and then import the needed libraries by running the same cell.

## Defining CADA
The fourth cell builds the CADA class from the original paper [1], with our addition of Walktrap and Label Propagation.

## Building an LFR
The fifth cell defines the function for generating the synthetic network using LFR.

## Adding anomalies
The sixth cell is the function inject_random_anomalies() which injects random anomalies to the graph. This could be expanded or changed, for example by also adding replaced anomalies.

## Calculating the mean F1 score
The seventh cell is the function for calculating the mean F1 score over 5 graphs with a different seed. This function could be changed by using another metric than F1 or taking the std instead of the mean.

## Experimenting with different networks
Starting from the eighth cell, the different parameters are used to create different graphs, apply cada and plot the results for the different algorithms. You can run the cells from the parameters that you want to vary and define which algorithms you want to use. You can also choose which values you want to use for the parameters. It is recommended to save the results in .npy files for future use. It is explained in the text in the notebook what actions are done in the different cells.


[1] Helling, T.J., Scholtes, J.C., Takes, F.W. (2019). A Community-Aware Approach for Identifying Node Anomalies in Complex Networks. In: Aiello, L., Cherifi, C., Cherifi, H., Lambiotte, R., Lió, P., Rocha, L. (eds) Complex Networks and Their Applications VII. COMPLEX NETWORKS 2018. Studies in Computational Intelligence, vol 812. Springer, Cham. https://doi.org/10.1007/978-3-030-05411-3_20
