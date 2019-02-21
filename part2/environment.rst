

:authors: Jason Lowe-Power

.. _development-environment-chapter:

---------------------------------------
Setting up your development environment
---------------------------------------

This is going to talk about getting started developing gem5.

gem5-style guidelines
~~~~~~~~~~~~~~~~~~~~~

When modifying any open source project, it is important to follow the project's style guidelines.
Details on gem5 style can be found on the gem5 `wiki page`_.

.. _wiki page: http://gem5.org/Coding_Style

To help you conform to the style guidelines, gem5 includes a script which runs whenever you commit a changeset in git.
This script should be automatically added to your .git/config file by SCons the first time you build gem5.
Please do not ignore these warnings/errors.
In the rare case where you are trying to commit a file that doesn't conform to the gem5 style guidelines (e.g., something from outside the gem5 source tree) you can use the git option ``--no-verify`` to skip running the style checker.

The key takeaways from the style guide are:

- Document your code
- Use 4 spaces, not tabs
- Avoid lines longer than 80 characters
- Use `PascalCase` for class names, `camelCase` for member variables, and `snake_case` for local variables.
- Sort the includes


git branches
~~~~~~~~~~~~

Most people developing with gem5 use the branch feature of git to track their changes.
This makes it quite simple to commit your changes back to gem5.
Additionally, using branches can make it easier to update gem5 with new changes that other people make while keeping your own changes separate.
The `Git book`_ has a great chapter_ describing the details of how to use branches.

.. _Git book: https://git-scm.com/book/en/v2

.. _chapter: https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell
