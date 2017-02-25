

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


# auxoft-flow versions:
#
# short_version="a.b.c.d"
#   a - product version : 0 - it's beta versions, >= 1 - releases
#   b - product subversion:
#     if b is odd then this is development versions
#     if b is even then this is release versions
#
#   c - if b is odd then c = sprint number
#   c - if b is even then c - path version
#      if c is odd then this is stable release
#      if c is even then this is unstable release
#
#   d - if b is odd then d = nightbuild number
#   d - if b is odd then
#     if c is odd then d not set
#     if c is even then d = rc/patch number
#
# full_version="a.b.c.d+<version_name>"
#
#  0.0.1.1+alpha           dev version, sprint = 1, nightbuild = 1            it's nightbuild
#  0.0.1.2+alpha           dev version, sprint = 1, nightbuild = 2            it's nightbuild
#  0.0.2.0+alpha           dev version, sprint = 1,                           it's sprintbuild
#
#
#  0.1.0.1+alpha           unstable release version, release candidate 1      it's rcbuild
#  0.1.0.2+alpha           unstable release version, release candidate 2      it's rcbuild
#
#  0.1.1+alpha             stable release version                             it's release build
#
#  0.1.2.1+alpha           unstable release version, patch 1                  it's patch build
#  0.1.2.2+alpha           unstable release version, patch 2                  it's patch build
#
#  0.1.3+alpha             stable release version                             it's release build
#
#
#  0.2.24.1+alpha          dev version, sprint = 24, nightbuild = 1           it's nightbuild
#  0.2.24.2+alpha          dev version, sprint = 24, nightbuild = 2           it's nightbuild
#  0.2.25.0+alpha          dev version, sprint = 24,                          it's sprintbuild
