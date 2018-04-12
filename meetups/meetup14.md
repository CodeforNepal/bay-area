# Code for Nepal - Akshara Meeting

## Event

|   event       | Google hangout meeting
| :------------ |:-------------------------------------------- |
| Schedule      | April 11, 2018 Wednesday at 07.39 PM to 08.20 PM  |
| Venue         | Remote |

## Agenda

* Updates from Hackathon on Saturday

## Attendees

* Anup Dhamala
* Ijesh Giri
* Nripesh Parajuli
* Pragya Tripathi
* Prasanna Suman

## Conversation Summary

- Prasanna - Did foundational work, still needs to work more on it
- Kritish - Made Front-end mocks, added more information on metadata
- Ijesh - Added ingestion to ETL pipeline but haven't integrated with Anup's work yet. Needs to integrate with Anup's work. After that back end
- Anup - Did Elastic Search site updates, added transliteration config, filtered stopwords (found list online), worked on stemming, researched more 
- Pragya - Took trained model from nep-ocr, used it to run some tests. Scenarios with picture on text, first page.

- Nripesh - benchmarking, verify accuracy. Ijesh's suggestion is to tag text with low accuracy.

- Ijesh - Final MVP's demo for each piece
- Prasanna - 4 more days left, need to push through

- Hosting - Use Code for Nepal's account for hosting. Most probably AWS-Singapore. Need to host our MVP server - Prasanna to set it up for now. Need to dockerize so that we can easily move in future.

- ETL - Ijesh and Anup's work needs to be coordinated.
  - Integration with OCR - Nripesh already has a script. Need to create a Dockerfile.

- Pragya's questions 
  - do we need to concat lines? Not for MVP. We could add pagination in future.
  - Do we need to make tesseract asynchronous? Not for MVP. We need to address it for future.
  
- Anup's question
  - Are we going to fill in all of metadata? Whatever we can extract from scripts.
  
- Prasanna - Need to make architectural diagrams and document what we are doing.

## Action Items

- Prasanna - Needs to talk to C4N's founder for C4N's server information. Finish UI code. Send Anup access information.
- Everyone - document architecture for every component
- Everyone - pick a name
- OCR - Create a Dockerfile (Nripesh), tagging for low accuracy (Pragya)
- Anup - Configure AWS instance for ES when he gets server access
- Ijesh - Data injestion from pustakalaya.org
