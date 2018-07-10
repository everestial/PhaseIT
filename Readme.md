This is a pipeline for haplotype phasing. This pipeline incorporates 2 major tools with several other subsidiary tools.

The general data analyses workflow for haplotype phasing is:
  - Step 01 - A) ReadBackPhasing of called variants (VCF) against aligned BAM reads to create phased haplotype blocks. This step uses tools **phaseRB** or **HapCut2**.
  - Step 01 - B) Conversion of RBphased haplotype blocks to HAPLOTYPE file.
  - Step 02 - A) General purpose haplotype phaseExtension using phaseExtender.
  - Step 02 - B) Haplotype phase extension in F1 hybrids or trio using phaseStitcher.
  - Step 03) Conversion of phased haplotype to VCF using VCF-Simplify.
  
Note: All these pipelines are complete and functioning. I need some more time to put all those tools under one hood of phaseIT.
If you are already interest in using the tools, go ahead and let me know if you have any questions.

Q/A: What kind of genome is this tools targeted to?
   Haplotype phasing has been a core part of genetics and genomics science since traditional allele sequencing began. Exiisting haplotype phasing 
   tools are mostly geared towards organsism that have lots of genotype data available. Unfortunately, emerging model system have not been
   very fortunate to exploit the confidence in phasing due to lack of required high volume genotype data from lots of individuals - which include
   reference panels, phased data from highly inbred lines.
   Readbackphasing provides a very first step in providing more clean approach to phasing because adjacent heterozygous variants can be phased with
   same aligned reads that the variants were called from. While sequenc readds are getting larger which definitely helps us produce larger phased haplotype 
   blocks; these haplotype are still broken due to low coverage issues, or even with the high coverage reads from certain genomic regions can be missing 
   due to pure random process.
   PhaseIT takes haplotype phasing to next level by utilizing these phased haplotype blocks from sevveral samples and aims to join two haplotypes by 
   looking at the LD pattern between two blocks of a sample across other sample that might bridge those breakpoints. Since, we are now not dealing with LD 
   between two blocks (with several SNP positions) rather than SNPs at just two position the haplotype phase confidence are highly elevated and 
   error largely reduced. This is due to fact that when joining two phased blocks there are only two possible configuration rathern than 
   traditional 2^n. Plus the already phased haplotype strings provide strong computational confidence about the predicted phase state.
   I also show that RBphasing reduce switherror significantly with only few samples in hand by running phaseExtension in human genome NA....
   
phaseIT is largely suitable for emerging model system that have reference genome but do not have large number of genotyped individuals. Plus, phaseIT
provides the benefit of running controlled and recursive phaseExtension, there by providing a chance to improve and regularly check the phase quality checks.
Additionally, it reduces the traditional burden of preparing an inbred line.

<br>
   
### To be continued .......
.............................

