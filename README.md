# The Set Orienteering Problem

This document is an attachment of the papers:

1.	_C. Archetti, F. Carrabs, R. Cerulli_, [The Set Orienteering Problem](https://www.sciencedirect.com/science/article/pii/S0377221717310202), European Journal of Operational Research, Volume 267(1), pp. 264 - 272, 2018. 

2.	_Francesco Carrabs_, [A Biased Random-Key Genetic Algorithm for the Set Orienteering Problem](https://www.sciencedirect.com/science/article/pii/S037722172031002X), European Journal of Operational Research, Volume 292(3), pp. 830-854, 2021.  

3.	_F. Laureana, C. Archetti, F. Carrabs, and R. Cerulli_, A New Formulation and a Branch-and-Cut Algorithm for the Set Orienteering Problem, Submitted.

We document the file format of the instances used in these papers. Files can be downloaded at http://www.dipmat2.unisa.it/people/carrabs/www/DataSet/InstancesSOP.zip 
or
https://github.com/fcarrabs/Set_Orienteering_Problem/upload/main

*** Instances *** 

Instances are obtained by adapting instances for the Generalized Traveling Salesman Problem (GTSP) proposed in: 
“M. Fischetti, J. J. Salazar Gonzalez, P. Toth, A branch-and-cut algorithm for the symmetric generalized traveling salesman problem, Operations Research 45 (3) (1997) 378–394”. 
In particular, among all these instances, we select the instances for which the distance is defined as the Euclidean distance between customers’ coordinates. These instances have a number of vertices ranging from 52 to 1084 and a number of clusters equal to ∼ 20% of the number of vertices. They are 51 in total (see the paper for more details about the generation of the instances).

Files are organized as follows. 

			-  The depot is node 1. This node is the only one inside the cluster zero.		
			-  File name is structured as follows:  <TSP-instance-name>T<percentage of best/optimal GTSP solution>p<#kind of generation of profits>.sop

A second set of instances has the abbreviation “RND” inside the name. In this set the vertices are randomly assigned to the clusters.

			-  File format follows TSPLIB format with an additional GTSP_SET_SECTION: One line for each cluster of customers: 
				<cluster_id> <cluster_profit> list:<customer_id>

*** Detailed Results *** 
	
The detailed results of the algorithms introduced in the papers above can be downloaded from the following link:
http://www.dipmat2.unisa.it/people/carrabs/www/DataSet/SOP_BRKGA_DetailedResults.xlsx

or from

https://github.com/fcarrabs/Set_Orienteering_Problem/tree/main/Results

