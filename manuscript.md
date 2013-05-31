What ecologists can learn from software developers?
==================================================

Ignasi Bartomeus^1,* Vicenç Garcia-Altes^2,** ...

1 Department of Ecology, Swedish University of Agricultural Sciences, SE-75007 Uppsala, Sweden.
2 Developer Advisor at Plain Concepts, Bilbao, Spain.

*nacho.bartomeus@gmail.com
**vigarcia@plainconcepts.com

Introduction
------------

There is not an standardized way of organizing your research because every researcher has its own work flow and because different problems require diffrent working habits. Science requires this flexibility to succeed because we, as scientists, need to integrate in our every day work time for hands-on research, but also for discusion and inspiration. However, there is an increasing pressure to produce more, and burocracy can consume a lot of time that is not dedicated to conduct science. The need for increasing the scientific production is on debate (e.g. slow science manifesto, TREE), and the main claim is that there is a risk to sacrifice quality by quantity, we do not advocate that increasing production is the way forward, but we do propose a set of tools that can help the researcher to keep with the increased production demands, without decreasing quality.

Software developers faced a similar problem, where they were asked to deliver great products in a fast changing world. This need to deliver value in short term without decreasing quality forced the community to develop new ways of organizing the workflow. Hence, in some aspects, they are ahead of us. 

Parallel to the quality/quantity trade off, there is also another unresolved tension when doing research, which is less acknowledged. On one hand, science is becoming more collaborative (Neff & Olden 2010, Wuchty et al. 2007), articles are signed by bigger teams, and doing big science with broad reaching conclusions requires joint effors from different teams. However, on the other hand most research activities like analyzining data and writting articles are still done mainly at the individual level. Collaborators give more or less frequent feedback, but the responsible researcher for a given task works on its own most of the time. This work flow is even more clear when young scientists work with advisors in a jerarquical way. There is long tradition of research done by a leading author, rather than by a team. While both strategies are valid, and have pro's and con's, we feel that when working in a team, ecologists often do not get the most power of teamwork. Software developers also are ahead of us in this area. 

Here, we propose a series of tools that can be useful for having better workflows. This tools were originally developed to write code, but we aim to apply them to a broader context, hence they should be customized to the researcher needs. Ecology is also becoming more code driven, specially since the spread of R as an statistical tool, we do not cover here how scientists can do better code (see: REF), but how some of this this ideas can be applied to your daily workflow. Not all ideas will fit every reseacrher, and we do not advocate all of them should be used. #this paragraph needs more work#

Version control
---------------

Every researcher does in a way or another some tracking of how the documents he is working on evolve. However, my experience, and the experience of many collegues, is that this home-made solutions end up being messy. Software developers have adopted a common protocol for tracking changes, version control. In a nutshell, it allows you to track all the changes you make to your basecode 

The beauty of it is that forces you to document your changes, and hence you can easily go back to older versions. When used in a colaborative way by using a version control server, all collaborators has access to the latest version in real time, avoiding any risk of overwritting, and you can track changes effectively. Moreover, by having a history of your work, it enhance reproductibility and transparency. This is specially important to boost open science movements (REF).

While originally developed for writting code, you can track field protocols, monitor entire projects, or writte collaborative papers, like I am doing right now with this one (see also Tim for an open example). There are several options researchers can use. The first one is using one of the well known Version Control Systems on the cloud, as github (biggest and good for open science), Bitbucket or Team Foundation Service. These systems, mainly used to control source code, could also be used to track changes in documents, specially if they are plain text documents. You could also use Version Control Systems installed on premise in your data center. Git, Mercurial, Team Foundation Server and Subversion are the main actors. The last option is to use a Document Management System, a software specialized on tracking changes in documents, like GoogleDocs, Confluence or Sharepoint (n'hauriem de buscar més, sobretot de gratuits) 

Pair programing -> ho podriem canviar a Collective Code Ownership
----------------

As mentioned above, scientists are good on having meetings to discuss the working plan, but when it came to analyzing data, or writting the manuscript, they ussually work alone. Similarly, software programmers traditionally code alone. However, some companies have implemented techniques to promote collective code ownership, like pair programming (Williams, Laurie (2001). "Integrating Pair Programming into a Software Development Process" ). The basics are that two people work on the same computer at the same time. One, the driver, writes code while the other, the observer, reviews each line of code as it is typed in. The two programmers switch roles frequently. While reviewing, the observer also considers the strategic direction of the work, coming up with ideas for improvements and likely future problems to address. This frees the driver to focus all of his/her attention on the "tactical" aspects of completing the current task, using the observer as a safety net and guide. (Extret de la wikipedia a pelo)

Despite it can seem a waste of resources, the advantages are clear, being the main one the reduction of errors (Canfora, Gerardo; Aniello Cimitile, Felix Garcia, Mario Piattini, Corrado Aaron Visaggio (2007). "Evaluating performances of pair designing in industry". The Journal of Systems and Software 80 (80): 1317–1327, "Agility counts". The Economist. September 20, 2001..). Fixing those errors a poteriori is more expensive in terms of time and resources invested. Moreover, in science errors are more difficult to spot, as usually the analysis are conducted only once, reducing the chances of catching errors.

We peopose that, in addition to for coding (e.g. many researchers writte at least its own simple simulations), this can be specially usefull in other stages of the research process. For example, when analyzing results for first time, you aim to get an overwiew of your data. When you do that alone, is easy to lose the focus of your questions and get stuck on getting the details right (e.g. ploting or applying further statistical tests that are apropiate for the data, but not longer apropiate for your original question), however, the figure of an observer that keeps the overall picture in mind, and a driver that concentrates on getting the analysis rigth can speed up the process. Similarly, when starting to write a manuscript, is convinient that someone take care of the overall structure and how ideas flow, while another focus on expresing the idea in the right way. Is important to notice that we see that as a tool to use among equals, for example, among two phd students, or postdocs, rather that a substitution of mentoring, which requires other strategies.

The overall benefit we see is also by increasing the motivation, which can be harder to find when working alone, and by increase creativity by building in each others ideas in real time, rather that in a two step process and avoid the white page syndrome (also applicable to analysis)

20% rule
--------

Academia is well known for its flexibility on designing your research agenda and schedules. That is needed when thinking critically and being creative is part of your job. However, with the presure for publishing, is easy to lose this flexibility. Here we encourage, mirroring big internet companies like google, to spend the 20% of your research time on things not related to your principal research projects (i.e. those manuscrips you plan to write). This suggestion is paradoxiacal with the fact that we aim to increase our productivity/quality ratio, but previous experience shows that from those side projects, where you can be more risky and try new ideas, can be very productive (any ref?). Moreover, this boost your creativity and the learned abilities on this time can be applied to your current research.  

On this time there are plenty of things to do, for example, read about other topic, colaborate on a crazy idea with someone from other department, write a blog or divulgate science, learn a programming lenguage or new statistical tool, try to apply some of your basic research... For example, Jeremy Fox recently published a TREE paper (REF) from what originally was a blog post. Or the rOpenScience team worked that way and end up publishing and uploading to CRAN R packages to access data (REF). 

Agile development?
-----------------
(this secction is very blurry, but I wanted to deliver the full story, we will make this section grow on next iteration)

Finally, while the lab organization varies a lot among countries, and among people within countries, we also want to cover some tools that are already more or less applied, but that have been show to increase efficiancy. For example, Lab meetings are common in most labs, and most times are usefull for generating a good environment, however, most labs I've been strugle on how to get the most of this meetings. Scientists ussually try their best and rely on previous experience and common sense, but some tequniques has been proved to work better. #Explain revision and planing of the goals? Lists and GDT?

#Agile: There are many software programming schools with different idearies, but we take the agile manifesto as an example, the basics of them is to focus on the people and not on the process and work incremntally. That imply optimization of the communication.

#Work incremental: Explain how seeing the project as whole, and not as parts help? For example, instead of planning the fiels season, getting the data, and the doing analysis, and then write a paper. plan the paper and field season, and start the writting and think on which stats will be done, collect the data and check that this data is what the paper needs, and that stats are apropiate, update methods, then anlyze the results, update and finish the paper...? this is explained already somewhere for science, so will be good to cite it.

#Increase diversity communication not within, but among groups. Ideas of having common places and share spaces with other departments...


#quines idees hem deixo? que es podria afegir?

Una opció seria explicar després de la introducció que és el desenvolupament àgil i quin sentit té. Com ajuda a la realització de projectes complexes. I després podriem pensar en tècniques que poden tenir sentit a la ciència. De fet el pair programming és una tècnica àgil. La més clara és la que comentes del work incremental. Hi ha d'altres que són potser massa tècniques (Test Driven Development) i les altres seríen d'interaccions entre persones (retrospectives, motivació, comunicació, etc). Com ho veus?

#Note to self: cite alon!












