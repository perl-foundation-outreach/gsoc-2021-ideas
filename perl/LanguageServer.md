Perl::LanguageServer
====================

Description
-----------

This is a Language Server and Debug Protocol Adapter for Perl

It implements the Language Server Protocol which provides
syntax-checking, symbol search, etc. Perl to various editors, for
example Visual Stuido Code or Atom.
(https://microsoft.github.io/language-server-protocol/specifications/specification-current/)

It also implements the debug adapater protocol for debugging Perl code
(https://microsoft.github.io/debug-adapter-protocol/specification)

Expected outcomes
-----------------
* Documenation improvements:
 * docs for beginners and usage examples
 * how to use Perl::LanguageServer with different Editors/IDEs (Vim, Emacs, Atom, Eclipse, ...)
* Testing
* Implementation of missing LanguageServer features:
  * Call hierarchy (https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_prepareCallHierarchy)
  * Auto completion (https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_completion)
  * Hover: function help and signature help (https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocument_hover)
  * Display of help from perldocs for statements, special variables and modules
* Improvements/fixes for the debugger
  * Variable display (currently not all expressions can be displayed)
  * Exception breakpoints
  * Data breakpoints

Required skills
---------------
* Good Knowledge of Perl
* Knowledge of AnyEvent, Coro, Moose and Perl debugger are helpfull

Rating
------
medium to high

Possible mentors
----------------
* Gerald Richter (richter@ecos.de)
* Andrew Solomon (andrew@geekuni.com)
