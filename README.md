

# README #

This README would normally document whatever steps are necessary to get your application up and running.

### What is this repository for? ###

* Quick summary
* Version
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

### How do I get set up? ###

* Summary of set up
* Configuration
* Dependencies
* Database configuration
* How to run tests
* Deployment instructions

### Contribution guidelines ###

* Writing tests
* Code review
* Other guidelines

### Who do I talk to? ###

* Repo owner or admin
* Other community or team contact


### TODO ###

- add version command
    default - get current version
    -n get next version from current branch (master - next sprintbuild, release/* - next releasebuild)


### Setup configure ###

```
# go to bin folder
> cd <bin_project_folder>

# add auxoft-flow of submodules 
> git submodules add https://..../auxoft-flow

# install af command to root project folder
> cd <root_project_folder>
> ./<auxoft_flow_folder>/bin/af install

# add hooks to ./<auxoft_flow_folder>/bin/hooks folder

# init auxoft
> ./af init

# or init auoxft and setup base app version
> ./af init -v 1.1.1.1 -n beta

```


### .afconf ###

```
#!/bin/bash


### 0 = true
### 1 = false

### for all commands
###
#
# setflag show_commands 0     #default 1
# setflag silent 0            #default 1


```


### Branches names ###

* master:                      master

* features:                    master -> feature/<feature_name> -> master

* nightbuilds:                 master -> nightbuild/<c>.<d> -> master

* sprintbuilds:                master -> sprintbuild/<c> -> master

* releases:                    master -> release/<a>.<b>

* hotfixes:                    release/<a>.<b> -> hotfix/<hotfix_name> -> release/<a>.<b>

* release candidate builds:    release/<a>.<b> -> rcbuild/<a>.<b>.<c>.<d> -> release/<a>.<b>

* patch builds:                release/<a>.<b> -> patchbuild/<a>.<b>.<c>.<d> -> release/<a>.<b>

* release builds:              release/<a>.<b> -> release/<a>.<b>.<c> -> release/<a>.<b>
