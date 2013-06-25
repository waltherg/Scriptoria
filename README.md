drcs-science
============
Ideas on a potential project to build a central website that tracks manuscripts being written with distributed revision-control systems (git, mercurial, ...).

Name
----
...

Why
---
Git keeps the full history of the documents, is safe, makes it easy to fork and modify scientific output. It *was* made for collaboration after all. Also, websites like github, bitbucket, and gitorious allow users to post "Issues", essentially a sophisticated and transparent form of peer-review.

However, there is currently no easy way to track manuscripts being developed on github, bitbucket, and other servers. The aim of the project is to increase the visibility of open science with distributed revision-control systems.

How
---
The system should, at the very least, do the following:
* Allow users to add repository on several common webservers (github, bitbucket, gitorious). Perhaps even allowing some automatic system based on a convention (if the depo starts with "ms_", "article_", ... and the user is registered, then track it).
* Tags the depo by types (manuscript, presentation, thesis, ...) and content (machine learning, molecular evolution).
* Use the servers' API to extract basic information the depo (starting date, number of commits, participants, branches, issues, DOI).

What
----
Tools:
* Yesod web framework (Haskell): fast, safe & fun.
* Open identification system.
* Goold ol' MySQL (?)
* 100% open source: the code should be stored on gitorious (more neutral than github).
* Offer an API.

