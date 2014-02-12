# Simple Open Data

So you want to publish some open data? Cheers! - you're awesome. Here are some
helpful hints to make it simple and effective.

## Goals

Why should you publish open data?

* **Using open methods of sharing can make your organization more efficient internally.** When you pay attention to how data is published, packaged, and managed, it's easier to point other departments to good resources, and easier for them to use those resources.
* **A wider audience means having more creativity and types of talent invested in understanding your data.** The most interesting uses can be unexpected - like cross-referenced studies or visualization projects that bring public attention to the details.

## Use Open Formats

Having a wider audience means changing your expectations for how they'll use data. You might use a particular operating system and software, and even have a site license for software - but others don't, and software can be prohibitively expensive. Why bother making data free if it costs thousands of dollars to open the file?

Luckily there are many simple, open formats that are supported widely, by commercial and free products and across operating systems.

### Text

**Avoid publishing text as Microsoft Word files.** There are multiple incompatible versions of the format and they are read inconsistently outside of Microsoft products.

**Publishing text as PDF is okay.** But remember that some of the purported benefits of PDF are myths: it is easily possible to edit any PDF file, so the files aren't any more tamper-proof than any other format.

If your text is minimally styled, prefer a simple format. **.txt** files are the simplest format possible, and easy to read in any system.

### Tables

**Never publish tabular data as PDF.** It's nearly impossible to read this data with a computer, and so potential users need to do a lot of manual work to parse or re-type the data.

**The best format for publishing table data is [CSV](http://en.wikipedia.org/wiki/Comma-separated_values). CSV stands for 'Comma-separated values', and is an option for Microsoft Excel's exports.

### Geographical Information

Geospatial data formats are different for vector versus raster data, and different formats are better for different sizes of data.

**For small vector data, use [GeoJSON](http://geojson.org/) or [KML](http://developers.google.com/kml/documentation/)**. These are simple, widely-adopted standards. Remember that these formats expect coordinates in the [WGS84](http://en.wikipedia.org/wiki/World_Geodetic_System) datum, which is also easier to use for data consumers, so reproject before publishing.

**For larger vector data, publish as Shapefiles.**

**A good, simple format for distributing raster data is [GeoTIFF](http://en.wikipedia.org/wiki/GeoTIFF).** It's an open standard with many implementations.

Certain Esri data types like FileGDB, `.lyr`, and `.zlas` are intentionally encrypted and only supported by expensive Esri products, so they aren't recommended for open data distribution. Likewise, GeoPDF is not recommended because it's rarely implemented and also has legal restrictions.

## Use Open Licenses

Specifying a license is essential for any kind of distribution: without clear legal terms, nobody can feel safe enough to use data. Which license you choose depends on a number of factors:

If the data is [a work of a Federal government employee as part of their job, it's Public Domain](http://en.wikipedia.org/wiki/Work_of_the_United_States_Government), so there's no choice. Similarly [US laws and other edicts of government](http://en.wikipedia.org/wiki/Edict_of_government) can't be copyrighted.

If your data doesn't fall into one of those conditions, you probably have copyright over it, which means that the rights you grant and those you keep are your choice.

The most liberal option is to declare your work [Public Domain](http://en.wikipedia.org/wiki/Public_domain) or license it under [CC0](http://creativecommons.org/publicdomain/zero/1.0/), an open license that replicates the Public Domain terms for other countries. This gives away most rights, like the right to demand attribution or prevent commercial usage, but it also means that users are less likely to have legal doubts and more likely to use the data.

If you want to require attribution, you can use the [ODC-BY](http://opendatacommons.org/licenses/by/summary/) license, which lets people use your data as long as they credit you as the original source.

There's another type of license with the property of being 'share-alike': this means that combinations of your data with other data need to be shared under the same license as your data. While this alleviates some fears of freeloading on other people's work, it does so at a high cost - share-alike is tricky to define legally and can easily scare off creative uses. Thus it's not recommended to use share-alike licenses like [ODbL](http://opendatacommons.org/licenses/odbl/) for any new projects.

## A Portal? Start Simple

