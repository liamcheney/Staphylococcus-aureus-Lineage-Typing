# Staphylococcus-aureus-Lineage-Typing

The <i>Staphylococcus</i> aurues Lineage Typer (SaLTy) was developed for the high-level classification of <i>S. aureus</i> WGS data.

SALTy rapidly divides the species into 60 phylogenetically well-defined lineages. The lineages were resolved through single linkage clustering of 10,000 core genome MLST (cgMLST) profiles from a core genome consisting of 1,724 genes. Lineages differed by at least 1,017 cgMLST alleles. Alleles of three core genes were identified that can uniquely define the 60 lineages. SALTy was validated on 5,000 genomes and 99.3% (4,966/5,000) of the isolates were assigned to the correct lineage.


GENERAL:
  -t THREADS, --threads THREADS
                        Number of threads (speeds up parsing raw reads).
  -f, --force           Overwite existing output folder.
  --report              Only generate summary report from previous SALTy
                        outputs.

INPUT:
  -i GENOME_FOLDER, --genome_folder GENOME_FOLDER
                        Input folder with assembled DNA sequence file.
  -r READS_FOLDER, --reads_folder READS_FOLDER
                        Folder with forward and reverse raw reads (fastq.gz)

OUTPUT:
  -o OUTPUT_FOLDER, --output_folder OUTPUT_FOLDER
                        Output Folder to save result.
  -csv, --format_csv    Output file in csv format.
  -s, --summary         Concatenate all output assignments into single file.

DB PATHS:
  -l LINEAGES, --lineages LINEAGES
                        Path to specific alleles for each lineage.
  -k KMA_INDEX, --kma_index KMA_INDEX
                        Path to indexed KMA database.
