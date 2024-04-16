# Hello!
The Police Data Accessibility Project (PDAP) is a nonprofit based in Pittsburgh, PA. 

Visit [pdap.io](https://pdap.io) to learn more and access data. You are also welcome to introduce yourself and meet data-access-minded people [in our Discord server](https://discord.gg/wMqex8nKZJ)!

## Contributing code
Thank you for your interest in helping out!

We mostly use Python (API, back end), Vue JS (front end), and SQL.

#### [Good first issues](https://github.com/orgs/Police-Data-Accessibility-Project/projects/25/views/1) for new contributors
#### [Volunteer](https://airtable.com/appcYa6x4nS7W8IR3/shrk9c5sBsBr3cdJJ) to be connected with projects in need of data skills
#### [Roadmap](https://github.com/orgs/Police-Data-Accessibility-Project/projects/21/views/2) of planned work
#### [Docs](https://pdap.io) about using PDAP tools
#### [Hugging Face](https://huggingface.co/PDAP) is where we maintain machine learning models

## PDAP Ecosystem
We have a few projects and experiments going to advance our mission.

```mermaid %% Here's a guide to mermaid syntax: https://mermaid.js.org/syntax/flowchart.html

%%{ init: {
    'theme': 'base',
    'flowchart': {'curve': 'linear'}
  } }%%

flowchart TD

classDef white fill:#fffbfa,stroke:black
classDef purple fill:#a895a7,stroke:black
classDef gold fill:#d5a23c,stroke:black

  submissions["`Human maintenance and submissions`"]
  crawling["`Automated crawling with **data-source-identification** repository`"]
  maintenance["`Automated maintenance with **data-cleaning** repository`"]
  db[("`Data Sources Database
(read and updated via API)`")]
  app["`The **data-sources-app**, which helps people search the database and answer questions`"]

submissions:::white --> db:::purple;
crawling:::white ---> db;
maintenance:::white --> db;
db --> app:::gold;
```
