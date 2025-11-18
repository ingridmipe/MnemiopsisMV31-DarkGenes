## Summary of what each column means in the final annotation file: 
--- 
- **`go_id`**: GO term ID.
- **`go_description`**: Description of the GO term.
- **`gene_ids`**: List of Gene_IDs that have that GO term.
- **`count_genes`**: Number of genes that have that GO term.
- **`category`**: GO category (BP, MF, CC).
- **`GeneRatio`**: Ratio of input genes that are annotated in a term (k/n).
- **`BgRatio`**: Ratio of all genes that are annotated in this term (M/N).
> #### I didn't calculate the following values, I wasn't sure if those are part of the enrichment analysis:   
>> - **pvalue**: Over-representation assessed using hypergeometric distribution (one-sided Fisher's exact test).
>> - **p.adjust**: Hypergeometric p-value after correction for multiple testing (BH adjusted p-values).
>> - **qvalue**: Another take on FDR adjusted p-values (Storey's method).
>> - ***`Count`***: Total number of genes from the input gene list that match the functional term **(I think this value match with the `count_genes` column).**

### Reference:
- https://bioinformatics.ccr.cancer.gov/docs/btep-coding-club/CC2023/FunctionalEnrich_clusterProfiler/