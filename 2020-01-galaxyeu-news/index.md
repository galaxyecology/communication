---
site: freiburg
tags: [galaxy,mmos,devops]
title: Massively Multiplayer Online Science in Galaxy to help Ecologists - a citizen science project.
---

A few years back the general webhook concept was contributed to the Galaxy codebase.
Webhooks have enabled custom modifications to the Galaxy User Interface (UI) without changing the Galaxy source code directly.
It has the advantage that the maintenance of costum changes is a lot easier. You can think about it like a plugin concept for the Galaxy UI.
Webhooks are powering the much loved XKCD or PhD comics that you see when you submit jobs or workflows for example - but this was just the first step ...

Today we are proud to introduce you an extension that enables __you__ to help our ecology community to annotate existing datasets
by classifying hoverflies into male and female.
This information will help ecologist in further data treatment, for example to train future machine learning models.

How it works and how to create new plugins of this kind?

Here we can take the example of the hoverflies:

The [SPIPOLL](https://www.spipoll.org) citizen science project is collecting images from all kind of animals, in our case from
[Episyrphus balteatus](https://en.wikipedia.org/wiki/Episyrphus_balteatus), also called marmalade hoverfly. In a second step a project manager
prepares certain tasks and seeks for community contribution to help classifying the images.
As a first project we have choosen to help with the task to classify ~5000 hoverfly images and identify the sex by looking at relative eyes position.

To make it really simple for __you__ to contribute to such a crowdsourcing project we teamed up with the [Massively Multiplayer Online Science](http://mmos.ch)
project, which is a citizen science platform connecting scientific research and video games! :)
Read more about the [H2020 GAPARS project](http://gapars.mmos.ch).


On the MMOS side, you had to populate the developer portal with pictures and provide all mandatory metadata.
We then had to create the simple webpage that could be embedded into Galaxy. This site displays the task (in our case a small describtion and the hoverfly image)
and allows to submit an answer to the MMOS server.

The hoverfly example can be found on [GitHub](https://github.com/galaxyecology/webhook_SPIPOLL_Flash/blob/master/templates/guess.html).
This is a very simple example, with a single picture displayed as a task, but you can imagine many other possibilities, and not only on pitures!

If you have a task where you need the help of thousands of researchers, talk to us and we will figure out together
if we can treat your data in a similar way as our marmelade flies!

Crowdsourcing in science is hard, nevertheless there are tremandous opportunities where we all can advance science and help our collegues.

Here we are trying to overcome the challenges by embedding the crowdsourcing tasks into Galaxy.
The idea is to provide a simple framework to create and manage tasks and data via the [MMOS platform](http://mmos.ch),
provide a simple UI (https://usegalaxy.eu/gapars-experiment) and integrate this into the [Galaxy Europe](https://usegalaxy.eu).
For us it made a lot of sense to offer the hoverfly images after you execute a job or a workflow. Usually you need to wait a few seconds until your job is
processed and you can study the results. During this time you can now classify marmelade hoverflies as a means to procastinate - but in a very meaningful way and the
good feeling to have helped our collegues from ecology :)

The work done by __you__ with this new Galaxy feature allows ecologist to extend metadata on already captured data
and will open new ways to analyse them. For example by
training machine learning models or taking into account new factors (here the sex of the flies) in statistical modeling.


Have much fun classifying flies and let us know if you have similar use-cases!
Thanks a lot to all contributors, particularly Rémi Planel ([GitHub rplanel](https://github.com/rplanel/)), Héléna Rasche ([GitHub erasche](https://github.com/erasche/)), the MMOS folks and Yvan Le Bras!

This work is a collaborative effort between french national Museum of natural History, UseGalaxy.eu (de.NBI) and the Swiss MMOS company. Thanks also to the H2020 GAPARS project!

If you want to read more about crowdsourcing citizen science data on UseGalaxy.eu have a look at the [new blog post by Yvan](https://galaxyproject.org/blog/2020+++++++++/)! 

    <div class="multiple-img">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/zTne29-GU_E" frameborder="0" allowfullscreen></iframe>
    </div>
