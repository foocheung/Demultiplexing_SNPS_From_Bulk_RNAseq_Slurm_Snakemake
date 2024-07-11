## Demultiplexing_SNPS_SLURM


# Prepare Environment
conda env create -f environment.yml

conda activate snps
module load r-ggplot
module load r

# Submit job
sbatch sm_call

# Run Somalier
mkdir SOM
./run_somalier
