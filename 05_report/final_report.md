# From Gene Mutation to Disease: Sequence Analysis of SCN5A in Brugada Syndrome

**Student:** Batigulao, Jehiah Bless T.  

**Course/Level:** BS Biology – Level 3  

**Instructor:** Prof. Abner Bucol  

**Disease/phenotype:** Brugada syndrome type 1  

**Gene:** SCN5A  

**Date of analysis:** September 2026  

**Galaxy history name:** BATIGULAO_Brugada_syndrome_SCN5A_Mutation_Lab.

##  Disease Background

Brugada syndrome is an inherited cardiac electrical disorder that can predispose affected individuals to ventricular arrhythmias and sudden cardiac death. The disorder is associated with characteristic electrocardiographic abnormalities, particularly ST-segment elevation in the right precordial leads, and may occur in individuals who otherwise appear structurally healthy. Clinical presentation can range from asymptomatic electrocardiographic findings to syncope, ventricular fibrillation, sudden cardiac arrest, sudden infant death syndrome, or sudden unexpected nocturnal death syndrome.

Brugada syndrome has a genetically heterogeneous basis. Pathogenic variants in **SCN5A** are an established cause of Brugada syndrome type 1. SCN5A-related disease is generally described as autosomal dominant, although penetrance and clinical expression can vary. The main affected organ is the heart, especially cardiomyocytes and the cardiac conduction system that generates and propagates electrical impulses [1, 3].

##  Gene and Normal Protein Function

The official gene symbol is **SCN5A**, which encodes the sodium voltage-gated channel alpha subunit 5. The gene is located on chromosome 3 at cytogenetic position **3p22.2**. The selected reference transcript was **NM_000335.5**, and the corresponding reference protein was **NP_000326.2** [2, 3].

The SCN5A gene encodes the alpha subunit of the cardiac voltage-gated sodium channel **Nav1.5**. Nav1.5 is an integral membrane protein located primarily in the plasma membrane of cardiac muscle cells. When the cardiac membrane depolarizes, Nav1.5 permits rapid sodium-ion influx. This inward sodium current produces the rapid upstroke of the cardiac action potential and supports propagation of electrical signals through the heart.

In this way, normal Nav1.5 activity is required for coordinated cardiac depolarization and conduction. A reduction or abnormality in Nav1.5 function can decrease cardiac sodium current, slow electrical conduction, and increase susceptibility to abnormal rhythms [1, 3].

##  Documented Mutation

The sequence-analysis portion of this laboratory exercise focused on the documented variant **SCN5A NM_000335.5:c.4296+1G>A**. This is a single-nucleotide G-to-A substitution at the +1 position of a splice-donor site. The +1 splice-donor position is important for recognition and removal of an intron during pre-mRNA processing.

| Feature | Documented variant |
|---|---|
| Disease/phenotype | Brugada syndrome |
| Gene | SCN5A |
| Reference transcript | NM_000335.5 |
| Nucleotide variant | c.4296+1G>A |
| Nucleotide change | G → A |
| Number of nucleotides changed | 1 bp |
| Variant type | Splice-donor-site single-nucleotide substitution |
| Supplied ClinVar record | VCV001739478.5 |
| Predicted effect | Abnormal SCN5A RNA splicing and reduced functional Nav1.5 |

The source laboratory record also contains an earlier documented-mutation table listing **c.481G>A, p.Glu161Lys (E161K)** and ClinVar accession **VCV000067927.19**. This is a different SCN5A variant from c.4296+1G>A. Because the mutant construction, translation, molecular mechanism, and conclusion analyze c.4296+1G>A, this report treats c.4296+1G>A as the primary analyzed variant. The variant identity should be confirmed with the instructor before final submission so that all repository files refer to one consistent mutation.

##  Hypothesis

The hypothesis was that the SCN5A c.4296+1G>A splice-donor substitution would disrupt normal RNA splicing. Abnormal splicing was expected to alter the downstream coding sequence, introduce premature stop codons, and produce either a truncated Nav1.5 protein or no stable protein because of nonsense-mediated decay.

The predicted biological consequence was loss or reduction of functional Nav1.5 channels. This would decrease cardiac sodium current, impair propagation of electrical impulses, and contribute to the conduction abnormalities and arrhythmia susceptibility associated with Brugada syndrome.

##  Methods

###  Reference-sequence preparation

The SCN5A reference transcript NM_000335.5 was obtained from the NCBI RefSeq record. The coding sequence was selected because it contains the protein-coding region without introns and untranslated regions. The WT CDS was saved as `SCN5A_WT_CDS.fasta`, and the translated reference protein was saved as `SCN5A_WT_protein.fasta` [2].

###  Wild-type translation

The WT CDS was imported into Galaxy and translated using the +1 reading frame. The resulting sequence was used as the WT control for the documented and artificial mutation experiments.

###  Documented mutation construction

A copy of the WT sequence was used so that the original reference was preserved. The nucleotide at the documented splice-donor position was changed from **G to A**, representing SCN5A c.4296+1G>A. The mutant CDS was saved and translated in the +1 reading frame.

###  Protein comparison

The WT and documented-mutant protein sequences were compared to identify the first amino-acid difference, downstream sequence changes, premature stop codons, and differences in apparent protein length. The alignment or comparison output was saved in the `04_results/` directory.

###  Artificial mutation experiment

A second sequence was created by changing the nucleotide at position 143 of the provided CDS from **A to T**. This changed the codon from **CGA** to **CGT**. Both codons encode arginine, allowing the effect of a synonymous nucleotide substitution to be examined.

##  Results

###  WT control results

| Parameter | WT result |
|---|---|
| Gene | SCN5A |
| Transcript | Transcript variant 2, mRNA |
| CDS length | 6,012 bp |
| Predicted protein length | 2,003 amino acids |
| Start codon | ATG |
| Stop codon | TGA |
| Reading frame | +1 / frame 1 |
| First 10 amino acids | MANFLLPRGT |
| Last 10 amino acids | DRESIV* |
| Protein identity | Expected SCN5A/Nav1.5 reference protein |

The WT sequence established the reference reading frame and protein product against which the mutant sequences were compared.

###  Documented-mutant translation results

The supplied mutant-sequence analysis reported a mutant CDS length of **6,048 bp** and a raw translated length of **2,016 amino acids**. The translated mutant contained a first amino-acid change from tyrosine to valine and premature stop codons. One translation summary placed the first difference at approximately position 1,373 and the first premature stop at position 1,374. The protein-comparison section placed the first difference at position 1,433.

| Parameter | Documented-mutant result |
|---|---|
| Mutant CDS length reported | 6,048 bp |
| Raw translated length reported | 2,016 aa |
| Reading frame | +1 / frame 1 |
| First amino-acid change reported in translation summary | Approximately position 1,373: Y → V |
| First amino-acid change reported in comparison summary | Position 1,433: Y → V |
| Premature stop codon | Present |
| Approximate downstream region affected | Approximately 644 amino acids |
| Overall result | Extensive downstream sequence alteration and premature termination |

The presence of multiple downstream amino-acid changes and premature stop codons is consistent with a major alteration of the coding sequence. However, these are computational translation results and do not prove the precise RNA-splicing product formed in vivo.

##  WT versus Mutant Protein Comparison

| Comparison question | Result | Biological meaning |
|---|---|---|
| Do WT and mutant proteins differ? | Yes | The mutant sequence diverges downstream of the affected region. |
| Is only one amino acid affected? | No | Multiple downstream residues are altered. |
| Are premature stop codons present? | Yes | Translation is predicted to terminate before the normal WT endpoint. |
| Is there a simple amino-acid deletion or insertion at the beginning? | No | The pattern is an extensive downstream alteration rather than a single local deletion or insertion. |
| Does the mutant retain a normal full-length protein product? | Not established | The raw sequence length does not show that a stable functional protein is produced. |
| Overall predicted consequence | Truncated, abnormal, or absent Nav1.5 protein | Functional SCN5A activity may be reduced. |

The mutant protein pattern supports the hypothesis that the splice-site variant has a substantial downstream consequence. A premature stop codon can remove important channel regions, while degradation of the abnormal transcript could prevent protein production entirely.

##  Artificial Mutation Experiment

The artificial mutation changed nucleotide **A to T** at position 143 of the provided CDS. The original codon **CGA** became **CGT**. Both codons encode arginine.

| Feature | Result |
|---|---|
| WT nucleotide | A |
| Mutant nucleotide | T |
| WT codon | CGA |
| Mutant codon | CGT |
| WT amino acid | Arginine (R) |
| Mutant amino acid | Arginine (R) |
| Protein-level classification | Synonymous/silent |
| Reading-frame change | None |
| Expected protein-length change | None |
| Direct amino-acid change | None |

This experiment demonstrates that not every nucleotide change alters the amino-acid sequence. Because the genetic code is degenerate, different codons can encode the same amino acid. The artificial mutation therefore has no direct predicted effect on protein structure based solely on the translated amino-acid sequence. Possible effects on splicing, mRNA stability, translation rate, or regulation were not tested.

##  Molecular Interpretation: Gene → Mutation → Protein → Cellular Effect → Phenotype

The proposed molecular pathway is:

**SCN5A gene**  
→ **c.4296+1G>A splice-donor substitution**  
→ **disrupted recognition of the splice donor**  
→ **abnormal SCN5A mRNA splicing**  
→ **altered downstream coding sequence and premature termination**  
→ **truncated, unstable, or absent Nav1.5 protein**  
→ **reduced cardiac sodium current**  
→ **abnormal cardiac depolarization and conduction**  
→ **ventricular arrhythmia susceptibility and Brugada syndrome phenotype**.

The sequence comparison supports the protein-level portion of this pathway because the supplied mutant translation contains downstream amino-acid changes and premature stop codons. The cellular and clinical portions are biologically plausible based on the known role of Nav1.5 in cardiac sodium-current generation and electrical conduction [1, 3].

The exact splicing pattern, transcript stability, amount of protein produced, membrane localization, and electrophysiological effect cannot be established from protein sequence comparison alone. These questions would require RNA analysis, protein-expression studies, channel-localization assays, and electrophysiological measurements.

##  Limitations

1. **Variant inconsistency in the supplied record.** The draft lists both c.481G>A/p.Glu161Lys and c.4296+1G>A. These variants must not be presented as the same mutation. This report uses c.4296+1G>A because it is the variant used in the sequence-construction and molecular-mechanism sections.

2. **Conflicting amino-acid coordinates.** The first mutant difference is reported as approximately position 1,373 in one section and position 1,433 in another. The final repository should use the coordinate from the finalized alignment or translation output.

3. **Raw mutant length is not equivalent to functional protein length.** A raw translated sequence of 2,016 amino acids does not demonstrate that a normal 2,016-amino-acid protein is produced when premature stop codons are present.

4. **Splicing was not measured experimentally.** The analysis predicts abnormal splicing but does not directly examine SCN5A RNA.

5. **Protein expression was not measured.** The experiment does not determine whether a truncated protein is produced, degraded, or transported to the membrane.

6. **Electrophysiology was not performed.** The effect on sodium current, action potentials, and cardiac conduction was inferred from known channel biology rather than measured in cells.

7. **Clinical risk cannot be predicted for an individual from this sequence exercise alone.** Disease expression depends on genetic background, penetrance, age, environmental factors, and other clinical variables.

##  Conclusion

This laboratory investigation demonstrates how the location and molecular context of a nucleotide change influence its biological consequence. The documented SCN5A c.4296+1G>A variant affects a splice-donor site and is predicted to disrupt RNA processing. In the supplied computational representation, the mutant sequence shows extensive downstream amino-acid changes and premature stop codons, supporting a possible loss-of-function mechanism for Nav1.5.

Reduced or abnormal Nav1.5 activity can decrease cardiac sodium current and impair the propagation of electrical impulses through the heart. This provides a molecular explanation connecting the SCN5A variant to abnormal cardiac conduction and the Brugada syndrome phenotype. In contrast, the artificial A143T substitution changes the nucleotide sequence from A to T but preserves arginine because CGA and CGT encode the same amino acid. It therefore illustrates a synonymous mutation with no direct amino-acid change.

The overall relationship demonstrated by the experiment is:

**gene → nucleotide variant → RNA processing → protein product → cardiac sodium current → electrical conduction → phenotype**.

The computational findings provide a sequence-based prediction. Confirmation of the complete mechanism would require experimental RNA-splicing, protein-expression, channel-localization, and electrophysiological studies.

##  References

1. El Sayed, M., Goyal, A., & Callahan, A. L. (2023). *Brugada Syndrome*. StatPearls/NCBI Bookshelf. https://www.ncbi.nlm.nih.gov/books/NBK519568/

2. NCBI RefSeq. *Homo sapiens sodium voltage-gated channel alpha subunit 5 (SCN5A), transcript variant 2*. NM_000335.5. https://www.ncbi.nlm.nih.gov/nuccore/NM_000335.5

3. NCBI Gene. *SCN5A sodium voltage-gated channel alpha subunit 5 [Homo sapiens]*. Gene ID 6331. https://www.ncbi.nlm.nih.gov/gene/6331

4. NCBI ClinVar. Variant record supplied for *SCN5A* NM_000335.5:c.4296+1G>A. VCV001739478.5. https://www.ncbi.nlm.nih.gov/clinvar/variation/1739478/
