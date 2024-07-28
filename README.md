# Illumina GSA3.0 A2 to 23me format convertor

This is a simple python notebook that explains how to convert from illumina global screenin array 3.0 final reports to 23me format. Since most online admixture calculators use older build 27 and 23me type data format this script should help with conversion.
This script does not use multiprocessing in batches so avg time of converting 600K snps will take roughly 4hrs.

The script does the following
1. Performs liftover from newer Build38 to Build37 genome build.
2. Removes genotype with low GT Scores
3. Performs illumina SNP to dbSNP based rsid converion

Note: My base is not bioinformatics, Incase of issues in conversion and improvements pull requests are welcome.
