# HPC

# for sbatch

#!/bin/bash

#SBATCH --mail-user=liw17@nih.gov

#SBATCH --output=slurm_%j.out

#SBATCH --cpus-per-task=50

#SBATCH --mem=80g

#SBATCH --time=24:00:00


	module load R/3.4.3_gcc-4.9.1
	cd ~/Documents/Figure5/
	Rscript F5B220PCF2.R
	
