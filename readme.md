<br/><br/><br/>
<img src="https://s3-eu-west-1.amazonaws.com/esaude/images/esaude-site-header.png" alt="OpenMRS"/>
<br/><br/><br/>

# eSaude Admin App

[![eSaude Docs](https://omrs-shields.psbrandt.io/custom/esaude/docs/blue?logo=esaude)](https://docs.esaude.org)
[![eSaude Slack](https://slack.esaude.org/badge.svg)](https://slack.esaude.org)

The eSaude admin application is an [Express](https://expressjs.com/) API and an
[Angular 4](https://angular.io/) web application that work together to
provide functionality that can be used to administer the eSaude ecosystem of
applications.

For more information see [docs.esaude.org](https://docs.esaude.org) or get in
touch on [Slack](https://paper.dropbox.com/doc/eSaude-Communication-Tools-BVFLlm1LzQqqVoOXtEXwJ#:uid=29125003&h2=Slack).

## Install

To install the eSaude admin app, first install the [prerequisites](https://paper.dropbox.com/doc/eSaude-App-Install-Guide-Uvk5mTlgG2m0nyOYy5Zyg#:uid=515415815748821&h2=Prerequisites) (Docker & Compose), then follow the [eSaude Admin install instructions](https://paper.dropbox.com/doc/eSaude-App-Install-Guide-Uvk5mTlgG2m0nyOYy5Zyg#:uid=853323144286988&h2=eSaude-Admin):

```
$ wget https://get.esaude.org/app/esaude-app-admin.yml
$ docker-compose -p esaude -f esaude-app-admin.yml up -d
```

:pushpin: You will need need `v1.2.30+` of the [eSaude Platform](https://paper.dropbox.com/doc/eSaude-App-Install-Guide-Uvk5mTlgG2m0nyOYy5Zyg#:uid=496479570672974&h2=eSaude-EMR-Platform) running to use the admin app.

## Develop

This repository contains the API and web components as [git submodules](https://github.com/blog/2104-working-with-submodules). Since you will
usually want to work on both components together, it makes sense to work from
within this repository by checking out the code recursively:

```
git clone --recursive git@github.com:esaude/esaude-admin.git
```

If you need to update the submodule code, you can do so by running the following
command in the root of the project:

```
git submodule update --init --recursive
```

Then, inside *each* submodule directory you need to tell git to track the `master`
branch by running:

```
git checkout master
```

:information_source: Note that changes made in the submodules will be pushed to
their respective repositories when you run `git push` in their directories.

See the [API](https://github.com/esaude/esaude-admin-api/blob/master/readme.md) and [web](https://github.com/esaude/esaude-admin-web/blob/master/readme.md) readmes for details on how to contribute to
each component.

## License

[MPL 2.0 w/ HD](http://openmrs.org/license/)
