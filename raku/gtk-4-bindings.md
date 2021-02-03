Moving Raku to GTK 4.0
==================================

Description
-----------

Raku has a module called GTK::Simple that binds to a small number of GTk-3 widgets in a Raku-ish manner. GTK-4 has
just been released and the goal is to enhance GTK::Simple to use the GTK-4 libraries. GTK::Simple does not
have all GTK-3 bindings, so the transfer to GTK-4 should be straight-forward.


Expected outcomes
-----------------
- Complete the steps (if any) in the [migration guide](https://developer.gnome.org/gtk4/unstable/gtk-migrating-3-to-4.html)
to prepare `GTK::Simple:api<3>` for `GTK::Simple:api<4>`
- Locate the most uptodate `dll` files for `GTK-3` for Windows, and ensure that `GTK::Simple:api<3>` works in Linux, Windows
and Mac (CI testing environments). Currently only a Linux testing environment is specified. 
- A first draft of `GTK::Simpe:api<4>` that verifies the existence of the gtk-4 libraries, and implements the existing
widgets.
- Stretch goals
  * implement more gtk-4 bindings, perhaps using software to create bindins directly from gtk-4 documentation.
  * implement for Raku a demo program showing the use of available widgets [like gtk-demo](https://developer.gnome.org/gtk4/stable/gtk4-demo.html).


Required skills
---------------

Students will need to be able to read and interpret software documentation, such as the documentation accompanying
GTK-4. This is a vital skill for any good software engineer, and this task will have an educational benefit far
beyond Raku or GTK.

Students will need to have or acquire an understanding of enough C to use Raku's `NativeLibs` 
interface to the GTK-4 library. The process is 
far simpler than in many other languages.

Students will need/acquire an understanding of the Raku language.

Students will need a solid understanding of the OS they use. GTK3 is important in Linux distributions, and GTK4
is still considered experimental. The GTK development documentation states that GTK3 and GTK4 can be both be installed
and run on the same mmachine, though a 'flatpak' installation is recommended.


Rating
------

Medium. Some parts of this task will be easy, some will take quite a lot of time (eg., the GTK libraries are large).


Possible mentors
----------------

Richard Hainsworth, aka finanalyst.  `richard@hainsworth.wales` Currently the maintainer of GTK::Simple.


