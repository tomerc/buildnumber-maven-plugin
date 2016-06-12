# MojoHaus BuildNumber Maven Plugin

This is the [buildnumber-maven-plugin](http://www.mojohaus.org/buildnumber-maven-plugin/).
 
[![Build Status](https://travis-ci.org/mojohaus/buildnumber-maven-plugin.svg?branch=master)](https://travis-ci.org/mojohaus/buildnumber-maven-plugin)

## Releasing

* Make sure `gpg-agent` is running.
* Make sure all tests pass `mvn clean verify -Prun-its`
* Execute `mvn -B release:prepare release:perform`

For publishing the site do the following:

```
cd target/checkout
mvn verify site site:stage scm-publish:publish-scm
```
