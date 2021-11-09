# process

This is data from human embryonic stem cells. The accession number is PRJNA631808.

The website is as follows: https://www.ncbi.nlm.nih.gov/sra/SRX8327390[accn].



1. At first, I use scanpy for gene processing. The genetic information comes from the results of CellRanger.

   1. top 20 gene

      ![image-20211102020009276](https://tva1.sinaimg.cn/large/008i3skNly1gw06uhtsvej30v80u0mzs.jpg)

2. Then, I took steps such as filtering and standardization.

   ![image-20211102020306162](https://tva1.sinaimg.cn/large/008i3skNly1gw06xj6t8uj32ee0rck6r.jpg)

3. I use the graph-based clustering algorithm Leiden to cluster.Only the gene information was used.

   1. Leiden result

   ![image-20211102020425240](https://tva1.sinaimg.cn/large/008i3skNly1gw06yw48thj30ws0u0djw.jpg)

   2. Marker gene

      ![image-20211102021552275](https://tva1.sinaimg.cn/large/008i3skNly1gw07at3iz8j31kn0u0q7u.jpg)

4. I chose the cell with the largest cluster 0( in blue color ), Use the transposable element expression obtained by my own tool to cluster the 0 cluster again. I found that cluster 0 was clearly divided into two.

   ![image-20211102020835085](https://tva1.sinaimg.cn/large/008i3skNly1gw07387scpj30wo0u0q9m.jpg)

5. I re-projected the te clustering results onto the original gene UMAP.

   ![image-20211102021023203](https://tva1.sinaimg.cn/large/008i3skNly1gw07540f6nj30y50u0gox.jpg)

6. Marker **te** between two clusters.

   ![image-20211102021126448](https://tva1.sinaimg.cn/large/008i3skNly1gw0767z3rzj31gv0u0djf.jpg)

7. Marker gene between two clusters.

   1. 0 vs 1

      ![image-20211102021241834](https://tva1.sinaimg.cn/large/008i3skNly1gw077i9ae6j30u00ur40f.jpg)

   2. 1 vs 0

      ![image-20211102021308575](https://tva1.sinaimg.cn/large/008i3skNly1gw077z0y64j30u00uv0uk.jpg)

   3. 0,1 vs rest

      ![image-20211102021503799](https://tva1.sinaimg.cn/large/008i3skNly1gw079yrfo5j31h00u0dj8.jpg)

8. I used other resolution to cluster by expresion of gene, but the result of te clustering can not be obtained.

   ![image-20211102021818082](https://tva1.sinaimg.cn/large/008i3skNly1gw07dcf7sij30xu0u00wu.jpg)

I wanna know the meaning of two clusters split by te expresion. Thank you!