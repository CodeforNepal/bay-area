# Code for Nepal - Akshara Meeting

## Event

|   event       | Google hangout meeting
| :------------ |:-------------------------------------------- |
| Schedule      | Mar 28, 2018 Wednesday at 07.30 PM to 08.20 PM  |
| Venue         | Remote |

## Agenda

* Go over tasks for the MVP and take assign them
* Updates
  * Ijesh has been scraping some of the literature content and trying out Elastic
  * Nripesh has an update on OCR for Nepali which he mentioned last Wednesday after folks left
  * Updates from Shreyasha regarding SoC

## Attendees

* Aish Raj Dahal
* Anup Dhamala
* Ijesh Giri
* Nripesh Parajuli
* Pragya Tripathi
* Prasanna Suman
* Kritish Rajbhandari

## Conversation Summary

- Prasanna has come up with tasks and sub-tasks in Github.
- One of the goals of the meeting -> find owners for the tasks
- Design discussion for data 
- What content can be searchable? Need to come up with things we need to make searchable (this was also covered last time). Kritish -> author, date, genre, language etc. (Kritish will come up with more)
- Anup: We now need to download text, parse and index for Elastic Search (ES). CLI script or simple UI based intermediary needed. Goal to make it usable by anyone for data collection. Right now, pick CLI script. In future, we might need UI. (Architecture may require to consider this for future)
- Prasanna: how to handle data corruption? 
  - Anup: Data can be easily modified in ES. ES has an API based interface. ES is not like database where things can be easily modified. We can re-index if needed in case of corruption. Snapshot can be taken for backup.
- Discussion about using SQL database along with ES.
  - Unanimous decision on using ES for MVP given our requirements. For future, we might need a database though.
- Pragya: While metadata of content can require edit, is the text content from different authors immutable?
  - Prasanna and Ijesh: We can take wikipedia approach but all for future considerations. For MVP, let's assume it is.
- Ijesh wrote a crawler to download Nepali poems from kavitakosh.org.
- Prasanna to begin front-end implementation.
- Discussed requirements for Elastic Search. Refer to https://github.com/Code4Nepal/bay-area/pull/2/commits/40eb7c280997d236edf59fd299cc9a1717d60c49
- Nripesh: A professor in Nepal has a Windows app. https://sourceforge.net/p/ne-ocr/wiki/Home/
  - Anup tried it and works alright (needs clear image, some mismatched characters, little buggy)
- How to ingest data into our system?
  * Create a json file with metadata and pass it to Anup?
- Need a Project Management platform -> Use Github's Kanban board
- Updates from Shreyasha: Summer of Code fund raising
  * Chosen to use Indiegogo or other fundraising platform to ask for $1000
	* She is writing fundraising blurb
- Aish checking on AWS account faster in Singapore

## Action Items

- Kritish to define metadata for searchable content
- Prasanna to work on front-end 
- Ijesh is going to come up with a schema for documents in ES
- Everyone - come up with name of a product
- Prasanna to add project management tool in github
- Shreyasha to send fundraising blurb by the weekend
