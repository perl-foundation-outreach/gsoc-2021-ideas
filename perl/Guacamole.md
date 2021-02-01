Supporting Pluggable Grammers with Guacamole
============================================

Description
-----------

[Guacamole](https://github.com/xsawyerx/guacamole) is a parser toolkit for Standard Perl. It provides fully static BNF-based parsing capability to a reasonable subset of Perl.  It includes a parser, deparser, linter, and syntax check of [Standard Perl](https://metacpan.org/pod/standard).

In this task, you will provide an ability to extend the default syntax that Gaucamole has to support additional syntax.

Example of such pluggable grammars:

* Dios
* Moose
* Dancer2

Expected outcomes
-----------------

Guacamole uses a BNF that needs to be decoupled into multiple parts:

* Preample
* Types of keywords
    * Nullable keywords
    * Unary keywords
    * List keywords
    * Assign keywords

Then we need syntax to allow people to add their own keywords based on the types listed above. Having syntax for inlined BNF would be useful along with code that will generate BNF.

```perl
package Guacamole::Grammar::Moose;
# ...
use Guacamole::Grammar;

Guacamole::Grammar::add_unary_keyword(
    'bnf' => '...',
);

# or
Guacamole::Grammar::add_list_keyword(
    'name' => 'OpHasKeyword',
    'args' => [
        qw< OpKeywordAbs OpUnaryKeywordArg >,
    ],
);

# or maybe
Guacamole::Grammar::add_list_keywords({
    'OpHasKeyword' => [
        qw< OpKeywordAbs OpUnaryKeywordArg >,
    ],
});
```

Users need a simple mechanism for turning on additional pluggable syntax. For example:

```perl
my $guacamole = Guacamole->new(
    'with' => [ 'Moose', ... ],
);

# with standard
use standard (
    'with' => [ qw< Moose ... > ],
);
```

Introspection (viewing the complete BNF, user BNF, extension-based BNF like Moose or Dios, etc.) would be very useful.

Required skills
---------------

* Knowledge of BNF
* Knowledge of Perl syntax

Rating
------

Medium.

Possible mentors
----------------

* Sawyer X (xsawyerx AT cpan DOT org, [GitHub](https://github.com/xsawyerx), [@PerlSawyer](https://twitter.com/PerlSawyer)).

