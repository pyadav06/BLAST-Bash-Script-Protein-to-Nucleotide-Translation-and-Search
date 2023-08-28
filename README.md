# BLAST-Bash-Script-Protein-to-Nucleotide-Translation-and-Search
This script performs a sequence similarity search using BLAST by translating a protein query file into a nucleotide query file and then searching it against a nucleotide sequence database. BLAST (Basic Local Alignment Search Tool) is a powerful tool for comparing biological sequences, such as proteins and nucleotides, to identify similarities and potential functional annotations.

**Prerequisites:**
Before using this script, make sure you have the following:

BLAST Executables: You should have the BLAST+ executables (e.g., blastp, blastx) installed on your system. You can download BLAST from the NCBI website.

Protein Query File: A file containing protein sequences in FASTA format that you want to search against the nucleotide database.

Nucleotide Database: A nucleotide sequence database in FASTA format against which you want to search for similarities.

**Usage:**
Place the protein query file (protein_query.fasta) and the nucleotide database file (nucleotide_db.fasta) in the same directory as this script.

Open a terminal and navigate to the directory containing the script.

Run the script using the following command:

```bash
bash blast_script.sh


The script will perform the following steps:

a. Translate the protein query file into a nucleotide query file using transeq from the EMBOSS suite. The translated sequences will be saved in a file called nucleotide_query.fasta.

b. Use BLAST to search the translated nucleotide query sequences against the nucleotide database. The BLAST results will be saved in a file called blast.tsv.

**Customization:**

BLAST Parameters: You can modify the BLAST parameters in the script to suit your specific needs, such as changing the E-value threshold, alignment scoring parameters, and more. Refer to the BLAST documentation for details.

Output Format: By default, the script outputs BLAST results in a human-readable format. You can change the output format using BLAST command-line options like -outfmt.


