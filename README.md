This is the repository for all data collected our in study and published in:

Sinder, S. B., Diaz, I. C., Patel, S. H., Romagnoli, J., Sharma, H., Perez, G. G., Dave, K. R., Perez-Pinzon, M. A., Bramlett, H. M., & Raval, A. P. (2026). Electronic cigarette vapor exposure modifies stroke-induced transcriptional and microglial responses in a sex-dependent manner. Neurochemistry international, 197, 106185. https://doi.org/10.1016/j.neuint.2026.106185

-----------------------------------------------------------
 American Heart Association
README file

General information
9/29/2026

1.	PI’s name: Dr. Ami P. Raval; Department of Neurology, University of Miami Miller School of Medicine, Miami, Florida, USA.

2.	PI’s ORCiD ID: 0000-0003-1757-9947 

3.	Association award number: 23TPA1142407

4.	Association award doi: https://doi.org/10.58275/AHA.23TPA1142407.pc.gr.172288

5.	Association award title: Impact of electronic cigarette vaping on stroke outcomes in animals of both sexes

6.	Date range of data collection: 
2/01/2021 to 2/01/2026

7.	List of up to six key words to describe data topic:
 
a.	Electronic cigarettes 
b.	ischemic stroke 
c.	microglia 
d.	sex differences 
e.	RNA sequencing
f.	neuroinflammation 

8.	Other: Corresponding author: Ami P. Raval, ARaval@med.miami.edu. Additional support: VA I01BX006223-01A1 (MPIs Raval and Bramlett), Florida Department of Health 25K06 (Raval), and an endowment from Drs. Chantal and Peritz Scheinberg










Data and file overview
1.	For each file name, a short description of what data it contains:

ALL DATA (EC Microglia paper).xlsb: Excel binary workbook containing the data dictionary, animal IDs, processed RNA-seq results, histological measurements, microglial morphometry, and Sholl measurements. 

README.md / this README: Study context, funding, file organization, access information, and methods.

RNA-seq table structure: Rows identify genes. Columns contain sample-level expression values, group summaries, log2FoldChange, pvalue, padj, and gene annotations. These are processed analysis tables, not raw sequencing reads.

2.	Other: The data dictionary is included within the excel workbook. The actual workbook extension is .xlsb; references to .xlsx should be corrected unless a separate .xlsx export is deposited. Raw sequencing reads and original microscopy images are not contained in this workbook.

Sharing and access information
1.	Licenses on data (The Association recommends CC-0 + attribution or CC-BY 4.0): CC BY-NC-ND

2.	Licenses on source code: N/A

3.	Links to other data deposits/repository links: https://github.com/spatel41-umiami/Raval-lab-EC-microglia-study

4.	Recommended citation for the data: Sinder, S. B., et al. (2026). Data for “Electronic cigarette vapor exposure modifies stroke-induced transcriptional and microglial responses in a sex-dependent manner” [Data set]. Raval Lab. https://github.com/spatel41-umiami/Raval-lab-EC-microglia-study. 

Methodological information
1.	Description of model:
a.	Animal: Rattus norvegicus, Sprague-Dawley rats
b.	Sex: Both (Female + Male) 
c.	Sample size: The animal list includes 32 RNA-seq animals (4/group across 8 groups), 12 females for RT-qPCR (6/group for Air + tMCAO and EC + tMCAO), and 48 histology animals (6/group across 8 groups). Eight RT-qPCR animals overlap with the RNA-seq list, and four are additional females. Analysis-specific n may be lower after exclusions; see the figure data and Supplemental Table 3 of the publication.
d.	Age: ~3 months
e.	Disease state: Experimental focal cerebral ischemia induced by 90-minute transient middle cerebral artery occlusion (tMCAO), with sham controls
f.	Interventions: Air or electronic cigarette vapor exposure using 5% nicotine Virginia tobacco JUUL pods for 16 consecutive nights before surgery. Sham animals received anesthesia for the same duration as the tMCAO procedure.
g.	Comparisons: Within each sex: Air + Sham, EC + Sham, Air + tMCAO, and EC + tMCAO, ie eight experimental groups overall. RNA-seq tables in the excel workbook compare EC with air separately by sex and surgical condition.


2.	Description of methods for data collection (may include links or references to publications or other documents): 
Exposure and surgery: The EcigAero Aerosol Exposure Apparatus (AutoMate Scientific) delivered 16 vapor episodes over 8 hours nightly. Each 8-minute episode alternated 2 seconds of vapor with 8 seconds of air, followed by 22 minutes of air. The reported flow was 3.2–4 L/min at 3.0 V. After the final exposure, rats underwent tMCAO or sham procedures. Cerebral blood flow was monitored before occlusion, immediately after occlusion, and at reperfusion.
RNA-seq and RT-qPCR: Novogene performed RNA quality control, poly(A) mRNA enrichment, library preparation, Illumina NovaSeq 6000 sequencing (150-bp paired-end reads), and bioinformatics analysis of ipsilateral cortex. For RT-qPCR, RNA extraction and quality assessment were followed by reverse transcription and SYBR Green detection on a Bio-Rad CFX Opus 96. Primers are listed in Supplemental Table 1.
Histology and microscopy: Brains collected at 21 DPI were perfusion-fixed with 4% paraformaldehyde, paraffin-embedded, and sectioned at 10 µm. NeuN, GFAP, and Iba1 immunostaining used DAB detection. Stereological estimates used an Olympus microscope and the optical fractionator probe in StereoInvestigator. Counting frames were 50 × 50 µm for neurons/astrocytes and 100 × 100 µm for microglia. Microglial images were acquired with a 60× oil-immersion objective (NA 1.2) from matched cortical regions, including ipsilateral peri-infarct tissue. The published sampling scheme included three sections, nine images per hemisphere, and at least 54 microglia per rat across both hemispheres.

3.	Description of methods used for processing data (how were data processed from raw data to analyzed data):
Transcriptomics: Novogene generated expression estimates, differential-expression statistics, and functional enrichment results. The paper describes FPKM-based expression analysis, log2 fold-change thresholds >1 or <−1, and p-value/FDR-adjusted q-value thresholds of 0.05. Preserve the distinction between unadjusted pvalue and adjusted padj values in the deposited tables. The precise analysis settings and gene lists should be used when reproducing individual figures.
Histology and morphology: ImageJ was used for two-dimensional measurements of soma/cell area, perimeter, and branch length. For Sholl analysis, neighboring processes were removed, images were converted to binary, and concentric circles were centered on the soma. Published radii ranged from 10 to 900 µm in 5-µm steps.
Statistics and quality control: Animals were randomized to exposure, with surgical failure as the a priori exclusion criterion; experimenters were blinded to exposure during acquisition and analysis. Data were presented as mean ± SD. The paper reports ordinary one-way ANOVA with Tukey comparisons for histological, morphometric, and Sholl outcomes. RT-qPCR used relative expression (2−ΔΔCq), ROUT outlier removal (Q = 5%), and unpaired two-tailed Student’s t-tests comparing Air + tMCAO with EC + tMCAO.

4.	Software: Microsoft Excel or compatible .xlsb-reading software opens the workbook. Reported analysis software: GraphPad Prism 9; R 4.1.1 in RStudio; ImageJ with Sholl Analysis Plugin v1.0; StereoInvestigator; and the Erogulu-Lab/Ion-Vitro-Sholl R code cited in the paper. Instruments include EcigAero, Illumina NovaSeq 6000, Bio-Rad CFX Opus 96, NanoDrop, Agilent BioAnalyzer, and Olympus microscopy.
<img width="468" height="407" alt="image" src="https://github.com/user-attachments/assets/aa57c602-99cd-4896-9010-56956eccf56c" />
