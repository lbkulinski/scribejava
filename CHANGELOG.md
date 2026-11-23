# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

This is a fork of [ScribeJava](https://github.com/scribejava/scribejava). The history of the upstream project up to
8.3.3 is in the [`changelog`](changelog) file.

## [Unreleased]

## [9.0.0] - 2026-11-23

First release of the `net.lbku` fork, based on upstream ScribeJava 8.3.3.

### Changed

- **Breaking:** Maven `groupId` is now `net.lbku` (was `com.github.scribejava`). Artifact ids and Java package names are
  unchanged.
- **Breaking:** the minimum Java version is now **11** (was 7)
- **Breaking:** `scribejava-httpclient-ahc` now uses `org.asynchttpclient:async-http-client` **3.0.14** (was 2.12.3).
  Its timeout settings take `java.time.Duration`
- Bumped `com.fasterxml.jackson.core:jackson-databind` from **2.14.0** → **2.23.0**
- Bumped `com.linecorp.armeria:armeria` from **1.20.2** → **1.43.1**
- Bumped `com.squareup.okhttp3:okhttp` from **4.10.0** → **4.12.0**
- Bumped `org.apache.httpcomponents:httpclient` from **4.5.13** → **4.5.14**
- Bumped `commons-codec:commons-codec` from **1.15** → **1.23.0**
- Bumped `jakarta.xml.bind:jakarta.xml.bind-api` from **4.0.0** → **4.0.5**
- Bumped `javax.xml.bind:jaxb-api` from **2.3.0** → **2.3.1**
- Netty is now **4.2.21** in `scribejava-httpclient-ahc` (was 4.1.60)
- Publishing to Maven Central now uses `central-publishing-maven-plugin`

### Removed

- `scribejava-httpclient-ning`, which depended on the end-of-life Netty 3 (and has no fixed release)
- Donation links that pointed to the upstream maintainer

[Unreleased]: https://github.com/lbkulinski/scribejava/compare/v9.0.0...HEAD
[9.0.0]: https://github.com/lbkulinski/scribejava/releases/tag/v9.0.0
