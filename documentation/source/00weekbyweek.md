<u>Week by Week</u>

# Class Syllabus

## Prerequisites - Suggested Reading/Viewing

### Pangeo, COGS and maybe Stac

![](https://github.com/tonybutzer/etscrum/raw/main/00-presentation/ard/abernathey-is-right.PNG)

---

![](https://raw.githubusercontent.com/tonybutzer/etscrum/main/00-presentation/ard/new-arch.PNG)

---
- The Future of Data-driven Discovery in the Cloud - Ryan Abernathey (Columbia University)
	- https://www.youtube.com/watch?v=7kDYfUe0Zhw
	- `The above youtube is worth watching - 14 minutes`


### COGs and ARD
- https://medium.com/planet-stories/cloud-native-geospatial-part-2-the-cloud-optimized-geotiff-6b3f15c696ed
- https://medium.com/planet-stories/towards-on-demand-analysis-ready-data-f94d6eb226fc

## Week by Week Class Summaries

### WEEK ONE
#### Week One Objectives

- FEEDBACK - send me direct chats with pithy comments that might improve our mission
- ESIP - don't hold back science - Rich Signell
- Discuss the goals for this class - success criteria - move one more science project to the cloud
- Comments and viewpoint of Neal Pastick
- Demos
	
	- [nginx on cloud server](http://10.12.69.188)
	- [jupyter notebook without the code](http://10.12.69.188/pie)
	- [ET Viewer Side by Side no timeseries sad](http://10.12.69.233/user/harmony/notebooks/notebook/00-Viz/96-hvplot-experiment-image-annual-et-viewer-decorator-version.ipynb)
	- [time series panel demo - little code](http://10.12.69.233/user/harmony/notebooks/notebook/00-Viz/panel-timeseries-get-x-y-and-plot.ipynb)

	- I will move some of these to Neal's interim web servers
- Discuss the Student cross section
	- http://10.12.69.216/00define_ET.html#students
	- http://10.12.69.216/00define_ET.html#student-individual-goals
<img src="https://raw.githubusercontent.com/tonybutzer/etscrum/main/00-presentation/bonus-slides/case-study-1.PNG">

- Discuss two Case Studies - Commonalities and Not
	- Evapo
	- permaFrost
- Contact Tony Butzer for cloud questions
- Discuss notebook love hate meter - any notebook shy/sensitive folks?
	- its just a tool; "you're a tool tony"
	- `There will be lots and lots of notebooks in this class`
- Point to the two computers - field any questions
	- web 10.12.69.216 hweb
		- [AWS on-boarding website paper --LINK](http://10.12.69.216)
	- mini-pangeo 10.12.69.233 harmony
		- [mini-pangeo --LINK](http://10.12.69.233)
- Computer Access Methods
	- Jupyter via browser and url and `VPN`
	- Terminal inside Jupyter
	- direct ssh and scp access - public key
		- ssh ubuntu@10.12.69.216
		- ssh ubuntu@10.12.69.233
	- open ports allowed via firewalls
		- 80, 8080 http
		- 443, 8443 https
		- 22 ssh,scp
	- use of `tmux` for session preservation across network/VPN failures/timeouts - long running jobs

- Point to the website - nginx/sphinx driven
	- [AWS on-boarding The website paper --LINK](http://10.12.69.216)
- Point to the github - 
	- [https://github.com/tonybutzer/harmony](https://github.com/tonybutzer/harmony)
- Quick Jupyter Session - jupyter fitting from single jupyter -- to self scaling hubs
	- focus here will be primarily mini-pangeo scope - a group of 13 students
- Self-directed study hints
	- notebook repo - past pangeo training
		- If you need one on one jupyter training I can arrange an hour with you
	- github link - needs pruning - notebook repo here: 
		- [https://github.com/tonybutzer/notebook/tree/master/00-Tutorial/00-Jupyter-Notebook-Pieschke](https://github.com/tonybutzer/notebook/tree/master/00-Tutorial/00-Jupyter-Notebook-Pieschke)
		- [https://github.com/tonybutzer/notebook](https://github.com/tonybutzer/notebook)
		- Tony can help you find just the right example or create it for you.
		- We wil use some of these examples in class and the Labs
- future todo - feedback based
	- create very small notebook snippets that illustrate concepts
	- refine sections of this "paper" and build examples
1. Project Kickoff and refinement of goals
	- Is this anything? - trial and error Seinfeld
		- doing this class is scary must be what its like to do stand-up comedy
		- this class is `new` sort of a science experiment in itself
	- `PRIOR Experience`
		- linux
		- docker
		- AWS
		- python
		- jupyter
		- management/leadership
	- `I want to build a notebook that radar charts the students`
	- Class questionnaire - via email - or maybe a notebook
	- Communication preference of each student
	- efficiency and boredom mitigation
		- perhaps split each 1 hour into - concepts and practice - allow folks to bail at 1/2 way point
		- perhaps - threads or channels
			- jupyter thread
			- linux thread
			- docker thread
			- devops thread
			- python thread
			- management leadership - steering committee thread for PANGEO - strategy

	- I want Neal to drive most of the agenda and deep dive talks - at least initially - people can opt out
		- for example I could write a chapter on costs in AWS
			-perhaps most would be interested - I know Neal is
1. Week ONE - DEC 1,2020 Introduction and Basic Cloud Tour 
	- Quick overview of this document
		- added a glossary
		- please skim
		- if you have comments or questions - please use Teams/Chat to contact me
			- I will likely post some of the converstaions in this document
	- Neal's team won a free mini-pangeo
		- terraform 
		- the littleist jupyter hub - intro
	- Neal wanted a kanban too/also
	- SEE DEVOPS WEEKLY
		- [DEVOPS LINK](http://10.12.69.216/27etops.html?highlight=devops)

## Teams Note
Hey Class: - the course website is starting to take shape and is here:
- http://10.12.69.216/
	
we will fill in more color/detail as we go through our CASE Studies.
- our companion github repo is here - can't live in the cloud without github/dockerhub.
	- https://github.com/tonybutzer/harmony

---
- this is also where our cache of notebooks will live - like this one:
	- https://github.com/tonybutzer/harmony/blob/main/class/06-Instructor/01-Students.ipynb
	- https://nbviewer.jupyter.org/github/tonybutzer/harmony/blob/main/class/06-Instructor/01-Students.ipynb
---
	- See you all on tuesday December 1st at 12 NOON 
	- See you next week for an open lab
	- The week after that I will look at Areas of Interest and how they relate to ET modeling
---
# WEEK TWO 

## Preface

### The cross communication is way more important than the technology lessons
- working together and sharing talent
- moving to the cloud where its natural to share everything
- creating libraries and documentation for the common good of the data center
- allowing our hard work in science to be broadcasted to the widest possible audience
- removing data and people silos where ever and when ever we can

### Welcome to the JupyterHub and Pangeo 
- extraordinary week 2
- let the fun begin

## Outline

### For Neal's Project
1. Acquire a CHS CUSTOM ACCOUNT and a Project VPC `[DONE]`
2. Setup 2 computers - a tiny admin box and jupyterHub micro-pangeo
3. Project Management steps rapidly developed via a sphinx website - backed up in git
4. Spin up a jupyter hub for coding and engineering collaboration
5. layout the data pipline big steps and refine a simple WBS to work from
6. Spin up a quick Kanboard to track actions and report progress to Neal

#### Details Example
> [Yesterday 4:11 PM] Pastick, Neal (Contractor) J
    Those data wrangling, pre-processing steps (e.g. re-projection if needed, spatial extent alignment), and database development are all that needed before performing modelling in this simple example. That is, once I have the tabular database developed through extraction of geospatial at each field plot, I can commence model calibration/validation/deployment. 
​[Yesterday 4:18 PM] Pastick, Neal (Contractor) J
    Guess I was a little vague w/ the raster pre-processing steps - can't recall what the resolution or projection is of all those datasets. The biggest thing might be to clip the data to a common extent - using a shapefile that we upload - and reprojecting and resampling things. No hard core per-pixel compositing methods needed here.
​[Yesterday 4:20 PM] Pastick, Neal (Contractor) J
    Could also stack all those data into a giant xarray for model inference later on - might be overkill as I should be able to point the models to the individual datasets

- `Deep Thoughts` by Neal Pastick
	- Key takeaways from last week
	- Motivating words to inspire the troops to forge ahead.
	- Account status
		- next steps
	- Phases for the Data and Processing from:
		- portal scraping, ftp transfers to buckets
		- ...
		- SageMaker ML and voila moments
- Michelle Anthony - any thoughts or questions about how this **disruptive** technology might vector your mid-term roadmap?
- Matt Rigge - can you talk about your role and your team and your pipeline you are targeting for cloud operation.
- Dev Dahal - talk about logging into Jupyter - opening a terminal and cloning a repo and what you hope to use this class for in your real job
- Anyone else?
	- We talked about a bunch of stuff in week 1
	- Anything we need to clarify about the cloud, AWS or CHS?
- Example panel based applications
	- Glaciers
		- [https://edu.oggm.org/en/latest/explorer.html](https://edu.oggm.org/en/latest/explorer.html)
		- similar to some of our WMS apps with far less backend engineering - scaffolding
	- Data Viz applets
		- widgets
		- graph display libraries
		- SDSU viz expert team - coming soon
- Gradually these classes should become more democratic - with lots of individuals taking the mic.
- Review last Week
	- pangeo is great
	- cloud is great
	- public data assets stored in the cloud == game changing paradigm
		- you MUST start to use cloud, readily available (fingertips), analysis ready remote sensing data assets - or be left behind
		- L8
		- Collection02
		- Sentinel
		- HLS ...bump ...bump ... YES
		- Evporation Model Outputs - after they go thru ScienceBase validation - but maybe even raw for evaluation
	- one computer to rule them all - t3a.2xlarge
		- [https://aws.amazon.com/ec2/instance-types/t3/](https://aws.amazon.com/ec2/instance-types/)
		- 8 CPU, 32Gig Memory, 200Gig local-ebs-elastic-block-storage  - with S3 access
	- technology zen equation
```python
science_joy = 1 * ec2 + docker * 1e3
```

### A World of Twos
- two computers
	- t2.micro
	- t3a-2xlarge
- two infrastructure elements
	- ec2
	- docker
- two technology companions
	- jupyter
	- python
- two science - image processing packages; fundamental building blocks.
	- xarray
	- pandas
- two people - who are "ALL IN" on the Cloud!
	- tony butzer
	- Rich Signell
- two barriers toward cloud acceptance
	- jargon
	- complexity

### Special Recognition for Kelcy (AWS CHS Credentials)
- implications for data movent to and from buckets directly from servers on-prem at EROS

### "Hey Tony; can I have an account on Neal's mini-pangeo?"
- "Yep, Yes, trueDat, Si, qui, Ja"
- ## हो   
- ## Hō

---


## Student Getting Started Instructions
#### Signing into the jupyterhub-mini-pangeo

- 10.12.69.233
    - username is '[LASTNAME]'
    - password is `harmony`


### git repo clone

- clone our notebook repo
- next week we will do a `git pull` for updates

### Instructions

![](./Assets/new-term.PNG)

#### open a terminal in jupyter
    - find Home Page - browser tab - or middle click jupyterhub above - tony to demo
    - [new] button - terminal
    - pwd ; ls; 
---
- mkdir opt
- cd opt
- git clone http://github.com/tonybutzer/notebook
---

### Don't feel like cloning sheep
---

<img src="https://dolly.roslin.ed.ac.uk/wp-content/uploads/2016/01/Dolly-and-surrogate-mother-768x915.jpg" width=10% style="vertical-align:middle">

<img src="https://dolly.roslin.ed.ac.uk/wp-content/uploads/2016/01/Dolly-and-surrogate-mother-768x915.jpg" width=10% style="vertical-align:middle">


## Just use group login:

- http://10.12.69.233
- harmony
- harmony
---

## Winner Winner Chicken Dinner
- that is all I wanted to get accomplished
- Everything else this week is a bonus!


---
## One on one sessions and jupyter tours available

- just open a chat with tony butzer for custom notebook tour relevant to your technology interests

## If I can Help you to the cloud - just ask
- its free free free - I am funded by OpenDataCube
---
## Rules of Behaviour and IT Security

- its a priviledge to work in a sponsored cloud
- Be Responsible not malicious
- Save the Planet with Science - Please!

- oh and if computer or language things break - use the TEAMS-CHAT - to tonybutzer
---

## How to cheat at Markdown
- Markdown is another zen item in the technology universe.
- below are two simple tables in markdown
- and a great editor for learning markdown in 10 minutes
	- [https://jonschlinkert.github.io/remarkable/demo/](https://jonschlinkert.github.io/remarkable/demo/)
- and as always all you need is a browser
	- We don't need no education
	- We don't need no thought control
	- No dark sarcasm in the classroom
	- Teachers leave them kids alone… -- Pink Floyd --

```
| sign | poet-line |
| ------:| -----------:|
| > | When the Star Belly Sneetches had frankfurter roasts
| > | Or picnics or parties or marshmallow toasts,
| > | They never invited the Plain-Belly Sneetches
| > | They left them out cold, in the dark of the beaches.
| > | They kept them away. 
| > | Never let them come near.
| > | And that’s how they treated them year after year.
| > | -- Dr. Seuss --
```

```
| sign | poet-line |
| ------| -----------|
| > | When the Star Belly Sneetches had frankfurter roasts
| > | Or picnics or parties or marshmallow toasts,
| > | They never invited the Plain-Belly Sneetches
| > | They left them out cold, in the dark of the beaches.
| > | They kept them away.
| > | Never let them come near.
| > | And that’s how they treated them year after year.
| > | -- Dr. Seuss --
```


### https://jonschlinkert.github.io/remarkable/demo/  -- [Clear] - 
- [https://jonschlinkert.github.io/remarkable/demo/](https://jonschlinkert.github.io/remarkable/demo/)
- try the above text in the remarkable wysiwig tool

---


## Science should be done with pandas and xarray

![](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/600px-Pandas_logo.svg.png)

![](http://xarray.pydata.org/en/stable/_static/dataset-diagram-logo.png)

### XARRAY 
- I'm doing science with `xarray`
	- xarray is like the Chicago airport - its not your final destination - but you can get anywhere from there
- everything else in python is just **glue**

## Notebook Drive By 

## Notebooks are:
- like storyboards for the real movie
- teaching vehicle to illustrate code and its outputs
- tool for rapid application development and collaboration
- the on-ramp to exciting panel applications
- a way to quickly teleport to your cloud computer with just a browser - even from the beach

### My best notebook to date
- and i have written hundreds of notebooks

#### [zen](http://10.12.69.233/user/harmony/notebooks/notebook/00-Harmony/02-week2/03-zen.ipynb)

### Xarray Basic - hello xarray
#### [gentle intro to xarray](http://10.12.69.233/user/harmony/notebooks/notebook/00-Harmony/02-week2/01-gentle-intro-to-XARRAY.ipynb)


### A word on public data assets
- public - that sounds nice
- planet really pushed this pangeo world - thanks planet
- [https://registry.opendata.aws/landsat-8/](https://registry.opendata.aws/landsat-8/)
### Notebook illustrates Pangeo, Xarray, Public Data Assets and Panda
- this notebook was featured by tony butzer at AR19
- the point is that when we move the Scientist to the data
	- everyone wins because so much more science and collaboration can be done
- Can xarray, pangeo and python help automate change detection pipelines for tree regrowth for Dr. Zhou?
- 

#### [pine-lake](http://10.12.69.233/user/harmony/notebooks/notebook/01-Everything-but-harmony/10-DEMO-lite-stac-xarray-all-sandbox/000-demo-pine-lake.ipynb)




## Jupyter Roles/Features/Capabilities
- text editor
- python coding and exploring
- teaching/collaborating tool - commands and output in the same place - writes text books as you go
- file transfer agent - upload and download files 
- web app development accelerator - panel package
- teleports people with a simple browser right inside their free computer
- AWS onboarding enabler - view the cloud - see the grand canyon without getting hurt
- terminal and bash access
- poor man's powerpoint tool
- and for `Science` - well that is what **jup** was **born for** - for those that realize it anyway
- ... and so much more ...  "A lot of people say this Jupyter thing is going to be huge -- its fantastic! -- who knew?" 


---
## END OF WEEK2

### Thank You Everyone

- i will sort out week 3 now!
---




2. WEEK THREE - Delaware River Basin AOI
	- https://panel.holoviz.org/reference/widgets/FileDownload.html
	- How to display AOI in Jupyter
		- geojson and shapefile
		- folium
- docker 
```
FROM developmentseed/geolambda:full
WORKDIR /home/geolambda
```

## Final Projects
https://earth-env-data-science.github.io/projects.html

## Rich Signell Influence, Experience and Why Cloud

Tony, I discovered something by Accident today.   If you add use "panel" as your urlpath in binder, it displays all your notebooks with Panel as apps.    Check out the last binder link here: 
https://github.com/reproducible-notebooks/Holoviz-Demos#holoviz-demos

[Yesterday 4:22 PM] Signell, Richard P
    Ooh this is cool too!    https://edu.oggm.org/en/latest/explorer.html

[Yesterday 12:44 PM] Signell, Richard P
    Tony, check out Ryan's book! https://earth-env-data-science.github.io/intro
​[Yesterday 12:44 PM] Signell, Richard P
    It's not really a book.   It's actually a course.  He describes how he "onboards" folks to Pangeo (essentially)
Edited​[Yesterday 12:44 PM] Signell, Richard P
    Look at the menu on the left 
​[Yesterday 12:45 PM] Signell, Richard P
    And then look at the Capstone project list: https://earth-env-data-science.github.io/projects.html
​[Yesterday 12:47 PM] Signell, Richard P
    This came up in the discussion here: https://github.com/pangeo-data/jupyter-earth/issues/11#issuecomment-740059579
A curated list of learning resources  · Issue #11 · pangeo-data/jupyter-earthFollowing up from the EarthCube meeting on Sept 10, one item that came to light was that it would be valuable to have a curated / opinionated list of learning resources to onboard scientists to the...github.com​[Yesterday 12:47 PM] Butzer, Tony (Contractor)
    that sounds perfect - this 2nd mouse approach feels nice
​[Yesterday 12:47 PM] Signell, Richard P
    I love that the students all did projects using the tools and have binder links!
​[Yesterday 12:48 PM] Butzer, Tony (Contractor)
    Neal Pastick is already a pangeo zealot - got is aws space today!
​[Yesterday 12:48 PM] Butzer, Tony (Contractor)
    we will be talking to neal - you will be a consultant on our data wrangling pipeline
​[Yesterday 12:53 PM] Signell, Richard P
    Sounds good!



2. LAB
3. Organizing our DATA Inputs in the Cloud
	- Fundamentals of S3
	- S3 is an object store
		- mostly not a big deal - but sometimes ...
	- Data Wrangling
	- Slow Data Transfers
		- ssh and scp
	- VPN do's and dont's 
3. LAB

---

## Project Initiation, Kickoff, and Approach

- Jump in with both feet approach.
- Gabriel Senay, Steffi Kagone - trail blazers
- Neal Pastick as trail blazer
- Continuous Training - Train The trainer
    - Example Steffi and Gabe Parish now writing visualizations directly

## Cloud Immersion Concept

### Use the cloud for EVERYTHING
- website
- kanban
- jupyter hub  - mini-pangeos
- all your data storage
    - move from clunky Netapps and archaic windows storage architectures
- leverage others work
- collaborate like hell

## Why

### For selfish reasons

- Impress your friends
- looks nice on the resume
- its more fun
- you don't have to deal with people you don't like

### Headlines

- Netflix Delivers Billions of Hours of Content Globally by Running on AWS 
- Steffi Kagone does 150 days of work in just THREE!

### Procurement delays not applicable

### Scalability

### USGS/DOI Efficiencies
- Remember DCOI threats
- Remember Cloud First
- Used to be mandates as a top down push
- Now science customer pull
- cost efficiencies
- It is irresponsible not to use the cloud

### Open Source Advantages
- numerous articles on why open source

### Python Momentum

### My favorite - less data wrangling - MORE SCIENCE

