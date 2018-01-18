.. _contributing:

Discussion and Contributing
===========================

Contributing to this wiki
-------------------------

To add to this wiki either:

#. Add an 'issue' explaining your suggestion to the `Issue Tracker <https://github.com/open-actuarial/open-actuarial-site/issues>`_ of the site's repository on GitHub. Someone else can then pick up the suggestion and incorporate it into the site. (very simple to do, good for anyone not yet comfortable with GitHub or Sphinx)
#. `Edit the site <editing_the_site_>`_ yourself by submitting a pull-request (requires knowledge of GitHub and Sphinx but significantly reduces the workload for the Core Team)


.. _editing_the_site:

Editing the site
----------------

.. highlight:: bash

This site is built using `Sphinx <http://www.sphinx-doc.org>`_, a Python package that creates static websites such as wikis or project documentation. The site is made up of a collection of rst and markdown text files with Sphinx turning the text files into a full website.

The site's code is version controlled using Git and hosted on GitHub.

A `Conda <https://conda.io/docs/index.html>`_ virtual environment is used manage the build environment and reduce the chance of build errors.

This site follows the standard steps for contributing to a GitHub based open-source project.

First time setup
^^^^^^^^^^^^^^^^

#. Fork the site's `repository <https://github.com/open-actuarial/open-actuarial-site>`_ to your personal GitHub account.
#. Clone your fork to your local machine::

    cd desired_folder # change directory to the location where you will keep the project

    # where user_name is your github username
    git clone git@github.com:user_name/open-actuarial-site.git # if using ssh or
    git clone https://github.com/user_name/open-actuarial-site.git # if using https

#. Add the main project as upstream (allows you to pull in changes made by others)::

    # add upstream (location of main repository)
    git remote add upstream  git@github.com:open-actuarial/open-actuarial-site.git # if using ssh
    git remote add upstream https://github.com/open-actuarial/open-actuarial-site.git # if using https

#. Move into project directory::

    cd OpenActuarialSite # move into the site's working directory

#. Set up the environment::

    pip install conda # if you do not have conda installed already (you will do if you have installed Anaconda)
    conda env create -f wiki_env.yml # creates a virtual environment using the yml file for the list of packages

    # start the virtual environment
    activate wiki # for windows
    source activate wiki # for MacOS or Linux

Making changes
^^^^^^^^^^^^^^

#. Fetch upstream updates from main GitHub repository (in case anyone else has made changes since you last worked on the project)::

    git pull upstream master

#. Create a new branch for your suggestion::

    git branch branch_name # where branch_name is the name of the feature or bug

#. Make the changes by adding new pages to the wiki (as rst or md files), editing existing ones or a combination of both
#. Test that the change has the desired effect by rebuilding the wiki using Make HTML::

    make html # from windows CMD not Git Bash

#. Commit the change to the feature branch::

    git add file_name # to stage a change to a single file, or
    git add . # if staging changes to all files
    git commit -m "commit_message"

#. Push the changes to your forked GitHub repository::

    git pull upstream master # (to check for changes by others)
    git push origin branch_name

#. Submit a pull request on main repository
#. The change will be reviewed by the Core Team - if revisions are requested further commits may be required
#. Pull request is accepted or rejected

If using two-factor authentication (2FA)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

On windows, GitHub for Windows makes it a lot easier to use 2FA. If using the command line then you will use ssh. See `Settings <https://github.com/settings/keys>`_ on your GitHub account to set up ssh keys.

Once ssh keys are set up:

#. Test ssh connection (from `GitHub articles <https://help.github.com/articles/testing-your-ssh-connection/>`_)::

    ssh -T git@github.com
    # Attempts to ssh to GitHub

#. Launch ssh agent::

    eval $(ssh-agent -s)

#. Add private key (if not already added)::

    ssh-add ~/.ssh/id_rsa
    # assumes key is already set up
