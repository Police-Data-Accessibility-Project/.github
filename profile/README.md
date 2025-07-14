# Welcome!
The Police Data Accessibility Project (PDAP) is a nonprofit based in Pittsburgh, PA. 

Visit [pdap.io](https://pdap.io) to learn more and access data. You are also welcome to introduce yourself and meet data-access-minded people [in our Discord server](https://discord.gg/wMqex8nKZJ)!

## Contributing code
Thank you for your interest in helping out!

We mostly use Python (API, back end), Vue JS (front end), and SQL.

#### [Good first issues](https://github.com/orgs/Police-Data-Accessibility-Project/projects/25/views/1) for new contributors
#### [Volunteer](https://airtable.com/appcYa6x4nS7W8IR3/shrk9c5sBsBr3cdJJ) to use your data skills on a community request
#### [Hugging Face](https://huggingface.co/PDAP) is where we maintain machine learning models

## PDAP Ecosystem
We have a few ongoing projects in repositories below, to help us share data and skills.

#### [Roadmap](https://github.com/orgs/Police-Data-Accessibility-Project/projects/21/views/2) | [Docs](https://pdap.io)

### Active services
Check out our [uptime stats](https://stats.uptimerobot.com/sl3EoLr7KL) for a high-level look at our services. We have several services automated. They include:
- [Automatic Archives](https://github.com/Police-Data-Accessibility-Project/automatic-archives) of Data Sources
- Syncing [Data Requests](https://github.com/orgs/Police-Data-Accessibility-Project/projects/26) from our database to GitHub.
- The Health Monitor checks our app for basic functionality.
- Notifications are sent to users who follow locations at pdap.io.
- We geocode locations and agencies which are missing metadata.


```mermaid %% Here's a guide to mermaid syntax: https://mermaid.js.org/syntax/flowchart.html

%%{ init: {
    'flowchart': {'curve': 'basis'}
  } }%%

flowchart TD

classDef white color:black,fill:#fffbfa,stroke:black
classDef purple color:black,fill:#cbbfca,stroke:black
classDef gold color:black,fill:#e2be77,stroke:black

requests["`Data Requests made by community members`"]:::purple
automation["`Automated crawling for Data Sources with 
*data-source-identification*; 
automatic maintenance with *data-cleaning*`"]:::gold
db["`Data Sources Database 
(via API)`"]:::white
app["`Apps like *data-sources-app* and *automatic-archives*, helping people answer questions with data`"]:::gold
scrapers["`*scrapers* and other code created in response to Data Requests`"]:::purple

automation --> db;
db --> app;
requests --> db; 
db --> scrapers
```
