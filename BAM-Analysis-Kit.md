BAM Analysis Kit is a bundle of genome tools that will analyse .BAM raw data file and outputs in file format similar to genetic genealogy companies. The goal of this kit to enable end users to analyse their own genome on their personal computer.

The tool provides the following output,
- genome_complete.txt.gz - Complete list from all confident sites
- genome_full_snps.txt.gz - Complete list of all known SNPs
- filtered-autosomal-o37-results.csv.gz - Filtered by Autosomal DNA SNPs tested by DNA companies
- filtered-x-chromosome-o37-results.csv.gz - Filtered by X DNA SNPs tested by DNA companies
- Admixture_Dodecad_Report.html - Dodecad dv3 Population Admixture Report
- Admixture_Eurogenes_Report.html - Eurogenes K=36 Population Admixture Report
- Admixture_Globe13_Report.html - Globe13 Population Admixture Report
- Complete_SNPs_y.csv - List of all identified Y-SNPs along with other columns
- ISOGG_Y_Haplogroup.txt - ISOGG Y-Haplogroup identification as on 1-Jul-2015
- MtDNA_Haplogroup.txt - Mt-DNA Haplogroup based on Build 15 (30 Sep 2012)
- MtDNA_Haplogroup_Report.html - Mt-DNA Haplogroup Report
- rCRS_mtDNA.txt - MtDNA mutations in rCRS format
- RSRS_mtDNA.txt - MtDNA mutations in RSRS format
- telomere.txt - Telomere length
- telseq.out - Telomere raw output file
- Variants_Y.txt - Y-DNA Novel Variants
- Y-STR_Markers.txt - Y-STR Markers
- Y_SNPs.txt - ISOGG Y-DNA SNPs
- bam_chr*.vcf.gz - VCF files if 'Delete VCF after processing' is unchecked.

**Prerequisites:**
- Windows 64 bit Operating System
- Microsoft .Net Framework 4.0
- 5 GB of free hard disk space.
- Minimum 2 GB RAM.

**Usage:**
Extract the download and click 'BAM Analysis Kit.exe'. Select the .BAM file and click 'Start Analysis'. After clicking 'Start Analysis', a command prompt will automatically open and start executing series of commands.

After a few minutes to several hours (or even days depending on your BAM file input and computer speed), the output will be available inside a subfolder called 'out'.

**Download:**  [BAM_Analysis_Kit.zip](https://drive.google.com/uc?id=0B_DZ5yg3R2FGcEd6TUUyVHI4dmc&export=download) (2 GB)

**Source Code:** located inside 'src' folder.

**Human Genome Reference:** The kit uses GRCh37.75 as reference. and uses snp142 for annotation of output genotype files.
- BOW (samtools) - GNU GPLv2
- Genome Analysis Tool Kit -  Non commercial License.
- lobSTR - GNU GPL v3
- telseq - GNU GPL v3
- bamtools - MIT License
- Cygwin - GNU GPL v3 

**References:**
- Li H., Handsaker B.*, Wysoker A., Fennell T., Ruan J., Homer N., Marth G., Abecasis G., Durbin R. and 1000 Genome Project Data Processing Subgroup (2009) The Sequence alignment/map (SAM) format and SAMtools. Bioinformatics, 25, 2078-9. [PMID: 19505943]
- McKenna A, Hanna M, Banks E, Sivachenko A, Cibulskis K, Kernytsky A, Garimella K, Altshuler D, Gabriel S, Daly M, DePristo MA (2010). The Genome Analysis Toolkit: a MapReduce framework for analyzing next-generation DNA sequencing data. Genome Res. 20:1297-303. [Pubmed]
- Ding, Zhihao, Massimo Mangino, Abraham Aviv, Tim Spector, and Richard Durbin. "Estimating telomere length from whole genome sequence data." Nucleic acids research (2014): gku181.
- Gymrek M, Golan D, Rosset S, & Erlich Y. lobSTR: A short tandem repeat profiler for personal genomes. Genome Research. 2012 April 22.
- SNPedia: a wiki supporting personal genome annotation, interpretation and analysis  Michael Cariaso; Greg Lennon Nucleic Acids Research 2011; doi: 10.1093/nar/gkr798
- van Oven M, Kayser M. 2009. Updated comprehensive phylogenetic tree of global human mitochondrial DNA variation. Hum Mutat 30(2):E386-E394. http://www.phylotree.org.  doi:10.1002/humu.20921 

*Change Log :1.8*
- Bug Fix - filtered-x-chromosome-o37-results.csv is empty due to typo fixed.

*Change Log :1.7*
- Bug Fix - Unable to load BAM from folders with spaces fixed.

*Change Log :1.6*
- Human Genome Upgraded to GRCh37.75
- SAMtools upgraded to 1.2
- lobSTR upgraded to 3.0.3
- SNPs upgraded to dbSNP 142
- GATK upgraded to 3.4
- Picard upgraded to 1.134
- Filters SNPs tested by DNA testing companies
- Provides mtDNA mutations in both RSRS and rCRS
- Identifies mtDNA and ISOGG Y haplogroup
- Reports Population Admixture using dv3, globe13 and eurogenes36.
- UI/Speed improvements
- Minor code change and bug fixes
- lobSTR used to calculate only Y-STR but CODIS processing removed.
- SNPedia report
- Download size and operational disk space significantly reduced.

*Change Log :1.5*
- Y-STR and CODIS supported for most BAM files.

*Change Log :1.4*
- Upgraded lobSTR to v3.0.2, GATK to v3.2.2
- Output includes more accurate Y-STR values.
- Includes CODIS output.
- Separated Y-STR and CODIS as optional.
- Displays used software version for convenience and advanced use.
- Adds Read Group tags for BAM files without them.

*Change Log :1.3*
- Updated with lobSTR from v2.0.4 to v2.0.8 (beta).
- Does not delete the VCF file after processing completes.

*Change Log :1.2*
- UCSC reference positions are zero based. This caused an offset of 1 position in output result - bug fixed.

*Change Log :1.1*
- Some files weren't created if mtDNA is not selected - bug fixed.

*Change Log :1.0*
- Works on all BAM files with build 37 positions
- Extracts SNPs from Autosomal DNA, X-DNA, Y-DNA and mtDNA.
- Provides mtDNA FASTA.
- Auto-converts Yoruba references in mtDNA and provides RSRS values.
- Provides Y-SNPs in ISOGG Nomenclature.
- Provides Y-STR markers.
- Calculates Telomere Length.*
