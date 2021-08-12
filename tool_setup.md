# Setup for creating a Galaxy wrapper for Cellranger-ATAC with planemo

Make sure you have a working planemo installation. To find out how to install planemo, check here: https://planemo.readthedocs.io/en/latest/installation.html

## Generate galaxy tool xml using planemo tool_init

planemo tool_init --force \
  --id 'cellranger_atac' \
  --name 'Process 10x Genomics single-cell ATAC-seq data using CellRanger-ATAC.'\
  --example_command 'cellranger-atac count' \
  --cite_url 'https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/using/fastq-input#ATACIntro' \
  --help_from_command 'cellranger-atac'
  
  ## Test run with very small test data
  
   cellranger-atac count --id=sample345 \
                        --reference= \
                        --fastqs=/home/florian/GenAP2/test_datasets/cellranger_ATAC/atac_pbmc_500_nextgem_fastqs/100k_sub \
                        --sample=test \
                        --localcores=2 \
                        --localmem=6