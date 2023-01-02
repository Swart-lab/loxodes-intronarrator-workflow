Empirical intron annotation for Loxodes magnus genome assembly
==============================================================

Snakemake pipeline to empirically annotate introns and produce an artificial
"intronless" genome sequence with
[Intronarrator](https://github.com/Swart-lab/Intronarrator) for downstream gene
prediction.

Data
----

Genome assembly is available from the European Nucleotide Archive under
accession [PRJEB55123](https://www.ebi.ac.uk/ena/browser/view/PRJEB55123);
RNA-seq data under accession
[PRJEB55324](https://www.ebi.ac.uk/ena/browser/view/PRJEB55324).

Pipeline and scripts to generate the genome assembly and RNA-seq mapping are
available from
[loxodes-assembly-workflow](https://github.com/Swart-lab/loxodes-assembly-workflow)
repository.

The same pipeline was used for annotation of the MAC and MIC genomes; path to
reference assembly and names of output files were modified accordingly.

Paths to input files in the `workflow/config.yaml` file are local paths used in
the original data analysis. When re-running the pipeline, replace these with
the actual paths on your system.

Curated output from this annotation are included in the [archive of genome
annotations](https://doi.org/10.17617/3.9QTROS).

Running workflow
----------------

To run on a local server, use `./run_snakemake.sh` script, and add rule names
and additional parameters, e.g. `./run_snakemake.sh --dryrun`.

