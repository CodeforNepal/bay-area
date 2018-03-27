# Code for Nepal - Akshara Meeting

## Event

|   event       | Google hangout meeting
| :------------ |:-------------------------------------------- |
| Schedule      | Mar 21, 2018 Wednesday at 07.00 PM to 08.00 PM  |
| Venue         | Remote |

## Agenda

* Going over movks for 
* Make some concrete technical decisions
* Gather deedbacks on the mocks, and general catch up

## Attendees

* Anup Dhamala
* Aish Raj Dahal
* Prasanna Suman
* Pragya Tripathi
* Kritish Rajbhandari

## Conversation Summary

-> prasanna explained the mocks.
-> anup asked app vs web (prasanna said for web now, but try to use scalable design/tools)
-> kritish commented looks consistent with plans so far.
-> discussion on progressive webapp.

-> prasanna mentioned that should do a hackathon and start doing things. 
-> prasanna asked for some concrete steps. 

aish-raj: said maybe not take big steps, but rather focus on few fundamental things. 
-> decide on front-end, backend, etc. 
-> example - python for backend as previously discussed which most people know/understand.

anup:
-> what are the requirements?
-> queries, users?

prasanna: over time we'll need authentication for users etc., but for now only something a client can see is okay.

prasanna: decide on metadata. 

anup: using elasticsearch seems enough.

nripesh asked: does elasticsearch scale?, anup: yes elasticsearch scale. 

Ijesh: search is limited for language. 

aishraj: lucene isn't that great for Nepali. 

prasanna: make action items, assign roles, do hackathon based on this. 

prasanna had some I wasn't clear about, then anup answered saying doublle.

prasanna: minimal frontend, elastic search backend, data-ingest using python.

anup: said sounds good. 

prasanna: comment on hosting.

kritish: finally was able to see the mock. asked questions about cross linking from authors to books, vice versa. 

ijesh: ranked search based on elastic search, etc. (ex: devkota then laxmi will come first, but elastic search is based on clicks, not scalable perfectly). 

prasanna: summer of code, fundraising, etc - lacking context.

aishraj: shreyasha said she'd talk to prashish regarding this. should start fundraising by March-end. 

prasanna: will touchbase regarding this as well.

anup: what's the best way to colaborate?

prasanna: trying to figure this out.

anup: where does biography come from?

prasanna: eventually crowdsourced, future wikipedia. 

anup: text search in nepali, not sure about whats possible/not possible. 


## Action Items

- Prasanna to create detailed list of task to commence work on MVP
- We have decided to stick to the basic for the MVP - Simple PWA for frontend (TypeScript + React (Alt React like Preact)), ETL in Python, Elastic for backend 
- Need to follow up on Summer of Code plans






