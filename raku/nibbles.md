Small and big bytes
===================

Description
-----------

Raku has been specced in the past to have support for 1-bit, 2-bit and 4-bit native unsigned integers, and associated arrays.  Alas, this has never been implemented.  For certain memory hungry applications, it would be very useful to have support for these, e.g. for bitmaps in graphics processing.  On the other end of the spectrum, there are application libraries that require 128-bit native integers.  It would be nice to have either end of this spectrum supported by MoarVM.

Expected outcomes
-----------------

Being able to use native 1-bit, 2-bit and 4-bit values and arrays.


Required skills
---------------

This would require C-programming skills.

Rating
------

I think this is a hard project, as it would require deep internals MoarVM knowledge and knowledge of numeric standards and knowledge of how this is supported on the various hardware (specifically with regards to JIT support).

Possible mentors
----------------

Elizabeth Mattijsen, Jonathan Worthington, Daniel Green.
