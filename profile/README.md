# Hello!
The Police Data Accessibility Project (PDAP) is a nonprofit based in Pittsburgh, PA. 

Visit [pdap.io](https://pdap.io) to learn more and access data. You are also welcome to introduce yourself and meet data-access-minded people [in our Discord server](https://discord.gg/wMqex8nKZJ)!

## Contributing code
Thank you for your interest in helping out!

We mostly use Python (API, back end), Vue JS (front end), and SQL.

#### [Good first issues](https://github.com/orgs/Police-Data-Accessibility-Project/projects/25/views/1) for new contributors
#### [Volunteer](https://airtable.com/appcYa6x4nS7W8IR3/shrk9c5sBsBr3cdJJ) to use your data skills on a community request
#### [Roadmap](https://github.com/orgs/Police-Data-Accessibility-Project/projects/21/views/2) of planned work
#### [Docs](https://pdap.io) about using PDAP tools and terminology
#### [Hugging Face](https://huggingface.co/PDAP) is where we maintain machine learning models

## PDAP Ecosystem
We have a few ongoing projects and experiments. They all help with the first step of answering any question about a police system: find a source of useful data.

```mermaid %% Here's a guide to mermaid syntax: https://mermaid.js.org/syntax/flowchart.html

%%{ init: {
    'flowchart': {'curve': 'basis'}
  } }%%

flowchart TD

classDef white fill:#fffbfa,stroke:black
classDef purple fill:#cbbfca,stroke:black
classDef gold fill:#e2be77,stroke:black

requests["`Data Requests made by community members`"]:::purple
automation["`Automated crawling for Data Sources with 
*data-source-identification*; 
automatic maintenance with *data-cleaning*`"]:::gold
db["`Data Sources Database 
(via API)`"]:::white
scrapers["`*scrapers* and other code created in response to Data Requests`"]:::purple
app["`The *data-sources-app*, helping people find Data Sources and answer questions`"]:::gold

automation --> db;
db --> app;
requests --> db 
db --> scrapers
```
