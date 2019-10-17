# Stoq Dockerfiles

This repository contains all of STOQ's Dockerfiles. 

## When creating a new Dockerfile

- Name it Dockerfile.<descriptive tag>

- Upload it to Gitlab's Dockerfiles repository

- On the stoq-dockerfile repository ond Dockerhub:

		- go to the 'Builds' tab

		- click the 'Configure Automated Builds' button

		- click the 'Build Rules +' button

		- set the configs to: branch, 'master', <tag to the build>,
		  <name of Dockerfile>, '/'. Autobuild and Build Caching should
be enabled.

		- click the 'Save and Build' button.

As soon as the build finishes, the builds will be available and their names
will be defined by the <tag to the build> defined on the rules.
