Create a Raku Data Analysis library
========================

Description
-----------

Data science has been the killer application for languages such as
Python and R for some time now. Having a comprehensive data analysis
library that is idiomatic and uses Raku's unique features would really
contribute to its popularity and usability.

Currently there are some partial statistics libraries, as well as
built-in facilities like map/reduce, including parallel versions. But
we need to take this as far as Pandas, if possible.


* Use of specific data strutures such as data frames for processing.
* Reading from a wide spectrum of formats, from CSV and JSON to
  highly specific statistics file formats.
* Handling missing data automatically in data sets.
* Powerful matrix and data frame processing and transformation,
  merging and joining.
* Processing of time series

The student would be expected to

1. Examine available facilities in Raku land for doing this kind of
   thing.
2. Settle in a minimal set of Pandas features that will be ported
3. Advance, milestone by milestone, to an initial release and, if
   possible, a functional release.

Expected outcomes
-----------------

* Contribution to upstream libraries
  like
  [Math::Libgsl::Matrix](https://github.com/frithnanth/raku-Math-Libgsl-Matrix) where needed.
* Version 0.1 with limited functionality released to the ecosystem.
* Competitive speed compared with Pandas or other implementations.


Required skills
---------------

Required or prefered skills the student should have to be able to
tackle this project.

* Some experience with Raku is appreciated, but not really
  needed. Will to learn will be a requisite.
* Experience in C to be able to use NativeCall for C interfacing.
* Experience in data analysis tools, specially Pandas or similar R tools.


Rating
------

Medium.


Possible mentors
----------------

- JJ Merelo (jjmerelo@gmail.com, [GitHub](https://github.com/JJ)),
  jmerelo on Freenode.


