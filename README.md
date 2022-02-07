# GenAP2 Galaxy implementation of CellRanger-ATAC
Disclaimer: This wrapper for CellRanger-ATAC is not developed or supported by 10x Genomics. This wrapper was written by scientists at GenAP to help facilitate usage of CellRanger tools inside of Galaxy.
Please find the full, official 10x Genomics licensing information at : https://support.10xgenomics.com/docs/license.

What is CellRanger ATAC?

https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/what-is-cell-ranger-atac

Naming convention of FASTQ files internally in Galaxy follows thes guidelines: 

https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/using/fastq-input#rightname

Installation:
1) Install this wrapper via the Galaxy toolshed.
2) CellRanger-ATAC (v2.0.0) is required for this wrapper and should be installed separately (see below). 

To use this tool, we assume that cellranger-atac (v.2.0.0) is available to Galaxy on the system, via the command cellranger-atac. Unfortunately at this point, we cannot include Cellranger-ATAC as part of this wrapper due to Licensing and distribution limitations. For more information on how to install CellRanger-ATAC on your system, please see :
https://support.10xgenomics.com/single-cell-atac/software/pipelines/latest/installation
