Jenkins-Docker Dev Env
======================

Purpose
-------

A simple docker-compose file which starts jenkins via Docker Compose.
The idea is to have a running jenkins locally for testing the current
setup creates a .jenkins_home (which is naturally in gitignore ...) so
you can revisit it on every developmen iteration in the same state.

![jenkins-docker](http://www.tothenew.com/blog/wp-content/uploads/2015/10/627x302xdocker-jenkins.png.pagespeed.ic.rdLVquN8qf.png)

Usage
-----
Create a .env file with any Environment variable you might want to send
to Jenkins such as 'jenkins.install.runSetupWizard' which you can set to
false in order to skip the wizard - [A Full list
here](https://wiki.jenkins.io/display/JENKINS/Features+controlled+by+system+properties)


Todo
----
1. Add a set of default plugins to jenkins via plugins.txt file in the
container
2. Configure commomn usecases such as Shared library development and
   varios command line utils
3. Consider - push jenkins_home to GitLFS ?! / Custom jenkins-dev
   container with a specific set of plugins ? - TBD

Collaborators
-------------
* Haggai Philip Zagury
* Chen Cohen

Looking forward
---------------
To be continued ...
