Create a Raku implementation of a gRPC client
========================

Description
-----------

[gRPC](https://grpc.io/) is a protocol that's used extensively, by itself or as part of
services such as [etcd](https://etcd.io). For the time being, there's no Raku module that
offers a high-level interface to it.

In this project, the student would be expected to create and release
to the Raku ecosystem a gRPC module, along with example on how to work
with it. There are many possible ways to implement a library,
including
using [NativeCall](https://docs.raku.org/language/nativecall), which
can bind to external libraries.

The student would be expected to:

1. Study different implementations of gRPC client to come up with a
   implementation strategy.
2. Create a library that's able to perform basic gRPC functions.
3. As a bonus, create client libraries for some services such as gRPC
   that work with it.

Expected outcomes
-----------------

* Functional version 0.1 released to the ecosystem.
* Examples included with the distribution on how to use it for
  interfacing with different services.
* If possible, stubs for downstream libraries that can be used easily
  or expanded.


Required skills
---------------

Required or prefered skills the student should have to be able to
tackle this project.

* Some experience with Raku is appreciated, but not really
  needed. Will to learn will be a requisite.
* Experience in C to be able to use NativeCall for C interfacing, in
  case an adaptation of an already existing C module would be the way
  to go.


Rating
------

Medium.


Possible mentors
----------------

- JJ Merelo (jjmerelo@gmail.com, [GitHub](https://github.com/JJ)),
  jmerelo on Freenode.
- Donald Hunter (donald.hunter@gmail.com, [GitHub](https://github.com/donaldh)),
  donaldh on Freenode.

