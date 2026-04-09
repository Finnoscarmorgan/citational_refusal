# Citational Refusal

This repository contains code for analysing the reception of Alexis Wright’s novel *Carpentaria*.

---

## Notebooks

This repository includes two primary notebooks:

### 01_word_frequency_tfidf_analysis.ipynb
Performs word frequency and TF–IDF analysis across the document corpus.

### 02_textual_attention_analysis.ipynb
Implements a method for approximating citational or textual attention by segmenting documents into ~180-word chunks (roughly paragraph length). It then measures how references are distributed across these segments.

The method captures **distribution rather than density**:

- If a name appears many times within a single section → **low chunk score**
- If a name appears once across many sections → **high chunk score**

This provides a heuristic measure of whether a theorist functions as:
- a dominant interpretive framework, or  
- a passing reference

---

## Outputs

The repository includes several CSV files supporting analysis:

### person_chunk_attention_by_document.csv
- Rows: individual documents  
- Columns: theorists (most prominent across the corpus)  
- Values: chunk-based attention scores per document  

This file indicates which theorists are most intensively engaged within each document.

### person_corpus_comparison.csv
Provides a summary of dominant theorists across the full corpus, alongside their associated chunk scores.

---

## File Naming Convention

### Format
YYYY-MM-DD__author-surname-given__source__title__type.pdf
### Example
2026-02-21__sharrad-paul__european-association-for-commonwealth-literature__beyond-capricornia-ambiguous-promise-in-alexis-wright__conference-presentation.pdf

---

## Parsed Metadata Fields

### Date
**2026-02-21**  
Publication or delivery date in ISO 8601 format.

### Author
**sharrad-paul**  
Surname–given format:
- Surname: Sharrad  
- Given name: Paul  

### Source
**european-association-for-commonwealth-literature**  
Hosting organisation, venue, or publication, expressed in slug form.

### Title
**beyond-capricornia-ambiguous-promise-in-alexis-wright**  
Full title in slug form. Reconstructed:

*Beyond Capricornia: Ambiguous Promise in Alexis Wright*

### Type
**conference-presentation**  
Indicates format of dissemination rather than publication type.

---

## Supported File Types

- book-chapter  
- book-review  
- conference-presentation  
- journal-article  

---

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