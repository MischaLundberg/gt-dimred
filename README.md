# gt-dimred
Genotype dimension reduction research

These are the core files used in the manuscript here: https://biorxiv.org/content/early/2018/09/23/423632

The pre-print has since been published at PLOS Genetics: https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1008432

If you want a simple Python script to carry out UMAP on your PC data, see https://github.com/diazale/gt-dimred/blob/master/scripts/general_umap_script.py

Most of the code is dedicated to data management and visualization.

PC data for the UKBB was provided to me so I didn't generate it myself.
PC data for the HRS (and HRS/1KGP data) was generated in PLINK. See `HRS_exploration.ipynb` and `HRS_1000G_exploration.ipynb` for details.
A demo version of work done on the 1KGP data can be found in another repo: https://github.com/diazale/1KGP_dimred

This HRS code is quite messy - this is because we worked with several subsets of the data and had to use proxies for ethnicities. While it works, it involves bouncing around different parts of it.

The UKBB code can be run in a straightforward manner provided you already have the data.


---

# Getting Started
In order to use these scripts to carry out `UMAP`, you should clone this repository via the commands
```  
git clone https://github.com/diazale/gt-dimred
cd gt-dimred
```

In order to install the Python dependencies, it is recommended to use the [Anaconda](https://store.continuum.io/cshop/anaconda/) Python distribution and package manager. After installing Anaconda, run the following commands to create an environment with UMAP's dependencies:

```
conda env create --file environment.yml
conda activate UMAP

## to deactivate the environment, type
#conda deactivate
```

In case you are updating your current version of the supported scripts, it would be best practice to also update your environment to the updated prerequisetes.
If you are using a Anaconda environment, you can do so by typing
```
conda env update --name UMAP --file environment.yml
```


If you receive any errors while running the supplied scipts, please ensure your versioning for the prerequisites is according to the tested versions.

