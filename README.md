# Factor Analysis and clustering of single-cell RNA-sequencing data derived from T cells 

This repository contains examples for analyzing scRNA-seq data derived from T cells. Four possible analysis parts are described including: 

- Data Preprocessing 
- Clustering and cell type identification of unstimulated (UNS) and stimulated cells 
- Application of different factor analysis methods

The code is available as jupyter notebook. Example output from preprocessing and clustering is shown in .html files. 

## Used data 
The data used for the analysis was originally obtained by [Cano-Gamez et al. how identified effectorness gradient of CD4+ T cells in response to cytokine stimuli](https://www.nature.com/articles/s41467-020-15543-y). 
The AnnData can be split into stimulated cells that were activated by anti-CD3 and CD28 beads, and unstimulated (UNS) T cells. To facilitate the cluster identification, the stimulated and unstimulated cells were analyzed separately. 

## Aim of the Project 
The [Cano-Gamez scRNA-seq data]( https://www.nature.com/articles/s41467-020-15543-y) was reanalyzed to further characterize the differentiation states of CD4+ T cells. As the identification of the diverse differentiation stages has turned out to be difficult, new ways for separating the cells had to be found. For this purpose, several factor analysis algorithms besides the standard method PCA were applied to the data including independent component analysis (ICA), Non­negative matrix factorization (NMF), Latent Dirichlet Allocation (LDA), and Linear Discriminant Analysis. 

## Provided Code 
The here available code is based on the standard procedures for preprocessing of scRNA-seq data (*Data_Preprocessing.ipynb*), and cell type annotation via clustering and marker genes (*Exploring_Cell-Types_in_UNS_data.ipynb*,  *Exploring_Cell_Types_in_stimulated_data.ipynb*). The *Factor_Analysis_Methods.ipynb* notebook provides the code to run the above-mentioned factor analysis methods. The resulting components can be used as input for cell type identification as shown in *Exploring_Cell-Types_in_UNS_data.ipynb* and *Exploring_Cell_Types_in_stimulated_data.ipynb*).

