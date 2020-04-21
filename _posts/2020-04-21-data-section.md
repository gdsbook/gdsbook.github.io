---
layout: post
title: "New Data Section available online"
---

Despite radio silence on this land, the book project continues ahead on full steam. If you are that kind of person, you should check out [our repository](https://github.com/gdsbook/book) for live updates on what we are up to. But if you just want curated, small batch, and more refined updates, this is your place.

Last week, we [added a new section](https://github.com/gdsbook/book/pull/83) to the online site for the book that includes the provenance and code we are writing to create all the datasets we use in the book. In most cases, to be able to show the technical and conceptual points we want in this book in an effective way, we need a streamlined dataset (a "clean" one as it were). This is fine for its convenience and ability to let us get to the point we want to make; but it is also a bit detached from how (geographic) data science is done in the real world. 
The data you need are typically dispersed across the web, in different formats, structures, etc. and taking them into a form and shape that fits your needs is usually more than half the job of analysing it.  

The new "Data" section, available online, will show you what sources we use, but also how we transform them into a usable format. It is not, though, part of the official book; it is more an "online extra". Hence, each notebook does not have the depth, detail and pedagogy we strive for in the book chapters. They are more like entries on a data scientist's diary that record how to reproduce their actions. We believe the code presented may be useful for folks. 

In addition to code and some narrative, each entry includes a direct link to the final dataset prepared for the book, in those cases where a single file is the output. This will make it easier to expose the data and to access them. Coupled with the fact that `geopandas` and `rasterio` support remote read of files, it'll make very easy to pull data for demos and illustrations. We'd love it if folks start adopting the book's datasets for their own applications!

The Data section is available at:

> [https://geographicdata.science/book/data/README.html](https://geographicdata.science/book/data/README.html)

And if you have any comment, feedback, or suggestion, we'd love to hear from you! Please, start the conversation by opening an issue at:

> [https://github.com/gdsbook/book/issues](https://github.com/gdsbook/book/issues)

Happy hacking!