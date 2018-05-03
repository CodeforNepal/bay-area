# Start

- Remember to take meeting notes
- Ask about project management platform
- Create a git repository in Code4Nepal github
- Remember to talk about updates from Shreyasha

# MVP Tasks

## Data

We need a well defined data model, before much of the work can proceed. In this task, depending on the digital sources we have, we will create a data model for our documents. 

### Outcomes

1. Determine the different types of documents (poems, authors, pdfs etc) we will index.
2. Determine the metadata for each of these types that users will be able to search through.

## ETL (Extract Transform Load) 

For the MVP we intend to keep things simple with just a frontend over elastic search, but we don't want to potentially pollute elastic search when we import new stuff. We will first store all the disaparate data sources in (SQL or something else?) and make an ETL to Elastic Search in Python.

### Outcomes

1. Well defined workflow for adding new documents in the elastic search. 
2. Ensure that we can quickly revert potential data corruption or loss 

## Frontend Implementation Work

The task is to create a frontend according to the mocks 

### Outcomes

1. Prepare a base foundational work universal app using preact, redux. Server rendering is a must for SEO but eventually we need to also make it a Progressive Web App.

2. Implement various views based on the mocks

    - Implement landing search page
    - Implement search results page
    - Implement feature filters modal
    - Implement the landing page recently viewed, most viewed lists

## Elastic Search Experiments

We need to explore the features of elastic search, and how it will work with our use case.

### Outcomes

1. Devanagari search quality tests

    - Figure out the state of art practices.

2. Transliterated Search

    - While indexing devanagari text, we will also store them as the transliterated latin text. This will allow users to search using latin script. Investigate the most performant way of doing this.

## OCR

We will run OCR for the PDF scans from pustakalaya.org. 

### Outcomes
1. Test quality for the Nepali OCR. In full text search high accuracy is not necessary, but a ball park number on the quality of OCR would be good to have
2. Figure out how OCR fits into the ETL pipeline

## Backlog Tasks

These are some tasks that  doesn't need to be worked on immediately, but we should keep them in mind:

0. Come up with a name of the product!
1. DevOPs decisions - where do we host the final MVP, what domain name do we use
2. For the MVP we want to keep things simple so for now we can use simple scripts for to injest data in our system. But ultimately this is a croud source platform, so anyone should be allowed to add data.
3. Connect with designers in the community to get feedback
