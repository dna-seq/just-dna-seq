Working With Annotation Information
===================================

After applying the necessary filters, click the **Variant** tab.

You will see a view with a table in the upper part and widgets below. You can move the border between them or switch to another view using the button in the upper right corner of the window:

View table - switch to table-only view
View detail pane - switch to widgets-only view
View table - switch to the default view (both)

For our purposes we'll need the table first of all.

The table contains columns and column sets with general info about the filtered variants, as well as connected to certain annotators. Some logically grouped column sets (by a particular annotator) can be extended or collapsed by clicking the +/- sign in the upper right corner of the column set (the topmost row). If you filtered by particular annotators, especially using "has data" condition, for other annotators it may show nothing for that particular variants, and they can be collapsed for convenience.

Each row of the table represents a variant that you can research.

Variant Annotation
------------------

UID - the variant number in this (filtered) sequence

Chrom - chromosome where the variant is located. Chromosome names are ‘chr1’ to ‘chr22’, ‘chrX’, ‘chrY’ and ‘chrM’.

Position - Chromosomal position of the variant. THe first position in each chromosome is position 1.

Ref Base - Reference allele at this chromosomal position (one of A,C,G,T, and N).

Alt Base - Alternative allele; called based on reads mapping to this chromosomal position.

Note -

Coding -

Gene -

Transcript -

RefSeq -

Sequence Ontology -

cDNA change -

Protein Change -

All Mappings -

Sample Count -

Samples -

Tags -


CADD Exome
----------

Score -

Phred -


CardioBoost
-----------


Cardiovascular Disease Knowledge Portal
---------------------------------------


ClinPred
--------


ClinVar
-------

Clinical Significance -

Disease Ref Nums -

Disease Names -

Review Status -

ClinVar ID -

Significance Detail -


dbSNP
-----

rsID - Database identifier („rs“ number) of this variant in dbSNP.

This column is empty if the observed variant is not described in dbSNP. Such
variants can be extremely rare variants or technical artifacts.


Extra VCF INFO Annotations
--------------------------

Gencode Gene Mapper
-------------------


gnomAD Gene
-----------


GWAS Catalog
------------


NCBI Gene
---------


OMIM
----


Original Input
--------------


PharmGKB
--------


PubMed
------


REVEL
-----


SIFT
----


VCF Info
--------

Phred -

VCF Filter -

Zygosity - Most likely zygosity of the variant this chromosomal position, computed from the
observed variant frequency (column 8) and can be “FP/HET” (<15%), “HET” (15-
75%), “HET/HOM” (75-85%), or “HOM” (>85%).

Alternate reads - Number of reads showing the alternative allele.

Total reads - Total number of reads.

Variant AF -

Haplotype block ID -

Haplotype strand ID -
