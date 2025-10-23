Installation (pyG framework)
============

Software Dependencies
---------------------
.. code-block:: python

​​python​​: 3.8.0 
​​torch​​: 1.8.1+cu111 
​​cudnn​​: 9.1.0.70 
​​numpy​​: 1.22.4 
​​scanpy​​: 1.9.8 
​​anndata​​: 0.9.2 
​​rpy2​​: 3.5.12 
​​pandas​​: 2.0.3 
​​scipy​​: 1.10.1 
​​scikit-learn​​: 1.3.2

Installation
------------

Download the S3RL code from GitHub: https://github.com/AI4Bread/stCAMBL, clone the repository with the following command:

.. code-block:: bash

   git clone git@github.com:AI4Bread/stCAMBL.git
   cd stCAMBL

Then, create a new conda environment and install the required packages:

.. code-block:: bash
   conda create -n stCAMBL python=3.8.0 
   conda activate stCAMBL
   pip install -r requirements.txt


.. note::

The code is tested with Python 3.8.0 and PyTorch 1.8.1+cu111 on a single NVIDIA GeForce RTX 3090 GPU.
If you encounter any issues, please check the compatibility of the packages in requirements.txt with your Python version.
Additionally, different versions of libraries and different GPU devices may lead to varied outcomes,
so to reproduce our results, please use the same versions and hardware configuration as specified.

Dataset Directory Structure

Download the datasets and place them in the Data directory, ensuring the directory structure appears as follows:

.. code-block:: text

   stCAMBL
   ├── Data
   │   ├── DLPFC
   │   │   ├── 151673
   │   │   ├── 151674
   │   ├── Nanostring
   │   ├── Human_Breast_Cancer
   │   ├── Mouse_Brain_Anterior

Processed datasets can be downloaded from the following links:

- `DLPFC <https://github.com/LieberInstitute/spatialLIBD?tab=readme-ov-file#raw-data>`__
- `Nanostring <https://purdue0-my.sharepoint.com/personal/tang385_purdue_edu/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Ftang385%5Fpurdue%5Fedu%2FDocuments%2FSigra%5Fdataset&ga=1>`__
- `Human Breast Cancer <https://www.10xgenomics.com/resources/datasets/human-breast-cancer-block-a-section-1-1-standard-1-1-0>`__
- `Mouse Brain Anterior <https://drive.google.com/drive/folders/1jDmx8IjiGhOD__spuuhFB1fWVDJtv5CU>`__
- `Human Lung Cancer <https://drive.google.com/drive/folders/14ZHjGeyyVUnYn_0EqpHmNVo1V1F5B1Hx>`__
- `Mouse Hippocampus Starmap <https://drive.google.com/drive/folders/14ZHjGeyyVUnYn_0EqpHmNVo1V1F5B1Hx>`__
- `Soybean <https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE270392>`__

