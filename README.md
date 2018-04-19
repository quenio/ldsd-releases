# LDSD Releases

This repository has the released packages of LDSD Languages.

## Pre-requisites

### Homebrew / Linuxbrew

One of the following is required to install any of the LDSD Languages:
- Homebrew (on macOS - at https://brew.sh)
- Linuxbrew (on Linux - at http://linuxbrew.sh)

Please report an issue if you cannot get any of the LDSD Tools installed using Homebrew or Linuxbrew.

### Java 8

The only pre-requisite to run the CML compiler is Java 8.

The commands of the LDSD Languages should just work after installation if Java 8 is available on the environment.

Please report an issue, otherwise.

## Quick, Two-Step Install with Homebrew / Linuxbrew

```
$ brew tap quenio/ldsd # To make the LDSD Language packages available.
$ brew install ldsd-math # To install the latest release of the Math language.
```

## Release Notes

To read the release notes of a specific version, please go to: https://github.com/quenio/ldsd-releases/tree/master/ldsd-<suffix>

Look for the files ending with '.zip.notes.md'. For example: ldsd-math-1.0.zip.notes.md

## Release Versioning

The release version format is YEAR.MONTH.DAY-CHANNEL, where:
- YEAR/MONTH/DAY: the year/month/day the version was released.
- CHANNEL: which channel the release was published in: _gold_: backward-compatible, high-quality releases with low-risk upgrade; _alpha_: development releases without quality/compatibility guarantees, i.e. high-risk upgrade.

Either release channel may include bug fixes and new features.

## Installing Specific Version with Homebrew / Linuxbrew

### Finding Packages

Before you can install the LDSD Languages, please run:

```
$ brew tap quenio/ldsd
```

After that, the LDSD Language packages will be available and they can be installed.

### Finding Versions

To find the versions of the LDSD Languages available to install:

```
$ brew update # To fetch all available versions.
$ brew search ldsd-math # To list available versions of Math language.
```

To read the release notes of a specific version, please go to (look for the '.zip.notes.md' files): https://github.com/quenio/ldsd-releases/tree/master/ldsd-<suffix>

### The Very Latest

If you'd like to always have the latest version of the LDSD Languages,
regardless of the channel where it was released:

```
$ brew update # To fetch all available versions.
$ brew install ldsd-math # To install the Math language.
```

Later on, to upgrade to the latest version:

```
$ brew update # To fetch all available versions.
$ brew upgrade ldsd-math # To install the Math language.
```

You may get a new gold version
(and thus backward-compatible/high-quality version),
but you may also get an alpha release.

### Specific Channel

If you'd like to get the latest release of a specific channel:

```
$ brew update # To fetch all available versions.
$ brew install ldsd-math-CHANNEL # where CHANNEL = alpha or gold
```

Once you've installed it, you can upgrade to the latest release of the channel with:

```
$ brew update # To fetch all available versions.
$ brew upgrade ldsd-math-CHANNEL # where CHANNEL = alpha or gold
```

### Specific Day Version

You can also get the release of a specific day:

```
$ brew update # To fetch all available versions.
$ brew install ldsd-math@YEAR.MONTH.DAY
```

### Specific Year Version

You can even get the latest release of a specific year:

```
$ brew update # To fetch all available versions.
$ brew install ldsd-math@YEAR
```

If you've installed the current year, you can upgrade to the latest release of the current year with:

```
$ brew update # To fetch all available versions.
$ brew upgrade ldsd-math@CURRENT_YEAR
```
