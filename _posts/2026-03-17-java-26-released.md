---
author: Abiola Lapite
title: Java 26 is Released
tags:
    - Java
    - Programming
categories: programming
---
Today marks the [official release](https://www.oracle.com/au/news/announcement/oracle-releases-java-26-2026-03-17/) of Java 26, so I've been combing through the [release notes](https://jdk.java.net/26/release-notes) to determine what, if anything, would be of interest to the working programmer. 

From what I can make out, that turns out to be very little. Most of the significant changes are either about housekeeping (the [removal](https://openjdk.org/jeps/504) of the long-dead Applet API) or garbage-collection related performance tweaks ([bringing](https://openjdk.org/jeps/516) "Ahead of Time Object Caching" to ZGC[^1] or [reducing G1 synchronisation](https://openjdk.org/jeps/522). Other than extending the HTTP client API to [support HTTP/3](https://openjdk.org/jeps/517)[^2], Java 26 brings absolutely nothing new for programmers who aren't free to use "preview" or "incubator" features in production work (which is pretty much all programmers who work with Java for a living). 

The fact that Oracle and the other contributors to JDK develop continue to find new opportunities to enhance performance is certainly a huge strength of the JVM as a platform, and even if the performance gains between releases are incremental, many such increments do add up over time, giving JVM users strong motivation to update to the latest LTS release as soon as possible. Where Java has long fallen short has been in the pace with which the language side of things has been updated. No matter how devoted one might be to quality, it seems absurd that a language feature like structured concurrency should still be [in preview](https://openjdk.org/jeps/525) after six iterations, or that the Vector API should be undergoing an [11th incubator](https://openjdk.org/jeps/529); worse yet, there's no guarantee that either feature will be considered ready for finalisation in the next few Java releases.

It would be one thing if Java's maintainers were seeking to add features drawn directly from academia, and therefore lacking real-world evidence as to how best to implement them, but that is hardly the case. Nothing being "incubated" or "previewed" is so cutting-edge that one can't find 2 or 3 relatively popular languages which have already implemented them. Worse yet, the features which **do** eventually make their slow and tortured way to final status are hardly so brilliant in implementation as to justify having taken so long: to illustrate, other than carrying "official" status, it's hard to see how Java's "records" improve much on the `@Value` annotation provided by Lombok so many years before records were finalised.

I don't expect Java's maintainers to make a dramatic course correction any time soon, so we can expect several more such lackluster releases before the inevitable Java 29 LTS announcement which grudgingly includes one or two new language features to ensure some minimum of programmer interest. It really is unfortunate that JVM alternatives like Clojure and Scala seem to have lost all steam, as now there's virtually no competition to spur faster change to Java itself. 

[^1]: Which just brings Oracle's ZGC back up to par with where Shenandoah already has been since Java 25.
[^2]: Which is in itself a minor API change, rather than a fundamental enhancement of Java the language. 