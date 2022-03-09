Results Analysis
-------------------

Performance on multiple models according to mutation-based structure information
*****************************************************************************************
To build a robust predicting protein stability changes model, dataset S1676 is used to train a model using 10-fold cross-validation. The results of our methods are replicated 10-fold cross-validation 20 times with shuffling the training data. Based on the availability of the PDB structure, we proposed four models SCpre-seq^str, SCpre-seq^seq, SCpre-seq and SCpre-seq^* to conduct comparative tests. When assuming that structures of wild-type and mutation proteins are unavailable for the training dataset, mutation-based structure features would get from G2S (SCpre-seq*).

** Table 1**. Performance of 10-Fold cross-validation on Dataset S1676

.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/Table1.png
  :align: center
  :width: 300px

.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/S1676bar.png
  :align: center
  :width: 300px


SCpre-seq achieves state-of-the-art performance on testing set S236
*****************************************************************************
.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/S236Picture2.png
  :align: center
  :width: 300px


**Figure S5**. Clustering results of scGNN compared to existing clustering tools.



SCpre-seq achieves state-of-the-art performance on testing sets S543
*****************************************************************************

.. image:: https://raw.githubusercontent.com/hurraygong/scGNN/master/pictures/S543Picture3.png
  :align: center
  :width: 300px



