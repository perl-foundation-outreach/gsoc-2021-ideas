# Raku Module Chain Introspection

## Description
Raku manages installed modules in a unique manner. The Raku compiler at compilation time is provided a variable `$*REPO` which contains a LINKED LIST of repositories in which the modules that have been locally installed have been stored. It is possible for a developer to manipulate the linked list and so ensure that only specific modules (or versions of them) are used to compile a Raku program, even though the local system may contain multiple versions of a module.

One common way to manipulate the linked list is to use the -I option provided to the compiler, eg `-I lib`. In this case, 'lib' is the first repository that is searched.

When the Raku compiler requires a module (via a 'use', 'need', or 'require' statement), it will search the linked list for the first instance of the module, and then stop searching when a match is found.

## Expected Outcome

What is needed is a tool, eg, **rakumods** that can do the following:

1. list all the modules that would be found by Raku using a specific incantation. eg. `rakumods -Ilib -I../old_mods/lib --use *`.  
The -I values are what would be provided to raku. In addition, rakumods would need to use `%*ENV` for locations raku would use to find repositories.  
The `--use` parameter is given a regex.

1. list the first instance of a module in the repository chain that matches a given `use` statement, eg., `rakumods -Ilib --use Pod::To::HTML:ver(0.3+)`
1. list the repository keys, not the names, of modules, eg., `rakumods -Ilib --use Pod::To::HTML --keys`
1. output the pod tree from the module(s) in the specified repository chain, eg., `rakumods -I lib --use Pod* --pod`

This tool is needed in order to give a developer information about the specific modules in a chain. When multiple modules are installed, an inconsistency may occur because a newer module is being accessed by the compiler.

In addition, a developer may want Pod information about the functions/methods/classes installed locally. This is currently not easily accessible from the command line.

## Required skills
1. Code in Raku
1. Read the documentation in POD form in Raku core modules (not everything in the CompUnit chain is reflected in the Raku official documentation)
1. Create unit tests

## Rating
This is a medium hard project. The coding and algorithms will be simple. Most of the difficulty will be in assembling an undertanding of the Respository management system from existing core modules.

## Mentors
JJ Merelo, Richard Hainsworth (rnhainsworth@gmail.com)
