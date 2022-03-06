Results Analysis
-------------------

SCpre-seq
^^^^^^^^^^^^^^^^

Performance on multiple models according to mutation-based structure information
*******************************




SCpre-seq achieves state-of-the-art performance on testing sets S543
********************************






SCpre-seq achieves state-of-the-art performance on testing set S236
********************************



scGNN showed significant enhancement in cell clustering compared to the clustering tool (e.g., Seurat) when using the raw data. The comparison was conducted on four tools (i.e., Seurat, CIDR, RaceID, and Monocle3) using four benchmark datasets. ARI of each test is indicated on each UMAP, comparing the predicted cell clusters to the benchmark labels.

.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/FigureS5.png

**Figure S5**. Clustering results of scGNN compared to existing clustering tools.

scGNN illustrates AD-related neural development and the underlying regulatory mechanism
****************************************************************************************


.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/F5.large.jpg

**Figure 5** Alzheimer’s disease dataset (GSE138852) analysis based on scGNN. (A) Cell clustering UMAP. Labeled with scGNN clusters (left) and AD/control samples (right). (B) Comparison of cell proportions in AD/control samples (left) and each cluster (right). (C) Heatmap of DEGs (logFC > 0.25) in each cluster. Six oligodendrocyte sub-clusters are merged as one to compare with other cell types. Marker genes identified in DEGs are listed on the right. (D) Selected AD-related enrichment pathways in each cell type in the comparison between AD and control cells. (E) Underlying TFs are responsible for the cell-type-specific gene regulations identified by IRIS3.

.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/FigureS6.png

**Figure S6**. Comparison of DEG expression before (Left) and after scGNN imputation (Right). DEGs were identified using the Seurat package based on scGNN predicted clusters, and the six oligodendrocyte sub-clusters were merged into one. Cells were randomly selected from half of the merged oligo group to make the figure more balanced.
