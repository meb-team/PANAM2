PANAM2 is a pipeline for depicting the microbial community by implementing a phylogenetic approach for the annotation of the gene coding for 16S and 18S rRNA. It is based on PANAM (Taib et al. 2013) with some improvements and focusing on Illumina sequencing.
https://github.com/panammeb/PANAM2


**These script are part of the preprocessing of reads for the PANAM2 pipeline**

* To run these scripts you can put them next to the PANAM2 folder.

* Only the `Full_script_panam_HG.sh` script is needed to run for preprocessing. 

* An example of command line :

```
nohup bash Full_script_panam_HG.sh -w <BIN_FOLDER> -x <WORKING_DIRECTORY> -y <RAW_READS_FOLDER> -z <AMPLICONS_file.txt> &> nohup.preprocessing_panam.out &
```

* A conda env can be build using the Rpanam_env.yml (note: This environment is for preprocessing only at the moment)

	+ An example of conda command line to create the env : `conda env create -n Rpanam --file Rpanam_env.yml`
	+ Then, enter the environment : `conda activate Rpanam`