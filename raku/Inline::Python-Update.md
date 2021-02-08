Bring Inline::Python up to Inline::Perl5's level

Description
Inline::Python was started shortly after Inline::Perl5 and may in the long run turn out to be the more important of the two.
Nevertheless at some point the author decided that developing both in tandem was slowing down development too much.
He decided to explore in Inline::Perl5 first and when the best way to build a language bridge was found port that to Inline::Python.
Inline::Perl5 now supports almost everything one could expect from it and the architecture works well.
Porting this to Inline::Python is what's missing and what the author doesn't seem to find the time for.

Expected outcomes
Port the architectural advantages of Inline::Perl5 to Inline::Python, most notably the custom meta class that's used to generate wrapper classes on the fly.

Required skills
A reasonable familiarity with Raku and Python and maybe C and an interest in how languages actually work.

Rating
medium

Possible mentors
Stefan Seifert <nine@detonation.org> - the author of Inline::Perl5 and Inline::Python.
