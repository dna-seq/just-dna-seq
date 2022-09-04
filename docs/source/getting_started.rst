Getting Started
===============

OakVar vs OpenCravat
--------------------

Both OpenCravat and OakVar can be used to annotate a human genome. However, as OakVar is based on OpenCravat and contains more advanced features customized specially for personal longevity genomics, it is recommended to use OakVar, and this documentation is based on it.

* **NOTE:** *An older OpenCravat-based version of documentation (in progress) could be found here: https://just-dna-seq.readthedocs.io/en/master/*

Installing OakVar
----------------------------

Instructions how to install OakVar could be found in the OakVar documentation: https://oakvar.readthedocs.io/en/latest/

Uploading Your Genome
---------------------

1. Open OakVar in your browser. You will see the index page:

.. image:: index.png
  :alt: Index page

2. In the **Variants** section you should choose the right assembly version of the **Genome:** hg38/GRCh38, hg19/GRCh37, or hg18/GRCh36.

For example we'll take a small VCF file of the hg19/GRCh37 version named example.vcf.

3. Click **Add input files**. A file upload dialog will open, allowing to browse and select the vcf file (or multiple files at once).

After loading the file(s) it will show next to the **Add input files** button along with another button **Clear file(s)** and a small **X** button next to each file name. If you click that **X**, the appropriate file will be deleted. If you click **Clear file(s)**, all the files you loaded will be deleted.

.. image:: vcf-loaded.png
  :alt: vcf files loaded
  
4. Scroll the left area down to the **Annotations** section.

Here you can select categories of annotators (above) and checkboxes for particular annotators. Let's select the **ClinVar** annotator from the **Clinical Relevance** category:

.. image:: select-annotations.png
  :alt: Selecting annotators
  
**Note:** An annotator may belong to multiple categories at once.

The checkbox and **X** buttons between the categories and the annotators sections allow to select all of the displayed annotator chechboxes or to clear all of them.

If you right-click any annotator, a pop-up window with its description will open in the right area:

.. image:: annotation-description.png
  :alt: Annotator description
  
5. When you select all the annotators you need, click the large **ANNOTATE** button below in the left area.

Annotating a large genome file may take some time. While loading, it will appear in the right area on the top of the list, displaying different stages of the processing in the **Status** column, and when finished, the **Open Results Viewer** button will appear in that column of the particular genome row:

.. image:: genome-annotated.png
  :alt: Genome annotated
  
Now click the **Open Results Viewer** button, and the annotated genome will open in a new browser tab/window.
