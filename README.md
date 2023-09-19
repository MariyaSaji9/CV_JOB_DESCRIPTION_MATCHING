# Resume Matching with Job Descriptions Using PDF CVs
***
# About
***
/ This project endeavors to establish an automated system designed to facilitate the precise alignment of candidate resumes with job descriptions, leveraging Natural Language Processing (NLP) and Transformer Libraries, the DistilBERT model. The overarching goal is to optimize the recruitment process by effectively extracting, categorizing, and assessing information from resumes. Subsequently, this system identifies candidates who best match specific job descriptions.
# Phases in the project
***
### 1.	PDF Data Extraction
/ The objective is to extract critical information from resumes provided in PDF format. This process involves extracting skills, categorizing resumes into job categories, and retrieving educational qualifications. The implementation leverages the Tika library for PDF parsing, regular expressions for pattern matching, and the NLTK library for text preprocessing.
### 2.	Job Description Data Understanding:
/ This phase centers on acquiring and comprehending job descriptions drawn from the Hugging Face dataset. This phase harnesses the Hugging Face datasets library to curate job descriptions and preprocess it. This compilation is pivotal in facilitating the matching process.
### 3.	Candidate Job Matching
/ Candidate-Job Matching involves a multi-step process to evaluate the suitability of candidates for specific job descriptions. Here are the detailed steps and findings:
##### 1.	Embedding Generation:
/ After preprocessing the Job descriptions and CVs, Leveraged the DistilBERT model from Hugging Face's Transformers library to generate embeddings for job descriptions and CVs.
##### 2.	Similarity Calculation: 
/ Computed cosine similarity scores between the embeddings of job descriptions and CVs. This quantified the similarity between each CV and job description.
##### 3.	Ranking and Selection:
/ For each job description, ranked CVs based on their similarity scores. The top 5 CVs with the highest similarity scores were selected as potential matches. The ranking process allowed for efficient identification of the most relevant candidates for each job description. It ensured that the most promising candidates were presented to recruiters.



