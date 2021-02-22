Pull Request Club: Stats
======================================================

Description
-----------

[Pull Request Club](https://pullrequest.club/) is a web application where users can sign up with their GitHub accounts. Its purpose is to connect
 - people who are looking for an open source project to work on, with
 - people who want new contributors for their open source projects.

Pull Request Club gives out monthly assignments. Web application is built on Catalyst (Perl), and it has a SQLite database.

Expected outcomes
-----------------

- [**Improve landing page:**](https://github.com/kyzn/PRC/issues/41) Currently, [landing page](https://pullrequest.club) does not talk too much about how the site works. We can add some graphics, explain it better, add more information to make it scrollable.

- [**Build a stats page:**](https://github.com/kyzn/PRC/issues/41) Currently there is no way for users to see how much action is happening through the site. We can build a page that shows how many users, how many active users, how many repos in the pool, how many active assignments etc.

- [**Internationalization:**](https://github.com/kyzn/PRC/issues/25) Currently the site is only available in English. We want to show it in other languages too, so we need to wrap all strings around a i18n module.

- [**Announcements:**](https://github.com/kyzn/PRC/issues/39) Add infrastructure for showing site-wide announcements. This means creating a new table and adding some connectors for it.

- **Mojolicious:** If you are feeling adventurous, [Mojolicious just released version 9.0](https://mojolicious.io/blog/2021/02/14/announcing-mojolicious-9-0/). Current framework we use is Catalyst, but we might want to give Mojolicious a try.

- [More work to be done can be seen on GitHub issues.](https://github.com/kyzn/PRC/issues)


Required skills
---------------

This differs based on what issue you want to work on, but here's some basics:
- Some experience with Perl (5) is required. If you have experience with other languages, and want to give Perl a try that's fine too.
- Some knowledge about web applications would be nice. If you know what MVC is, that should be enough. If you have experience with a Perl based web framework, that's great.
- Some knowledge of relational databases is required. If you are interested in issues like "announcements" above, You should know about SQL a bit.

Rating
------

Medium


Possible mentors
----------------

Kivanc Yazan `<kyzn at cpan.org>`
