# Demultiplexing SNPS From Bulk RNAseq Using Slurm and SnakeMake


## Prepare Environment
- conda env create -f environment.yml

- conda activate snps
- module load r-ggplot
- module load r

## Submit job
- sbatch sm_call

## Run Somalier
- mkdir SOM
- ./run_somalier

## Ancestry
- ./somalier ancestry --labels ancestry-labels-1kg.tsv 1kg-somalier/*.somalier ++ SOM/*.somalier

## Relate
- ./somalier relate SOM/*.somalier
