# Instructor notes

## General remarks

This course was run multiple times by us - the authors and at least once by an external group of teachers (who has not been trained by us).

We are fairly confident that this course "works" and the exercises have been valued as good or excellent.

This course was designed during COVID-19 pandemic for an online delivery.
We heavily depend on the online setting, ie. video call with breakout rooms, the ether pads for collaborative writing. 
We are not sure if this course in its current form would work in real-world workshop. For one there is will an significant overhead in starting group activities (people need to move around etc).
Unlike speaking up, the pads allows multiple student provide answers and suggestion in the same time. 

We delivered the training as 4 x 4 hours modules. The last day has at least one hour breathing space which we reserve for "project clinic" - discussing needs of individual projects 
and a short episode dedicated available resources at the UoE.
It means that there is possibility to add additional episode(s) or taking more time for the existing ones (for example to allow more time in the breakout rooms). 

The instructor folders contains the slide decks for the delivery, which works better than scrolling through carpentry website.
There are also set of word documents with content of the etherpad with the exercises for the student. 
They are bundled into "days". 

We tried to order the episodes in logical sequence, but they can be shuffled around.
The first day is probably the most intense. We typically stop the delivery 15 minutes before the allocated time (even if still we are in the middle of the episode). 
It gives student time to give sensible feedback and the course does not feel rushed.
The left over of the episode are continuing on the next day. It is typically Being precise episode which we split between ORCID and Ontology. 

There is also an option to move IP and Openness to the last day.

### Breakout rooms

Generally, students asked for more time in the group activities in their feedback forms. 
We typically give 5 minutes for the breakout rooms. While it may feel too short for an "active" group, it feels long for not so "engaged" one. So it is a balance. 
Also, we make sure to discuss the groups' answers so more time in the rooms will extend the episodes duration.

The groups should be about 5-7 participants if possible, that should guarantee sufficient level of engaged students in each group (despite our effort some students remain muted all the workshop).
We used zoom for the delivery and could see in the breakout room dialog who has muted mic and camera off and active speakers.
We tried to move participants between groups if one turned too particularly quiet.
We also send broadcast messages encouraging switiching mic etc.

### Etherpads

In our experience, students are more inclined to write down their answers, comments and suggestions than speaking up. So the "discussion" challenges are moved into the pad and we ask to write answers commenting on them.

For the True/False quizes, selecting correct answers we typically start talking over the exercise when we notice than first students are finishing the given exercise. 
It makes the course more dinamic, while we expect our audience accustomed to multitasking such as listening while completing a test.

The quiz like test (true/false, agree, select) are an excuse to comment on the answers. Always if there are some wrong answers, but, also to stress out the most important aspects of the topic.

For the end of episode quiz, we tend to ask students to complete them during the break and after the break comment only on "wrong" answers.

## Specifics for each episode

### 1. Welcome

You can start breakout rooms so students can introduce themselves in the groups.

### 2. Introduction to Open Science

When presenting Open Access explain what other "benefits" it brought with it (apart from costs free access). For example, the time save in trips to libraries or asking inter-libraries loans. 
That should act as an example for the 

Exercise 1. Benefits of openness

Here you should have at least two groups One for Open Data and one Open Software.
Comment on student answers, fill the gaps if some aspect are missing, for example publishing negative results for Open Data. Learning by example for Open Software.

Exercise 2. Personal benefits of being “open”

Answers will tend to cluster, you can comment on that. 
We talk about the typically overlooked: *"•	distinguish yourself from the crowd"*, as in the current "transition" period having those skills can still make a difference as all job/grants/fellowship competitors would have typically have good academic record. Open practices can be this one extra point.

The IP part can be skipped if the IP episode is planned on the same day.

### 3. Being FAIR

Exercise 1. Impossible ...

We give some teams a) the Impossible protocol and some b) the Imposible Average.
Those two work the best. 
We said that it is going to be a race who can get the answers first.
We warn there is no time to read the full manuscript, nor it is how we "typically look for data and protocols".

Sometimes there are answers to 1a. For the average in 5-7 minutes it is rather unlikely. 
We then explain what was the problem with 1a and demonstrate the problem with 1b. 
Show the tables with meaningless headers, say how to get the right column.
Then copy from from pdf to excel the table to show hot it gets scrambled.

That scrambling depends in what program the pdf was oppended. We recommend firefox or bing as they usually do not copy nicely (Acrobat does much better job). Foreing localales also can messad up with copying.

Exercise 2. FAIR Example

Typically some answers for I or R end up in A. 
You should do quick demo of the zenodo record and highlith the most important part (or point to them using the students answers)

Exercise 3. FAIR and You

We only once got the right answers. 
Always worth going back to Zenod and show: *Accessible - Trackable and countable*
as the views and downloads, mention the new metrics. 



### 4. IP and Openness

Exercise 1. Checking common licence:

Try to make it code-along exercise, clicking through the licence text and make the point (but give students the head start).

### 5. Intro to metadata

Use the life demo of omero records to show different kind of metadata rather than slides.

When talking about Minimal Inf, show the fairsharing.org collection.
Mention it is a good resource to find all the standards and repos for FAIR.

Exercise 3. What to include

Start by typing the title and the purpose.
you can ask people to think first of the C. elegans image and what should be added there, so start with domain specific ie microscopy, then go general.
You need to add the crucial metadata elements if student did not think about them, for example genotype, tissue type , generally sample description, some experimental conditions


### 6. Being precise

We demo of ORCID by clicking from the paper via ORCID to the list of authors publication.

The ontology section apart from explaining in slides should be code-along/demo of navigation from bioportals to ontologies, explaining the elements of the terms records, show synonyms, class mapping and visualizations.

### 7. (Meta)data in Excel

Show what happens when saved as text (there are also merged cells which messed up row, date change, not only lost of color).

### 8. Laboratory Records

We use benchling as:
- we have nice real notebooks to show
- we know it
- it has wow effect and tends to attract new users no problem.

But the exercises could be easily adopted to any other ELN.

Apart from the exercise 1, the rest should code-along experience when instructor perfoms all the operations explaining where to click, what is being shown etc.

The aim is not to teach Benchling per say, but to show how easy is to:
- reuse
- follow provenance

Protocols.io give doi and offer forks plus who used our protocol. It can also be demonstrated during the life demo.

### 9. Files organisation

This notepad must be reformatted online before the class. The file/directory names should in mono-space so they align nicely. 
That is being lost during copying from word.

Exercise 1.
The aim is to show how sorting helps finding info unless the naming convention messes up with the sorting.

Exercise 4: Typical folder organizations

The webpage contains our answer to this exercise. The wet projects typically do not get good answers.

### 10. Reusable analysis

We just start jupyter from the network directory on the server and pass the link to students. We asked them first to make a copy of the notebook (the notebook is readonly), that creates some race condition but after a while student have their own copy.

More fancy setup is possible but that was good enough.

That is code-along episode with instructor performing the tasks together with the students.

Before the exercises the instructor should walk through the notebook elements and explain why it is good fot the analysis.

In case the group contains advanced users, ask them to illustrate all variables on the graphic. R offers much more than just multipane graphic, a novel visualisations are possible.

### 11. Version Control

Exercise 3: Changelog in action

We have two examples of real repositories to look at. 
Before the exercise instructor should explain the github screen, which are the entries, how to see what files were changed etc.

Then after exercises instructor should show more features of github:
- navigate back in the history
- markdown
- contributors page with commits stats, user home page with they output.

We use this course repo as the demo of contributions as it has easy to explain burst of activities. 

### 12. Templates for consistency

Ideally it should be the last episode on the 3rd day.
We ask students for feedback and then we do the exercise, that way they can stay and work on templates after the course allocated time. Templates need 20-30 minutes time. If it is too late than it needs to be moved to the next day. 

You need to provide a shared file/directory for students to work on templates.

Then on the next day we give feedback.
If the 2nd day worked well, than the excel template should adhere to the good practices in headers naming etc.

Typical issues which can be comment on:
- in excel table, multi values entry eg authors in one cell with ',' rather then in row of cells (so not authors parsing is necessary)
- lack of cleer rule how to distinguish between keys and values
- lack of obvious fields, like names, title, experiment ref, date

### 13. Public repositories

Instructor should click through the appropriate repository records when discussing the students answers.

Exercise 2: Dataset discovery
- after student assessment try, clicking into keyword
that gives nothing, comment on it.

The search for "neuromuscular junction", if you scroll down you will find exotic hits like

*Surveys of Forest Birds on Puerto Rico, 2015*

Exercise 3: Domain specific repositories.

You may try to assing domain to room and let the studens chooce room for a group activity.
Or you ask students to keep typing their anwers working on their own.

At some instructor should demonstrate some of the features of all the repos which are being evaluated, so the other students also see them. Either using the students answer of showing one of the instructor "favourite" feature of each repo.

Exercise 4: Finding a repository

When discussing answers show how FAIR sharing fails for omics type with too many hits and why the curated lists from funders and journals are good place to start.

### 14. It's all about planning

Practical exercise, at least 20 minutes before break, encourage working during the break, sometimes needs 10 minutes more. 
Students should have access to a shared document so they can write simultanously.

After the break the groups switch DMPs and evaluate other work. 
Worth stressing up what reviewers should pick up (like non sensible copy pasting).
While students evaluate instructors should check DMPs themselves and pick up the points worth commenting/ prizing, correcting.

