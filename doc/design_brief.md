# Sley: Standards and tools for weaving together human subjects data

Sley is a set of conventions and tooling for organizing human subjects data. If you're familiar with BIDS and fmriprep, sley has the same general flavor.

The code in this package will be written in R, unless aspects of it would immensely benefit from being written in other languages. Someday, we may provide python tooling as well. The conventions for sleyed data will apply across implementations, of course.

The author of this package has written 

The target audience for this project is researchers who are actively, personally analyzing data -- graduate students, postdocs, and research assistants. These people will know good research practice, or have excellent guidance on it. Usually, they will _not_ be expert programmers or data curators, nor will they have good guidance on those topics. This project aims to provide a straightforward, easy-to-follow set of conventions to follow to describe the data elements collected in a study and the semantic relationships between them, and provide tools to leverage those relationships in quality checks, data exploration, and visualization.

There are many existing packages that can use these relationships (`psych`, `careless` and such)

Some concrete examples:

To score self-report measures, researchers need to specify which items belong to which measures and factors within those measures, and also (generally) specify which elements in the measure are reverse-scored. Generally, after computing these scores, that information is discarded, even though it be used to check several aspects of data quality. At the single-participant level, you can check for long series of repeated answers or even-odd concurrence; across participants, you can check to ensure your factor structure is what you expect

## On the name

A "sley" (or "reed") refers to the grating on a weaving loom that keeps the long parallel warp threads aligned, and assists in setting each new row of the weft in place while weaving. The process of "sleying" is stringing and tensioning each thread on the loom.

Much like in weaving, not all research needs to, or even should, use sley -- sleyed looms are primarily used in Western traditions focused on producing relatively large amounts of
