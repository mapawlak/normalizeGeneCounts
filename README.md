# normalizeGeneCounts

## Description
Function takes raw counts of NGS data and normalize to [CPM, RPKM or TPM](https://www.rna-seqblog.com/rpkm-fpkm-and-tpm-clearly-explained/).

## Usage
normalizeGeneCounts(counts, TxDb, method)

## Arguments

*counts*  A data frame with gene ID in rownames and sample ID in colnames

*TxDb*    `GenomicFeatures` object created from the same gtf as counts object

*method*  Should be "CPM", "RPKM" or "TPM"

## Example
```
CPM <- normalizeCounts(counts, TxDb, method = "CPM")
```
