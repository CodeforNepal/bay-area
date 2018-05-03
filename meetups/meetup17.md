# Meeting Notes 03-05-2018

## Agenda
- Catchup on the progress so far
- Domain name decisions

## Team Updates

### ऐश 

- AWS is in a frustrating long enterprise sales cycle. Aish looked into  Azure. Azure has an anual  5000 USD credit for non-profits.
> Shreyasha Comment: 
> - Double check with Ravi about Azure, because C4N may have remaining credits for Azure
> - Ravi told Aish to do what Aish things is the best

- Aish did SSL on kabootar.im and for MVP we can try something similar, where parijat.kabootar.im will map to the server Anup setup. The process is documented here - https://certbot.eff.org/lets-encrypt/ubuntuxenial-nginx

> Anup Comment: 
> - Anup has also worked on SSL for Docker which we can use to setup for parijat.kabootar.im - https://github.com/Code4Nepal/akshara-project/tree/nginx_setup_ssl

### प्रज्ञा

*Might be missing things here*

- Tried different libraries to improve accuracy for Nepali OCR
- Created OCR code pull request
- We will use tessaract from bash command line
 
### अनुप 

- Anup setup reverse proxy using nginx for es and frontend. This addresses the following issues - 
  - CORS restrictions from frontend. ES is served from /es when fronend is served from / 
  - Public access to the ES instance is restriced to GET requests
- He had some issues getting frontend to work correctly, Prasanna to look into it.
- The dev server is almost ready, sans SSL setup

### इजेश

- Ijesh has ETL scripts in progress from SahityaSangraha. He can use the :9200 port to injest into dev ES server.
- Some issues with Ijesh access to GH. Should be resolved now.

### प्रसन्न

- Worked mostly on integrating frontend with the production setup, and little issues here and there
- Updated the production setup to user superstatic whcih is a more production ready server

## Name

In order to setup SSL we need to determine the name. While we can defer the decision momentarily and use parijat.kabootar.im instead, we need to short list the candidates based on the following criterias - 

1. Domain name must be available
2. Domain name must be easy to remember, so no high Sanskrit
3. Domain name must be generic enough, and not focused on Nepali alone

For now, we are using parijat.kabootar.im for MVP

## Action Items

- Short list of potential domain names based on what is available (Prasanna)
- Get a demoable version up and running by this week. Bulk of the work remaining at this point is frontend related. (Prasanna and who-ever else)
