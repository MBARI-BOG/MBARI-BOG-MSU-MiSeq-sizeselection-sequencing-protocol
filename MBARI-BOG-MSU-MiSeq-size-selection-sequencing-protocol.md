---
# MIOP terms
methodology_category: Omics Analysis
project: Marine Biodiversity Observation Network (MBON)
purpose: biodiversity assessment objective [OBI:0001969]
analyses: PCR [OBI:0000415], Amplicon Sequencing [NCIT:C204813]
geographic_location: Monterey Bay [GAZ:00002509]
broad_scale_environmental_context: marine biome [ENVO:00000447]
local_environmental_context: upwelling [ENVO:01000005]
environmental_medium: sea water [ENVO:00002149]
target: 12S [NCIT:C128263]
creator: Jacoby Baker, Kobun Truelove, Kathleen Pitz
materials_required: Illumina MiSeq [OBI:0002003], PCR instrument [OBI:0000989], agarose gel electrophoresis system [OBI:0001134], Blue Pippin or Pippin HT
skills_required: sterile technique, pipetting skills, standard molecular technique
time_required: # minutes (integer)
personnel_required: 1
language: en
issued: # YYYY-MM-DD
audience: scientists
publisher: Monterey Bay Aquarium Research Institute (MBARI)
hasVersion: 1
license: CC0 1.0 Universal
maturity level: mature

# FAIRe terms
## pcr
pcr_primer_forward: AATGATACGGCGACCACCGAGATCT-[i5-BC(index 2)]-ACACTGACGACATGGTTCTACA
pcr_primer_reverse: CAAGCAGAAGACGGCATACGAGAT-[i7-BC(index 1)]-TACGGTAGCAGAGACTTGGTCT
pcr_primer_name_forward: PE1-BC-CS1
pcr_primer_name_reverse: PE2-BC-CS2
pcr_primer_reference_forward: # 10.1111/1462-2920.13023
pcr_primer_reference_reverse: # 10.1111/1462-2920.13023
pcr_primer_vol_forward: # 1.0
pcr_primer_vol_reverse: # 1.0
pcr_primer_conc_forward: # 10
pcr_primer_conc_reverse: # 10


## library preparation sequencing
barcoding_pcr_appr: two-step PCR
pcr2_thermocycler: # The manufacturer and model of a thermocycler used in the second step PCR
pcr2_amplificationReactionVolume: 15
pcr2_commercial_mm: 2.5X HotMaster Mix
pcr2_custom_mm: # not applicable
pcr2_dna_vol: 1
pcr2_cond: initial denaturation:95_3;denaturation:95_0.25;annealing:60_0.5;elongation:72_1;final elongation:72_3;15
pcr2_annealingTemp: 60
pcr2_cycles: 15
pcr2_analysis_software: # The program used to analyse the PCR runs  in the second step PCR
pcr2_method_additional: # Additional information on PCR or PCR-free method, that has not been shared in the given record in the second step PCR
sequencing_location: Michigan State University RTSF Genomics core
platform: Illumina
instrument: Illumina MiSeq [OBI:0002003]
seq_kit: # The name of sequencing kit
lib_layout: paired end
adapter_forward: AATGATACGGCGACCACCGAGATCT
adapter_reverse: CAAGCAGAAGACGGCATACGAGAT
lib_screen: The library was size selected using a Blue Pippin or Pippin HT (Sage Science, Beverly, USA)
lib_conc: # The concentration of the prepared library pool that was loaded onto the sequencing platform for a sequencing run.
lib_conc_unit: # ng/µL | nM | pM
lib_conc_meth: # Qubit Fluorometer
phix_perc: 20
mid_forward: # Forward multiplex Identifiers (MIDs), that was used to specifically tag unique samples in a sequencing run. Sequence should be reported in uppercase letters
mid_reverse: # Reverse multiplex Identifiers (MIDs), that was used to specifically tag unique samples in a sequencing run. Sequence should be reported in uppercase letters
checksum_method: # The specific algorithm or technique used to compute the checksum (checksum_filename, checksum_filename2) for verifying data integrity. Examples include MD5, SHA-256, and CRC-32.
seq_method_additional: # Additional information on library preparation and sequencing method, that has not been shared in the given record.

---

# Michigan State University (MSU) Illumina MiSeq sequencing with size selection protocol

## PROTOCOL INFORMATION

### Minimum Information about an Omics Protocol (MIOP)

- MIOP terms are listed in the YAML frontmatter of this page.
- See [MIOP_definition.md](https://github.com/BeBOP-OBON/0_protocol_collection_template/blob/main/MIOP_definition.md) for list and definitions.

### Making eDNA FAIR (FAIRe)

- FAIRe terms are listed in the YAML frontmatter of this page.
- See <https://fair-edna.github.io/download.html> for the FAIRe checklist and more information.
- See <https://fair-edna.github.io/guidelines.html#missing-values> for guidelines on missing values that can be used for missing FAIRe or MIOP terms.

### Authors

- All authors known to have contributed to the preparation of this protocol, including those who filled in the template.
- Visit https://orcid.org/ to register for an ORCID.
- Date is the date the author first worked on the protocol.

| PREPARED BY  | AFFILIATION  | ORCID        | DATE       |
| ------------ | ------------ | ------------ | ---------- |
| Jacoby Baker | MBARI | 0000-0002-0673-7535 | 2025-11-25 |
| N. Kobun Truelove | MBARI | 0000-0002-2236-1849 | 2025-11-25 |
| Kathleen J. Pitz | MBARI | 0000-0002-4931-8592 | 2025-11-25 |

### Related Protocols

- This section contains protocols that should be known to users of this protocol.
- Include the link to each protocol.
- Include the version number and release date (if available).
- Internal/External: "Internal" are derivative or altered protocols, or other protocols in this workflow. "External" are protcols from manufacturers or other groups.

| PROTOCOL NAME | LINK         | VERSION      | RELEASE DATE | INTERNAL/EXTERNAL |
| ------------- | ------------ | ------------ | ------------ | ----------------- |
| Environmental DNA (eDNA) 12S Metabarcoding PCR Protocol (with Platinum SuperFi II Taq) V.3  |  [https://github.com/MBARI-BOG/MBARI-BOG-12S-superfiII-metabarcoding-pcr-protocol/blob/main/MBARI-BOG-12S-superfiII-metabarcoding-pcr-protocol.md](https://github.com/MBARI-BOG/MBARI-BOG-12S-superfiII-metabarcoding-pcr-protocol/blob/main/MBARI-BOG-12S-superfiII-metabarcoding-pcr-protocol.md) | 3.0 | yyyy-mm-dd   | Internal      |
| Content Cell  | Content Cell | Content Cell | yyyy-mm-dd   | Content Cell      |

### Protocol Revision Record

- Version numbers start at 1.0.0 when the protocol is first completed and will increase when changes that impact the outcome of the procedure are made (patches: 1.0.1; minor changes: 1.1.0; major changes: 2.0.0).
- Release date is the date when a given protocol version was finalised.
- Description of revisions includes a brief description of what was changed relative to the previous version.

| VERSION | RELEASE DATE | DESCRIPTION OF REVISIONS |
| ------------- | ------------- | ------------- |
| 1.0.0 | 2025-11-25 | Initial release |

### Acronyms and Abbreviations

| ACRONYM / ABBREVIATION | DEFINITION |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

### Glossary

| SPECIALISED TERM | DEFINITION |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

## BACKGROUND

### Summary

This protocol covers the processing steps following initial PCR for secondary amplification, library preperation, size selection and sequencing. This protocol is performed by Michigan State University (MSU) Research Technology Support Facility (RTSF) Genomics Core ([https://rtsf.natsci.msu.edu/genomics/](https://rtsf.natsci.msu.edu/genomics/)).


This work was supported by NASA grant NNX14AP62A ‘National Marine Sanctuaries as Sentinel Sites for a Demonstration Marine Biodiversity Observation Network (MBON)’ funded under the National Ocean Partnership Program (NOPP RFP NOAA-NOS-IOOS-2014-2003803 in partnership between NOAA, BOEM, and NASA), and the U.S. Integrated Ocean Observing System (IOOS) Program Office.



### Method Description and Rationale

This protocol follows on the two-step amplification strategy using Fluidigm adapters CS1 & CS2 (see related PCR protocol above).


### Spatial Coverage and Environment(s) of Relevance

This protocol has been used to sequence extracted DNA from filtered sea water samples taken from marine coastal stations off the western coast of North America (primarily off of California).

- ocean [ENVO:00000015]

## PERSONNEL REQUIRED

1 technician

### Safety

>Identify hazards associated with the procedure and specify protective equipment and safety training required to safely execute the procedure

### Training Requirements

Sterile technique, pipetting skills.

### Time Needed to Execute the Procedure

Average time for MSU to process samples depends on sequencing queue, but generally takes around two months from sample shipment to receiving data back.

## EQUIPMENT

- Opentrons Consumables: If using Opentrons OT-2 Robot for KF Plate Prep.
- Description: E.g., "filter".
- Product Name and Model: Provide the official name of the product.
- Manufacturer: Provide the name of the manufacturer of the product.
- Quantity: Provide quantities necessary for one application of the standard operating procedure (e.g., number of filters).
- Remark: For example, some of the consumable may need to be sterilized, some commercial solution may need to be diluted or shielded from light during the operating procedure.

| DESCRIPTION | PRODUCT NAME AND MODEL | MANUFACTURER | QUANTITY | REMARK |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| **Durable equipment** |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |
| **Consumable equipment** |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |
| **Chemicals** |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell | Content Cell | Content Cell |

## STANDARD OPERATING PROCEDURE


### Preparation

>not applicable


### Secondary Amplification

1. Secondary amplification and NGS were performed at Michigan State University's Research Technology Support Facility (RTSF).
    An aliquot of 20 μL from each purified primary PCR product was sent to RTSF Genomics Core at MSU for secondary PCR amplification with primers which targeted the CS1/CS2 ends of the primary PCR products and added dual indexed, Illumina compatible adapters with barcodes. 
 - PE1-BC-CS1 (forward): `AATGATACGGCGACCACCGAGATCT-[i5-BC(index 2)]-ACACTGACGACATGGTTCTACA`
 - PE2-BC-CS2 (reverse): `CAAGCAGAAGACGGCATACGAGAT-[i7-BC(index 1)]-TACGGTAGCAGAGACTTGGTCT`

 
2. The secondary PCR amplifications were carried out in 15 μL reactions, using 1 μL of primary PCR product.
 - 6 μl 2.5X HotMaster Mix
 - 7 μl DI water
 - 1 μl Primer Mix (6uM)
 - 1 μl primary eDNA PCR product

3. Secondary 12S cycling parameters:

 ```
 95°C 3 minutes
 15 cycles of the following three steps:
 - 95°C 15 seconds
 - 60°C 30 seconds
 - 72°C 1 minute
 72°C 3 minutes
 25°C Hold
 ```
 
4. An agarose gel was run after secondary PCR to confirm the presence of target bands and absence of non-specific amplification across environmental samples as well as the absence of amplification in NTCs.
5. After secondary PCR, products were run through Invitrogen SequalPrep Normalization Plate (ThermoFisher Scientific) using manufacturer's protocol to create pooled library.
6. The library pools were QC’d and quantified using a combination of Qubit dsDNA HS, Agilent 4200 TapeStation HS DNA1000 and Invitrogen Collibri Library Quantification qPCR assays.


**Primers**: Secondary PCR primer sequences

| PCR Primer Name | Direction | Sequence (5’ -> 3’)|
| ----- | ----- | ----- |
| PE1-BC-CS1 | forward | AATGATACGGCGACCACCGAGATCT-[i5-BC(index 2)]-ACACTGACGACATGGTTCTACA |
| PE2-BC-CS2 | reverse | CAAGCAGAAGACGGCATACGAGAT-[i7-BC(index 1)]-TACGGTAGCAGAGACTTGGTCT |



**Reaction Mixture**: PCR reagents, volumes, initial and final concentrations

| Reagent | Volume | Initial Concentration | final concentration|
| ----- | ----- | ----- | ----- |
| primary PCR product | 1 μl | N/A |N/A |
| 2.5X HotMaster Mix | 6 μl | content |content |
| Primer Mix | 1 μl | 6 μM |content |
| DI water | 7 μl | N/A |N/A |

**PCR Cycling Program**: 

| PCR Step | Temperature | Duration | Repetition |
| ----- | ----- | ----- | ----- |
| Intial Denaturation | 95° C | 3 minutes | 1 |
| Denaturation | 95° C | 15 seconds | 15x |
| Annealing | 60° C | 30 seconds | 15x |
| Extension | 72° C | 1 minute | 15x |
| Final Extension | 72° C | 3 minutes | 1 |
| Hold | 25° C | ∞ |  |

### Size selection of final library

1. After the pooled library was QC'd, the library was size selected with either a Blue Pippin or Pippin HT to select for the vertebrate/fish band (~350 bp) and remove the co-amplified bacterial band (~435 bp).
2. After size selection, the pooled library was QC'd again to confirm selection of the correct band and new amplicon concentrations.

### Sequencing

1. The pooled product for the genetic locus was loaded on a standard MiSeq v2 flow cell and sequenced in a 2x250bp paired end format using a v2 500-cycle MiSeq reagent cartridge.
2. The MiSeq run was performed with a 20% PhiX spike added.
3. Primers complementary to the Fluidigm CS1 & CS2 oligomers were added to appropriate wells of the reagent cartridge to server as sequencing and index read primers.
4. Base calling was done by Illumina Real Time Analysis (RTA) v1.18.54 and output of RTA was demultiplexed and converted to FastQ format with Illumina Bcl2fastq v2.20.0 
5. 12S Sequencing primers (5’ to 3’ direction):
 - FL1-CS1(read1)	`A+CA+CTG+ACGACATGGTTCTACA`
 - FL1-CS2(read2)	`T+AC+GGT+AGCAGAGACTTGGTCT`
 - FL2-CS1rc		`T+GT+AG+AACCATGTCGTCAGTGT`
 - FL2-CS2rc(index)	`A+GAC+CA+AGTCTCTGCTACCGTA`


#### Positive Control

>Please include information about any positive controls, used in every PCR run to verify success of the PCR reaction. This should include a description of the sequence(s), the concentration and volume added, and the reference sequence(s).

#### Negative Control

>Please include information about any negative controls, such as PCR-grade water used as a no template control (NTC) when setting up each PCR plate.

### Quality Control

<quality control steps>


### Basic Troubleshooting Guide

> - Identify known issues associated with the procedure, if any.
- Provide troubleshooting guidelines when available.

## REFERENCES

> - Insert all references cited in the document.
- Please insert full DOI address when available, e.g. http://doi.dx.org/10.1007/s11258-014-0404-1.

## APPENDIX A: DATASHEETS

> Link templates (e.g. preformatted spreadsheets) used to record measurements and report on the quality of the data as well as any documents such as manufacturer specifications, images, etc that support this protocol. Please include a short note describing the document's relevance.