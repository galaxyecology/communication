    Few days after the *[Crowdsourcing citizen science data on usegalaxy.eu Galaxy hub blog post!](https://galaxyproject.org/blog/2020+++++++++/)* it's a pleasure to go deeper on the gamification orientation of this work done in a collaborative effort between french national Museum of natural History, usegalaxy.eu german team and Swiss MMOS company thanks to the H2020 GAPARS project!
    we introduced the general webhook concept a few years back into galaxy
    this has enabled custom modifications to Galaxy UI without changing Galaxy source code and make maintenance of those changes easier. It is a plugin concept for Galaxy UI.
    this is what is powering the much loved XKCD or PhD comics for example - but this was just the first step ...
    Today we are proud to introduce you an extension that helps our ecology community to annotate existing datasets classifying hoverflies into male and female so this information can be used in further data treatment for example to train future machine learning models.
    How it works and how to create new plugins of this kind? 
        Here we can take the hoverflies example:
        pictures collected by SPIPOLL citizen scientists are uploaded in the SPIPOLL database. Project managers have prepared these pictures describing tasks that can be done on one subpart of the pictures, here hoverflies pictures (5000) where we can potentially easily identify male and female looking at relative eyes position. 
        description of pictures batchs, tasks and gold standards (subpart of the 5000 pictures where the result (male or female) is known) as manner to get the data was send to MMOS
        On the MMOS side, you have to populate the developer portal with pictures and provide all mandatory metadata
        You then have to create the "web page" (have a look here for the hoverflies example https://github.com/galaxyecology/webhook_SPIPOLL_Flash/blob/master/templates/guess.html) who will populate the Galaxy webhook, display the picture (the task) and allow to submit an answer. 
            Here is a simple example, with a single picture displayed by task, but you can imagine many other possibilities, and not only on pitures!
            You have thousands (or more) pictures you want to treat through a simple task? You can use this hoverflies example to create your own Galaxy webhook! Please don't hesitate to contact us!
    it is good to help as in citizen science, three important issues regarding notably crowdsourcing related tasks are the fact that 1/very few people contribute to major part of results, 2/majority of contributors treat only few tasks and never come back, 3/opening contributors to others citizen science projects is difficult. Here the idea is to give a quite simple framework to create & manage tasks and data (MMOS platform http://mmos.ch/), have a GUI (web page on a web server, Galaxy webhook https://usegalaxy.eu/gapars-experiment/) and places where can shape the user experience (here the Galaxy Europe platform https://usegalaxy.eu/)
    in the hoverflies example, the work done by Galaxy webhook analysts allow to extend metadata on already captured data and so can open new ways as training machine learning models or taking into account a new factor (here sex) in statistical modeling 
    what next ? 
        Disseminating the hoverflies "app" on others channels than https://usegalaxy.eu/ like ecology oriented website or forum.
        creating others examples to better appreciate costs, limitations and potential of this approach
