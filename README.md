# Citational Refusal
This repository contains code related to analysis on the reception of Alexis Wright's novel Carpentaria. 

## Notebooks 
This repository contains two notebooks:
- **01_word_frequency_tfidf_analysis.ipynb** this notebook contains word frequency and TF-IDF analysis of the document.
- **02_textual_attention_analysis.ipynb** this notebook roughly quantifies citational/textual attention by 'chunking' the documents in 180 word (roughly paragraph) segments and then tracks/measures the distribution of the citation across the text (not density). That is:
- If a name appears many times in one section → low chunk score
- If a name appears once in many sections → high chunk score
This intends to provide a rough metric of whether a specific theorist becomes the dominant interpretive frame for an article, or is mentioned only in passing. 

## Outputs
This repository contains a number of csv files that guide analysis:
- **person_chunk_attention_by_document.csv** this document lists all analysed documents in the first column, and then lists the dominant/most mentioned theorists in the header. Each document is broken into an indivudal 'chunk_score' for each theorist thereby showing which theorists are most intensly engaged. 
- **person_corpus_comparison.csv** this files provides a rough summary of the most domiannt theorists across the corpus wuth their associated chunk_score.

## File Naming Convention
### Format for pdf files are as follows: Template
YYYY-MM-DD__author-surname-given__source__title__type.pdf

for example: 
2026-02-21__sharrad-paul__european-association-for-commonwealth-literature__beyond-capricornia-ambiguous-promise-in-alexis-wright__conference-presentation.pdf

is

Parsed Metadata Fields
Date
2026-02-21
Publication or delivery date, expressed in ISO 8601 format.
Author
sharrad-paul
Author name in surname–given order:
Surname: Sharrad
Given name: Paul
Source
european-association-for-commonwealth-literature
Hosting organisation or venue, rendered in slug form.
Title
beyond-capricornia-ambiguous-promise-in-alexis-wright
Full work title in slug form. Reconstructed in standard orthography:
Beyond Capricornia: Ambiguous Promise in Alexis Wright
Type
conference-presentation
Document classification indicating delivery format rather than journal publication.

Other formats include: book-chapter, book-review, conference-presentation. 