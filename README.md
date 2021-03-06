# Pediatric_CKD_Cohort_Holle_2022
Chronic kidney disease (CKD) is characterized by a sustained pro-inflammatory response. The underlying mechanisms are incompletely understood, but may be linked to gut dysbiosis. Dysbiosis has been described in adults with CKD; however, comorbidities limit CKD-specific conclusions. We analyzed the fecal microbiome, metabolites and immune phenotypes in children at three different CKD stages (G3-G4, G5 (hemodialysis), after kidney transplantation) and healthy controls. Serum TNF-α and sCD14 were stage-dependently elevated, indicating inflammation and gut barrier dysfunction. We observed microbiome alterations in CKD, including a diminished production of short-chain fatty acids. Bacterial tryptophan metabolites were increased in CKD. CKD serum activated the aryl hydrocarbon receptor and stimulated TNF-α production by monocytes, corresponding to a shift towards intermediate/non-classical monocytes. Unsupervised T cell analysis revealed pro-inflammatory shifts in MAIT and Treg cells. Thus, gut barrier dysfunction and microbial metabolites exacerbate inflammation and may therefore contribute to the increased cardiovascular burden in CKD.
# Study cohort 
In this cross-sectional study, we recruited patients from the Department of Pediatric Gastroenterology, Nephrology, and Metabolic Diseases at Charité University hospital in Berlin, Germany, between February 2018 and June 2018. Written informed consent was obtained from all participants and/or their parents prior to study entry. The study was approved by the local Ethical Review Board (EA2/162/17). All procedures performed were in accordance with the ethical standards of the institutional and national research committees and the 1964 Helsinki declaration and its later amendments or comparable standards.
Patients (age 3-18 years) were enrolled in the following groups:
- CKD group: CKD stage G3-G4, estimated GFR (eGFR) 15-60 ml/min*1.73m2
- HD group: CKD stage G5D, patients on maintenance hemodialysis, enrolled earliest four weeks after initiation of HD
- KT group: patients after successful KT, earliest four weeks after KT, without a history of rejection or chronic graft failure, eGFR > 60ml/min*1.73m2
- HC group: normal kidney function, treated at the hospital for reasons other than kidney disease
We excluded patients with a body weight below 15kg, acute or chronic inflammatory diseases, fever, diabetes, chronic liver disease, inflammatory bowel disease, or other gastrointestinal disorders (constipation, diarrhea, short bowel syndrome). Patients with antibiotic prophylaxis or treatment within the four weeks prior to recruitment were excluded.

# 16S processing 
Sequence processing and OTU classification 
The sequences obtained were processed using LotuS (1.62)(16). Poisson binomial model based read filtering was applied(17). OTU clustering (UPARSE)(18) was based on a sequence similarity of 97%, while SILVA(19), GreenGenes(20) and HITdb(21) were incrementally used as databases for taxonomic assignment Lambda taxonomic similarity search. The taxonomic classification (genus 95% identity) was parsed using a custom Perl script, such that unassigned taxonomic levels were assigned to the last known taxonomic level and sequentially numbered. Normalization and computation of alpha diversity measures were performed using the rarefaction tool kit (RTK 0.93.1) with default settings(41).

# Data
phyloseq_object.r: hold information at all phylogenetic level and metadata of the study cohort.
OTU.txt, Phylum.txt, ... : abundance tabels generarted using LotusS (1.62).
