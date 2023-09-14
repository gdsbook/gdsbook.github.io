---
layout: post
title: "Overview"
categories: bookupdate
author: "Dani Arribas-Bel"
meta: ["Announcement"]
---

Today, Dani gave an overview of the book to the [Geographic Data Science Lab](2023-06-16-liftoff.md), including the motivation for writing it, its contents, and even a live demo. You can watch the talk/demo at:

<iframe width="560" height="315" src="https://www.youtube.com/embed/2Qxaf0xQJiY?si=fxooRASYmkCDk297" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
 
Part of the entertainment of this video is watching Dani running the book, live on Teams, from his iPad, and through Jupyter Lab _and_ Rstudio. It is (mostly) a success. If you too would like to run the book on your own machine, as Dani does in the video, here're some tips.

The trick to getting it all to work is [Docker](https://docker.com). As we argue in [Chapter 2](https://geographicdata.science/book/notebooks/02_geospatial_computational_environment.html), building transferrable platforms that can support open science is non-trivial, but critical. To that end (and leveraging Dani's [GDSenv](https://darribas.org/gds_env/), our book can run on the GDS Docker image, [`v9.0`](https://github.com/darribas/gds_env/releases/tag/v9.0). This is the platform you use, for example, when you run our book on Binder, and you can also run it locally on your machine, without the need of internet connectivity. To learn how to run the book on your own machine, we've got you covered: Chapter 2 has a [section](https://geographicdata.science/book/notebooks/02_geospatial_computational_environment.html#running-the-book-in-a-container) exactly on that!

**NOTE** - The only update you will need to apply form the chapter is the
version of the container you will use. We currently specify version `7.0`, but
the officially supported image is now `9.0`.

At the [end of the talk](https://youtu.be/2Qxaf0xQJiY?feature=shared&t=2023), Dani also runs the book from RStudio (!). This is also supported through Docker and a small toy project of Dani, [`gdsrpy`](https://github.com/GDSL-UL/gdsr). This container runs on top of the fantastic [Rocker](https://rocker-project.org/) project, so you can use those instructions to get it up and running. 

In short, you need to download the image:

> `docker pull darribas/gdsrpy:2.0`

And run it from your machine:

> `docker run --rm -ti -e PASSWORD=<your password> -v /folder/to/mount:/home/rstudio/work -p 8787:8787 gdsrpy:2.0`

Ideally, you want `/folder/to/mount/` to contain a copy of the book, which you
can download from [here](https://github.com/gdsbook/book/archive/refs/heads/master.zip) thanks to Github.

Happy hacking!