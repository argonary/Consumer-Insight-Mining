# Consumer Insight Mining via Unstructured Web Data

## Key Findings
- Infiniti is the most aspirational brand by lift with purchase-intent phrases (2.28), ahead of Lexus (2.03) and Acura (1.83)
- BMW dominates raw discussion volume (3,100 posts) but shows low co-mention lift, consistent with it being used as a benchmark rather than an active consideration target
- Three perceptual clusters emerge: Toyota/Honda/Nissan (mainstream), Lexus/Acura/Infiniti (Japanese luxury), and Mercedes/Audi/Cadillac/BMW (European and domestic luxury)
- The corpus follows a Zipf-like power-law distribution (theta = -2.61), confirming it has the statistical structure of natural language

## Overview
NLP analysis of ~10,000 forum posts scraped from the Edmunds entry-level luxury sedan thread. Applies Zipf's law validation, brand frequency analysis, co-mention lift, MDS brand mapping, attribute-brand lift, and aspirational brand detection using bigram phrase matching.

## Methods
- Zipf's law validation via OLS regression
- Brand frequency counting with model-to-brand normalization
- Co-mention lift with a 5-word proximity constraint
- MDS projection from lift-derived distance matrix
- Attribute-brand lift across five attribute categories
- Aspirational brand detection using bigram phrase matching

## Stack
Python, NLTK, statsmodels, scikit-learn, seaborn, matplotlib

## Data
Scraped from the Edmunds entry-level luxury performance sedans forum thread using Selenium. Raw data not included in this repo.
