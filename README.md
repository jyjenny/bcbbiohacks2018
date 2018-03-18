# bcbbiohacks2018
sadcricket co. ltd.

Graph library: networkx
Community detection: girvan_newman
Community layout: networkx.spring_layout
Plotting the hills: 3d Gaussian
All plots: matplotlib.pyplot

PPI layer:
- layout of communities with spring, st that more connected communities are closer to each other
- Size of communities along x-y plane (i.e. sigma of Gaussian) proportional to number of genes in community
- FUTURE: mu of Gaussian in communities can be shifted according to centrality of nodes in the community
- FUTURE: Height of communities along z-axis should be inversely proportional to number of GO / number of genes; i.e. communities with many similar GO term mappings have higher peaks
    - So then expect thicker PPI-GO lines for higher peaks

GO layer:
- Each dot is a GO term, with colors for namespace:
    - Red = P
    - Blue = C
    - Yellow = F
- FUTURE: size of dots is number of proteins mapped to it
- FUTURE: GO terms are arranged according to tree hierarchy, so closer to centre of circle means it’s lower in the tree i.e. more specific; GO terms close to each other are closer in the tree

GWAS layer:
- Have a server ready, input a GWAS feature i.e. “diabetes-associated”
- FUTURE: highlight proteins (points on surface of the hills) with this GWAS feature, the community it belongs to, and the GO terms it maps to


~7-10 dimensions represented in a 3D space