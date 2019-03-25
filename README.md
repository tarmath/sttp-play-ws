## sttp-play-ws ##

[![Build Status](https://travis-ci.org/ragb/sttp-play-ws.svg?branch=master)](https://travis-ci.org/ragb/sttp-play-ws)

[sttp][sttp] backend for [play-ws][playws].

### Goals ###

The main goal of this library is to allow the usage of sttp machinery in the context of an already existing Play app, avoiding inclusion of a different HTTP client.
If you develop HTTP clients with sttp to be used, e.g. on an Akka based micro Service, and you need some of the same logic in your Play Frontend / backoffice application writen in play, this library may be helpful.


### Getting it ###
 
 Include the following on your build.sbt or similar:
 
 
```scala
libraryDependencies += "com.ruiandrebatista.sttp" %% "sttp-play-ws-<playVersion>" % "0.1.0"
```

This library is published for both play 2.6 and 2.7.
Check the following table for artifact name and associated play versions you might use for the artifact name.

| Artifact Name   | Play Version |
|-----------------|--------------|
| sttp-play-ws-26 | 2.6.17       |
| sttp-play-ws-27 | 2.7.0             |

### Usage with Guice ###




### Notes ###

This library depends on `
play-ws` (ense many play dependencies) and not on the play-ws-standalone project. This is due to the missing multipart support on the standalone artifact.
When this gets sorted library will probably change to depend solely on play-ws-standalone.






[sttp]: https://github.com/softwaremill/sttp
[playws]: https://github.com/playframework/play-ws

