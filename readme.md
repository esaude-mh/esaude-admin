<br/><br/><br/>
<img src="https://s3-eu-west-1.amazonaws.com/esaude/images/esaude-site-header.png" alt="OpenMRS"/>
<br/><br/><br/>

# eSaude Admin App

[![Build Status](https://img.shields.io/travis/esaude/esaude-admin/master.svg)](https://travis-ci.org/esaude/esaude-admin)
[![eSaude Slack](https://slack.esaude.org/badge.svg)](https://slack.esaude.org)

The eSaude admin application is an [Express](https://expressjs.com/) API and an
[Angular 2](https://angular.io/) web application that work together to
provide functionality that can be used to administer the eSaude ecosystem of
applications.

For more information see [docs.esaude.org](https://docs.esaude.org).

## Install

To install the eSaude admin app, first install the [prerequisites](https://paper.dropbox.com/doc/eSaude-App-Install-Guide-Uvk5mTlgG2m0nyOYy5Zyg#:uid=515415815748821&h2=Prerequisites) (Docker & Compose), then follow the [eSaude Admin install instructions](https://paper.dropbox.com/doc/eSaude-App-Install-Guide-Uvk5mTlgG2m0nyOYy5Zyg#:uid=853323144286988&h2=eSaude-Admin):

```
$ wget https://get.esaude.org/app/esaude-app-admin.yml
$ docker-compose -p esaude -f esaude-app-admin.yml up -d
```

## Develop

See the [API](api) and [web](web) readmes for details on how to contribute to
each component.

## License

[MPL 2.0 w/ HD](http://openmrs.org/license/)
