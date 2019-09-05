# Digenic

#### Get summary statistics on the digenic hits in a case/control population.
#### Authors: Joseph Hostyk, Gundula Povysil
#### Overview:
Traditional collapsing searches for QVs (qualifying variants - variants that pass certain filters) in every gene. Here, we explore the digenic model:	searching for QGPs (qualifying gene pairs - two genes in both of which a sample	has a QV).

We first calculate how many total QGPs there are in the dataset. Because that list is pretty large, we demonstrate thresholds necessary to get that amount down to a manageable number. A collapsing matrix marks how many QVs each sample has in each gene.
Our file format is a tab-separated file with sample names as column headers and gene names as row headers.

Usage:<br>
<pre>
digenic.py &lt;matrixFilePath> &lt;geneListFilePath>
</pre>

Options:<br>
<pre>matrixFilePath    &emsp;&emsp;&emsp;&emsp;&emsp; Path to the gzipped matrix.
geneListFilePath   	Path to file with each gene on a new line.
-h --help           &emsp;&emsp;&emsp;&emsp;Show these options.
