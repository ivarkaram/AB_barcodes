# AB_barcodes
## Code to generate antibody barcodes (AB) compatible with Visium Spatial Transcriptomics.

To allow for multiplexed protein profiling with DNA-conjugated antibodies using the Visium spatial gene expression solution from 10x genomics, AB barcodes that are not overlapping with the spatial barcodes needs to be generated to distinguish these 2 sets of barcodes.

Here code has been generated for that purpose, specifically:
* n randomly generated barcodes of l length (here 100 barcodes of 16 nucleotide length)
* Hamming distance of at least 6 from any AB barcode to any Visium spatial barcode
* Hamming distance of at least 7 from any AB barcode to any other AB barcode
* GC content within the same range as the Visium spatial barcodes (25%-75%)
* No more than 3 consequtive bases for any AB barcode

## Dependencies
* Python 3.8.5
* Numpy 1.19.2

Other versions of Python and Numpy may also work
