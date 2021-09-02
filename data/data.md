# Data file for CoV_sequences.fasta

## Search parameters for SARS-CoV, SARS-CoV-2, and MERS-CoV genome sequences
https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/virus?SeqType_s=Nucleotide&VirusLineage_ss=Severe%20acute%20respiratory%20syndrome%20coronavirus%202%20(SARS-CoV-2),%20taxid:2697049&VirusLineage_ss=Severe%20acute%20respiratory%20syndrome-related%20coronavirus,%20taxid:694009&VirusLineage_ss=Middle%20East%20respiratory%20syndrome-related%20coronavirus%20(MERS-CoV),%20taxid:1335626&QualNum_i=50&Completeness_s=complete&Region_s=Africa&Region_s=Asia&Region_s=South%20America

## Commentary
Includes sequences for SARS-CoV, SARS-CoV2, and MERS-Cov.
Search filters: only complete sequences, maximum 50 unknown bases, from Africa, Asia, and South America.

Download from NCBI page wouldn't go through for some reason, even with adblockers off on both chrome and Firefox. Actual dataset obtained from Kevin, who was able to download using the link above. 

# Data File for Analysis 1

## Search Parameters
https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/virus?SeqType_s=Nucleotide&VirusLineage_ss=SARS-CoV-2,%20taxid:2697049&Region_s=Africa&Region_s=Asia&Region_s=Oceania&Region_s=South%20America&Completeness_s=complete&Lineage_s=B.1.1.7&Lineage_s=B.1.351&Lineage_s=B.1.351.3&Lineage_s=P.1&Lineage_s=P.2&Lineage_s=B.1.617.2&Lineage_s=R.1&Lineage_s=B.1.1.214

## Commentary
Search done on 8/18/21

Search Filters: 
sequence type: nucleotide, only complete sequences, maximum 50 unknown bases, species: SARS-CoV2
GeoLocation: Africa, South America, Asia, and Oceania,
Pangolins: B.1.1.7, B.1.351, B.1.351.3, P.1, P.2, B.1.617.2, R.1, B.1.1.214

Search filters described in Analysis plan yielded a file size that was way too large. Removed sequences from North America and Europe, and specificed pangolins for more manageable file size. 

Pangolin filters include 2 not listed in variant_dict to test splice_fasta's ability to discriminate pangolins.

# Data file for Analysis 2

## Search Parameters
https://www.ncbi.nlm.nih.gov/labs/virus/vssi/#/virus?SeqType_s=Protein&VirusLineage_ss=SARS-CoV-2,%20taxid:2697049&QualNum_i=50&ProtNames_ss=surface%20glycoprotein&Completeness_s=complete&USAState_s=IL

## Commentary
Search done on 8/20/21

Search Filters: 
sequence type: protein, only complete sequences, maximum 50 unknown amino acids, species: SARS-CoV2
GeoLocation: Illinois, U.S.

Geolocation was limited to samples from Illinois to reduce file size. 

Date must be set as the third line item in FASTA headers for date_diff and time_vs_align_score functions. 
Example header: >QWF05856.1 |R.1|2021-04-25|Severe acute respiratory syndrome-related coronavirus