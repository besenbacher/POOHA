# POOHA
POOHA: Parent Of Origin Haplotype Annotator ---
Assign parent of origin to heterozygous variants in a child using read-backed phasing


## Installation
To run the POOHA python script you need to have to have python3 with the pysam and pyvcf libraries installed. This can be installed using conda by creating a new environment using the environment.yml file:
```
conda env create -f environment.yml
```
To activate this new environment, use:
```
conda activate pooha
```

## Usage
You can see the options of the POOHA program using the -h option:
```
./POOHA -h
```
To identify all new mutations in a parent-offspring trio and assign parental origin to as many of them as possible run:
```
./POOHA {vcf_file} {father} {mother} {child} {child_bam_file}
```
Where {fater} {mother} and {child} should be the names given to those individuals in the vcf-file header.

