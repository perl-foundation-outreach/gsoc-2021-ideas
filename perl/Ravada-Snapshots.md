Ravada Snapshots
================

Description
-----------

[Ravada](https://ravada.upc.edu) is a Virtual Desktop Infraestructure system.
It is a frontend to [KVM](https://www.linux-kvm.org) and it uses mainly
[libvirt](https://libvirt.org) to manage the virtual entities.

The main goal of Ravada is to provide an easy to use frontend so users can easily
run the virtual machine desktops. It also has some features to help administrators
prepare and manage different kinds of pre-built bases.

In its current state of development [Ravada](https://ravada.upc.edu) it is a stable
and widely used application. It has been translated to 18 languages and it is a viable
alternative for organizations that want to provide remote desktops for their users.

We would want to give a new feature so our users can
backup and restore their virtual machines. It is our intention to provide this
new tool using snapshots already available through libvirt.


Expected Outcomes
-----------------

Snapshots could provide an easy
way to end users to backup and restore virtual machines. The goal
is the users are given a web page in the Ravada frontend to create snapshots and
also to revert the virtual machine to a former snapshot. There is already a web
frontend to manage all the Ravada features, the new forms must integrate with the
current frontend code.

Ravada has two running services: a frontend and a backend. The frontend runs as
a non-privileged user and interacts with the end users via a web interface.
The backend receives requests from the frontend and performs privileged operations
in the host operative system to manage the virtual machines.

- Define database tables so snapshots can be stored and shown in the web
frontend.
- Create new methods for the virtual machine classes to create and revert snapshots.
This should be done using libvirt API.
- Remove all the snapshots when removing the virtual machine
- Create a new type of request so the frontend can ask to perform the snapshots
operations.
- Provide a perl test file to check the snapshots are created, used and removed.
- Design a web form for the end user to create snapshots. The user should be able
to add a name and description for new snapshots.
- Design a web form for the user to revert the virtual machine to a previous snapshot.
- Design a web form for the user to remove snapshots.


Required skills
---------------

Experience with Perl, Mojolicious, HTML. Some small parts require Javascript and Angular.

Rating
------

Medium.

Possible Mentors
----------------

- Frankie (frankie@telecos.upc.edu / [GitHub](https://github.com/frankiejol))
- Fernando (fernando@telecos.upc.edu / [GitHub](https://github.com/fv3rdugo))

