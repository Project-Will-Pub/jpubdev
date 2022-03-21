# [pub.dev](https://pub.dev) REST API implementation in Java

[![Test](https://github.com/Project-Will-Pub/jpubdev/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/Project-Will-Pub/jpubdev/actions/workflows/test.yml)
[![CodeQL](https://github.com/Project-Will-Pub/jpubdev/actions/workflows/codeql.yml/badge.svg?branch=main)](https://github.com/Project-Will-Pub/jpubdev/actions/workflows/codeql.yml)
[![Maven Central](https://img.shields.io/maven-central/v/xyz.rk0cc.willpub/jpubdev.svg?label=Maven%20Central)](https://search.maven.org/search?q=g:%22xyz.rk0cc.willpub%22%20AND%20a:%22jpubdev%22)

This package aims to parse API result from pub.dev or other pub repository server information into
Java object.

This repository is "reverse engineering" [pub_api_client's](https://github.com/leoafarias/pub_api_client) feature to Java which written in Dart originally with different 
structures.

## Supported feature

* Search package
  * Supported sort with different method
* Fetch package's information
  * Released versions
  * Options
  * Pub score and analystic report

## User Agents

JPubdev has it's own user agents which following with this format:

```text
jpubdev/[jpubdev's version] (JRE [Java version])
```

And the table for square bracket:

| Square bracket label | Meaning | Sample |
|:---:|:---|:---:|
|jpubdev's version|JPubdev's version (Unchanged when new patch version released)|`jpubdev:1.0.0` > `1.0.0` <br/> `jpubdev:1.0.3` > `1.0.0` <br/> `jpubdev:1.2.0` > `1.2.0`|
|Java version|Java version uses for running jpubdev| `17` <br/> `17.0.1`|

## Install

**Maven POM**
```xml
<dependencies>
    <dependency>
        <groupId>xyz.rk0cc.willpub</groupId>
        <artifactId>jpubdev</artifactId>
        <version>1.0.5</version>
    </dependency>
</dependencies>
```
<p>* this package is bundled <a href="https://github.com/Project-Will-Pub/jpubspec">jpubspec</a> 2.0.1</p>

## Setup requirement

* Maven 3
* JDK 17 or higher

## License

BSD 3
