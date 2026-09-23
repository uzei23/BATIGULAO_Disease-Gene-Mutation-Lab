 CELL AND MOLECULAR BIOLOGY LABORATORY
 From Gene Mutation to Disease
 Investigating How DNA Sequence Changes Affect Protein Products and Human Phenotypes

 Student Information

Name: Jehiah Bless Batigulao
Course: Cell and Molecular Biology Laboratory
Date of Analysis: September 2026

PART I. SELECT A HUMAN DISEASE AND GENE

Disease and Gene
Disease/Phenotype:Brugada syndrome 1
Gene: SCN5A
Gene Name: Sodium voltage-gated channel alpha subunit 5
Chromosomal Location: 3p22.2

Brugada syndrome is an inherited cardiac disorder associated with abnormal electrical activity of the heart. The SCN5A gene is one of the major genes associated with Brugada syndrome type 1.

PART II. RESEARCH THE DISEASE

 A. Disease

Brugada syndrome primarily affects the heart and cardiac electrical conduction system. It is characterized by abnormal ECG findings and an increased risk of ventricular arrhythmias and sudden cardiac death.

SCN5A-related Brugada syndrome is generally inherited in an autosomal dominant pattern. Pathogenic SCN5A variants commonly reduce the function of the cardiac sodium channel Nav1.5, resulting in decreased sodium current and abnormal cardiac conduction.

 B. Gene and Normal Protein

Gene: SCN5A
Protein: Nav1.5 cardiac voltage-gated sodium channel
Reference Protein: NP_000326.2

SCN5A encodes the alpha subunit of the cardiac voltage-gated sodium channel Nav1.5. The channel is located mainly in the plasma membrane of cardiac muscle cells.

Nav1.5 allows sodium ions to enter cardiac cells during depolarization. This sodium current contributes to the rapid upstroke of the cardiac action potential and the propagation of electrical impulses through the heart.

PART III. OBTAIN THE NORMAL REFERENCE SEQUENCE

The normal SCN5A reference sequence was obtained from the NCBI RefSeq database.
Reference Transcript: NM_000335.5
Reference Protein: NP_000326.2
Transcript: SCN5A transcript variant 2, mRNA
WT CDS Length: 6,012 bp
WT Protein Length: 2,003 amino acids

The coding sequence (CDS) was used for the sequence analysis because it contains the protein-coding region without introns and untranslated regions.


PART IV. IMPORT THE NORMAL SEQUENCE INTO GALAXY

The wild-type and mutant SCN5A sequences were analyzed using Galaxy to examine the effects of the documented mutation on the predicted protein sequence.
Galaxy History Name: `BATIGULAO_Brugada_syndrome_SCN5A_Mutation_Lab.`
Date of Analysis: September 2026

PART V. ESTABLISH THE WILD-TYPE CONTROL

The wild-type SCN5A sequence was established as the control for comparison.

| Parameter                | WT SCN5A                   |
| ------------------------ | -------------------------- |
| Gene                     | SCN5A                      |
| Phenotype                | Brugada syndrome           |
| Sequence Type            | Wild-type control          |
| Organism                 | *Homo sapiens*             |
| Transcript               | Transcript variant 2, mRNA |
| Sequence ID              | 210-6257_1                 |
| CDS Length               | 6,012 bp                   |
| Predicted Protein Length | 2,003 aa                   |
| Start Codon              | ATG                        |
| Stop Codon               | TGA                        |
| Reading Frame            | +1 / Frame 1               |
| First 10 aa              | MANFLLPRGT                 |
| Protein Accession        | NP_000326.2                |

The WT sequence was preserved as the original reference and was not directly modified.

PART VI. FORMULATE A MUTATION HYPOTHESIS

The documented mutation investigated in this experiment is:

SCN5A NM_000335.5:c.4296+1G>A

This is a single-nucleotide substitution at the +1 position of a splice-donor site.

Prediction
 Nucleotides affected: 1 nucleotide
 Change: G → A
 Mutation type: Splice-donor site substitution
 Direct reading-frame effect: No direct frameshift from the single-base substitution
 Predicted RNA effect: Abnormal RNA splicing
 Predicted protein effect: Possible altered, shortened, or reduced protein
 Predicted function: Reduced or abnormal Nav1.5 function

The hypothesis was that disruption of the splice-donor site could interfere with normal SCN5A RNA processing and ultimately affect the predicted protein product.


 PART VII. CREATE THE DOCUMENTED MUTANT SEQUENCE

The documented mutation was reproduced by changing the specified nucleotide from **G to A**.

Documented Variant: NM_000335.5:c.4296+1G>A
Original Base: G
Mutant Base: A
Bases Substituted: 1 bp
Mutation Type: Single-nucleotide substitution
The original WT sequence was kept unchanged, and a separate copy was used to create the mutant sequence.

PART VIII. TRANSLATE THE MUTANT SEQUENCE

The mutant sequence was translated in Galaxy and compared with the WT protein.
The computational results showed:

Mutant CDS Length: 6,048 bp
Mutant Protein Length: approximately 2,016 aa in the raw translated sequence
Reading Frame: +1 / Frame 1
First observed amino-acid difference: around position 1433 in the protein comparison
Observed amino-acid change: Y → V
Premature stop codons: Present
Downstream amino-acid changes: Extensive

The appearance of multiple downstream changes and premature stop codons indicates that the predicted mutant protein differs substantially from the WT sequence.

 PART IX. COMPARE WT AND MUTANT PROTEINS

The WT and mutant protein sequences were aligned and compared.
The sequences first showed a major difference around amino-acid position 1433. After this point, numerous downstream amino acids differed between the two sequences, and premature stop codons were observed in the mutant.
This indicates that the mutant sequence does not simply produce a single amino-acid substitution. Instead, the predicted downstream protein sequence is extensively altered.

PART X. EXPLAIN THE MOLECULAR CONSEQUENCE

The molecular mechanism is:

SCN5A c.4296+1G>A
→ disrupted splice-donor site
→ abnormal SCN5A RNA splicing
→ altered downstream coding sequence
→ premature termination/abnormal protein
→ reduced or abnormal Nav1.5 function
→ reduced cardiac sodium current
→ abnormal cardiac electrical conduction
→ Brugada syndrome phenotype

The computational protein comparison directly supports the presence of downstream sequence changes and premature stop codons.

However, the exact RNA-splicing pattern, protein expression, sodium current, and cardiac electrical effects require experimental evidence.


 PART XI. SECOND EXPERIMENT: CREATE AN ARTIFICIAL MUTATION

A separate controlled mutation experiment was performed using a single-nucleotide substitution.

Prediction Before Translation
One nucleotide within a codon was changed without adding or removing nucleotides.

Therefore:

Mutation type: Single-nucleotide substitution
Bases affected: 1
Reading frame: No change expected
Possible effect: Synonymous, missense, or nonsense
Protein length: Expected to remain unchanged unless a stop codon is created

The artificial mutant was then translated and compared with the WT sequence.


PART XII. COMPARE THE DOCUMENTED AND ARTIFICIAL MUTATIONS

The documented mutation and artificial mutation were compared based on their sequence and predicted protein effects.

The documented mutation affects a splice-donor site and may cause abnormal RNA processing and extensive downstream effects.

The artificial mutation is a single-nucleotide substitution within a codon. Because no nucleotide is added or removed, the reading frame is expected to remain unchanged.

The two mutations therefore demonstrate that the effect of a mutation depends not only on the number of nucleotides affected but also on its **exact location and biological role**.


 PART XIII. INTERPRETATION

The analysis demonstrated several important principles of molecular genetics:

1. The exact location of a mutation can determine its effect on RNA and protein.
2. Deleting three nucleotides can remove one amino acid without shifting the reading frame.
3. Deleting one or two nucleotides can cause a frameshift and alter many downstream amino acids.
4. Not every mutation changes the amino-acid sequence.
5. Not every amino-acid substitution destroys protein function.
6. A frameshift can change many downstream codons.
7. A premature stop codon can produce a shortened or nonfunctional protein.
8. Protein function can be affected even when protein length changes very little.
9. Mutations can cause disease by affecting RNA splicing or gene expression without directly changing the protein sequence.

The computational results support the predicted downstream protein changes and premature stop codons. Experimental studies are needed to confirm the actual molecular and cellular effects.




