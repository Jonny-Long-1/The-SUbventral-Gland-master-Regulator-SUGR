# The-SUbventral-Gland-master-Regulator-SUGR

# Network creation
## Programs used
R 4.2.2

Gephi 0.10

## OS
Windows 11

## 2 class Network creation workflow
Network creation was carried out as described in (Molloy et al., 2024).

CSV files containing the expression profiles of the 8 transcription factors identied in the "extract up" cluster and the putative effectors identified by (Molloy et al., 2024) were loaded into 2_class_network_creator.R, and the corresponding output files loaded into 2_class_gefx_creator.R. The resulting gefx file was opened in Gephi 0.10, and the fruchterman reingold area applied with an area of 100,000. 

The network splitter 3d package was then used to split the network (https://gephi.org/plugins/#/plugin/network-splitter-3d). Degree was calculated for each node in Gephi; TFs were given a [z] value equal to their degree; and effectors were given a [z] value of 0. 

The following paramaters were then used to split the network:

Z-Maximum Level: 50 (equal to the largest [z] in the network)

Z-Distance Factor: 10

Z-Scale: 100

Alfa: 80
