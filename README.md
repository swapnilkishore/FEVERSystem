# FEVERSystem
An end-to-end system for automated fact extraction and claim verification.

This system was designed for the FEVER task which involves extracting evidence for a claim and judging whether it can be verified or not using Wikipedia pages as evidence.
There are three main tasks in this project. They are carried out in a sequential manner. These are document retrieval, sentence selection and recognizing textual entailment.

Dataset: 

FEVER (Fact Extraction and VERification) consists of 185,445 claims manually classified as ‘SUPPORTED’, ‘REFUTED’, or ‘NOTENOUGHINFO’. The purpose of this dataset is to evaluate an end-to-end system that performs the task of evidence extraction and claim verification. The dataset is divided into training data and testing data. The training dataset consists of the following fields:
Id: The id of the claim
label: One of {SUPPORTED, REFUTED, NOTENOUGHINFO}
claim: The text of the claim
evidence: A list of evidence sets extracted as being relevant to the claim.

Strategies:

Document Retrieval: MediaWiki API, Sequence Matcher
Sentence Selection: TF-IDF Score, Cosine similarity
Claim Labelling: Pre-trained BERT
