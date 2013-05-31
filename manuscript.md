What field ecologists can learn from software developers?
=========================================================

Ignasi Bartomeus^1,* ,Vicenç Garcia-Altes^2,** ,...

1 Department of Ecology, Swedish University of Agricultural Sciences, SE-75007 Uppsala, Sweden.
2 Developer Advisor at Plain Concepts, Bilbao, Spain.

*nacho.bartomeus@gmail.com
**vigarcia@plainconcepts.com

Abstract
--------

Introduction
------------

There is not an standardized way of organizing your research because every researcher has its own work flow and because different problems require diffrent working habits. Science requires this flexibility to succeed because we, as scientists, need to integrate in our every day work time for hands-on research, but also for discusion and inspiration. However, there is an increasing pressure to produce more. The need for increasing the scientific production is on debate (e.g. slow science manifesto, TREE papers), and the main claim is that there is a risk to sacrifice quality by quantity. We do not advocate that increasing production is the way forward, but we do propose a set of tools that can help the researcher to keep with the increased production demands, without decreasing quality.

Software developers faced a similar problem, where they were asked to deliver great products in a fast changing world. This need to deliver value in short term without decreasing quality forced the community to develop new ways of organizing their workflow. Hence, in some aspects, they are ahead of us. NEED TO DESCRIBE BRIEFLY AGILE HISTORY/ IDEALS / OBJECTIVES HERE. Vicenç?

Parallel to the quality/quantity trade off, there is also another unresolved tension when doing research, which is less acknowledged. On one hand, science is becoming more collaborative (Neff & Olden 2010, Wuchty et al. 2007), articles are signed by bigger teams, and doing science with broad reaching conclusions requires joint effors from different people. However, on the other hand most research activities like analyzining data and writting articles are still done mainly at the individual level. Collaborators give more or less frequent feedback, but the responsible researcher for a given task works on its own most of the time. This work flow is even more clear when young scientists work with advisors in a jerarquical way. There is long tradition of research done by a leading author, rather than by a team. While both strategies are valid, and have pro's and con's, we feel that when working in a team, ecologists often do not get the most power of teamwork. Software developers also are ahead of us in this area. 

The agile developement movement appears in XXXX with the idea of focusing on the people and not on the process. One of the main goals is the optimization of the communication in complex projects. For example, they realized that projects can not be divided in independent parts done by different people, but that should be build in constant communication. For example, projects where someone does the stats and a second person write the discussion is likely to fail if both persons don't communicate efficiently. A second principle is to work incremntally. Seeing the project as whole, and not as parts helps. For example, instead of first planning the field season, second getting the data and do the analysis, and finally write a paper, would be better to plan the full paper first, which data you need and how will be analyzed while starting the writting the introduction and methods. Then collect the data and check if that this data is what the paper needs, and that the planned stats are still apropiate, then update methods. Third anlyze the results and update and finish the paper. While this seems obvious and is common advice in science introductory courses (I am sure this is explained already somewhere for science, so will be good to cite it.) is not done as often as it should. Agile techniques explained below like retrospectives, can help mantain the incremental work, as well as motivation and comunication among the group.

Here, we propose a series of tools that can be useful for having better workflows. This tools were originally developed to write code, but we aim to apply them to a broader context, hence they should be customized to the researcher needs. Ecology is also becoming more code driven, specially since the spread of R as an statistical tool, we do not cover here how scientists can do better code (see: REF), but how some of this this ideas can be applied to your daily workflow. Not all ideas will fit every reseacrher, and we do not advocate all of them should be used. #this paragraph needs more work#


retrospectives, motivation and comunication
-------------------------------------------
While the lab organization varies a lot among countries, and among people within countries, Lab meetings are common in most labs, and most times are usefull for generating a good environment, however, most labs strugle on how to get the most of this meetings. Scientists ussually try their best and rely on previous experience and common sense, but some tequniques has been proved to work better. (cite alon)

#Vicenç, can you start this part? You are the expert!

#Options of meeting structures: a) focus on questions like Accomplishments since last meeting - Goals for next (#Explain revision and planing of the goals?) b) what I need to do - which help I need - from who- 
#Time boxing
#Lists and GDT? 
#scrum... 


Version control
---------------

Every researcher does in a way or another. Some track how the documents he is working on evolve by adding a date or a number at the end of the document file name. However, my experience, and the experience of many collegues, is that this home-made solutions end up being messy. Software developers have adopted a common protocol for tracking changes, version control. In a nutshell, it allows you to track all the changes you make to your basecode 

The beauty of it is that forces you to document your changes, and hence you can easily go back to older versions. When used in a colaborative way by using a version control server, all collaborators has access to the latest version in real time, avoiding any risk of overwritting, and you can track changes effectively. Moreover, by having a history of your work, it enhance reproductibility and transparency. This is specially important to boost open science movements (Ram 2013).

While originally developed for writting code, you can track field protocols, monitor entire projects, or writte collaborative papers, like I am doing right now with this one (see also other open examples). There are several options researchers can use. The first one is using one of the well known Version Control Systems on the cloud, as github (biggest and good for open science), Bitbucket or Team Foundation Service. These systems, mainly used to control source code, could also be used to track changes in documents, specially if they are plain text documents. You could also use Version Control Systems installed on premise in your data center. Git, Mercurial, Team Foundation Server and Subversion are the main actors. A simplier option, is to use a Document Management System, a software specialized on tracking changes in documents, like GoogleDocs, Confluence or Sharepoint (Check other's: Draft) 


Collective Code Ownership
-------------------------

As mentioned above, scientists are good on having meetings to discuss the working plan, but when it came to analyzing data, or writting the manuscript, they ussually work alone. Similarly, software programmers traditionally code alone. However, some companies have implemented techniques to promote collective code ownership, like pair programming (Williams, Laurie (2001). "Integrating Pair Programming into a Software Development Process" ). The basics are that two people work on the same computer at the same time. One, the driver, writes code while the other, the observer, reviews each line of code as it is typed in. The two programmers switch roles frequently. While reviewing, the observer also considers the strategic direction of the work, coming up with ideas for improvements and likely future problems to address. This frees the driver to focus all of his/her attention on the "tactical" aspects of completing the current task, using the observer as a safety net and guide. (copied from wikipedia)

Despite it can seem a waste of resources, the advantages are clear, being the main one the reduction of errors (Canfora, Gerardo; Aniello Cimitile, Felix Garcia, Mario Piattini, Corrado Aaron Visaggio (2007). "Evaluating performances of pair designing in industry". The Journal of Systems and Software 80 (80): 1317–1327, "Agility counts". The Economist. September 20, 2001..). Fixing those errors a poteriori is more expensive in terms of time and resources invested. Moreover, in science errors are more difficult to spot, as usually the analysis are conducted only once, reducing the chances of catching errors.

We peopose that, in addition to for coding (i.e. many researchers writte at least its own simple simulations code), this can be specially usefull in other stages of the research process. For example, when analyzing results for first time, you aim to get an overwiew of your data. When you do that alone, is easy to lose the focus of your questions (e.g. applying further statistical tests that are apropiate for the data, but not longer apropiate for your original question) and get stuck on getting the details right (e.g. getting the statistical model well specified or ploting some data), however, the figure of an observer that keeps the overall picture in mind, and a driver that concentrates on getting the analysis rigth can speed up the process. Similarly, when starting to write a manuscript, is convinient that someone take care of the overall structure and how ideas flow, while another focus on expresing the idea in the right way. Is important to notice that we see that as a tool to use among equals, for example, among two phd students, or postdocs, rather that a substitution of mentoring, which requires other strategies. 

The overall benefit we see is also by increasing the motivation. Some stages of the scientific process can can be harder to start when working alone, for example, is the well known white page syndrome. By starting this stages in a team, we can find the apropiate support and increase our creativity by building in each others ideas in real time, rather that in a two step process of person A writs a draft first, person B comment on that one later.

20% rule
--------

Academia is well known for its flexibility on designing your research agenda and schedules. That is needed when thinking critically and being creative is part of your job. However, with the presure for publishing, is easy to lose this flexibility. Here we encourage, mirroring big internet companies like google, to spend the 20% of your research time on things not related to your principal research projects (i.e. those manuscrips you plan to write). This suggestion is paradoxiacal with the fact that we aim to increase our productivity/quality ratio, but previous experience shows that from those side projects, where you can be more risky and try new ideas, can be very productive (any ref?). Moreover, this boost your creativity and the learned abilities on this time can be applied to your current research.  

On this time there are plenty of things to do, for example, read about other topic of your interest, colaborate on a crazy idea with someone from other department, write a blog or divulgate science, learn a programming lenguage or new statistical tool (may be attend a webinar), try to apply some of your basic research. All this activities, while not directly building on your current papers are key to your long term career goals.

#Increase diversity communication not within, but among groups. Ideas of having common places and share spaces with other departments...

Conclusions
-----------

#authorship recognition moving to teams (cite tscharanke papaer on acknowledging author contribution)...









