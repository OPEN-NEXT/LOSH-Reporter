---
title: LOSH Data Report
subtitle: |
          | Annual, mostly statistical report on Open Source Hardware based on data from the LOSH knowledge base
          | **${PROJECT_VERSION_DATE}**
          | *version:* [${PROJECT_VERSION}](${PROJECT_VERSION_URL})
version: "${PROJECT_VERSION}"
date: "${PROJECT_VERSION_DATE}"
lang: en-US
charset: UTF-8
license: CC-BY-4.0
keywords:
- Open Source Hardware
- LOSH
- OSHdata
papersize: a4
geometry: "top=2cm,bottom=2cm,left=3cm,right=3cm"
comment: license applies to generated reports; date is automatically generated
...

# Intro

## General

LOSH xxx

<!--- general info about LOSH to be added -->

Efforts partly merged with the [OSHdata project](oshdata.com), which published annually reports based on data crawled from the [list of OSHWA-certified OSH projects](https://certification.oshwa.org/list.html). Since OSHWA published [its API](https://certificationapi.oshwa.org/documentation), no crawling is needed anymore. And since LOSH is here to collect data also from other platforms, we decided to take care of regular OSHdata reports – now also including data from other platforms.

Generally, all data you will find here is also publicly available in the LOSH knowledge base. This report is generated using the [LOSH-Reporter](https://github.com/OPEN-NEXT/LOSH-Reporter/) tool (GPL-3.0-OR-LATER). All we do is running a bunch of pre-defined queries on LOSH's knowledge base using that tool. If you want to look into the raw data yourself, e.g. to run some self-defined queries, find it [here](https://gitlab.opensourceecology.de/verein/projekte/losh-rdf) ([CC0-1.0](https://gitlab.opensourceecology.de/verein/projekte/losh-rdf/-/blob/main/LICENSE)). The report you are reading is licensed under the Creative Commons Attribution 4.0 International License ([CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/legalcode)). This license covers the entire report, including the text and graphics. OSHdata is a project of the [Open Hardware Observatory e.V. (non-profit)](https://en.oho.wiki/wiki/Imprint) since 2021 (before is was a project of Kenny Consulting Group, LLC).

## Scope

xxx

<!--- brief description of scope to be added -->

## Get in contact with us

OSHdata is hosted by the [Open Hardware Repository e.V. (non-profit)](http://oho.wiki/) since 2021. Feel free to reach out to Robert to get in touch: [rm@oho.wiki](mailto:rm@oho.wiki?cc=mh@oho.wiki&subject=from the LOSH report)

LOSH was started inside the EU-H2020-founded [OPEN_NEXT](https://opennext.eu/) project back in 2020 and is hosted and maintained by [Open Source Ecology Germany e.V. (non-profit)](https://ose-germany.de/) since 2022. You can reach these folks via eMail ([verein@ose-germany.de](mailto:verein@ose-germany.de?cc=martin.haeuer@ose-germany.de&subject=from the LOSH report)) or Telegram ([@OSEGWelcome](https://t.me/OSEGWelcome)) – don't be shy; looking forward to e-meet you :)

You can also sign up for our newsletter [here]() or follow us on Twitter via [@OSHdata](https://twitter.com/OSHdata).

## This report…

<!--- brief intro specific to this version of the report to be added -->

[[TOC]]

# Highlighted Projects

OSH flagship projects

2…4 projects from OSEG-CAB & OHO-CAB to be briefly presented & promoted

<!--- 2021: MNT Reform, OpenFlexure; something from OHO -->

<!--- section to be written manually -->

# LOSH Data

## Introduction

Currently, LOSH collects data from the following platforms:

- [GitHub.com](http://github.com/)
- [Wikifactory.com](https://wikifactory.com/)
- [OSHWA Certification List](https://certification.oshwa.org/list.html)
- [Thingiverse.com](https://www.thingiverse.com/)

Additionally we have scripts catching data from:

- [Appropedia.org](https://appropedia.org/)
- [Open Know-How](https://openknowhow.org/) (including e.g. [Fieldready.org](https://www.fieldready.org/))

and making it available via GitHub (in [this repository](https://github.com/OPEN-NEXT/LOSH-list/)).

The minimum threshold for LOSH to be recognised as an OSH project is to have:

- a free/open license,
- a README file and
- at least one source file (other than the README.md, CONTRIBUTING.md or an image).

<!--- add short description of upload methods (copy from D3.4 + D3.3 report) -->

## Data Sources

### Current Data

By the publishing date of this report, the LOSH knowledge base contains:

- {ghproj} from [GitHub.com](http://github.com/) (not counting Open Know-How or Appropedia.org) ({} % of all its projects)
- {gltotalproj} from gitlab-based platforms ({} % of all its projects) <!---NOTE: gitlab-based repo hosts are listed in /specs/gitlab-platforms -->
- {wifproj} from [Wikifactory.com](https://wikifactory.com/) ({} % of all its projects)
- {oshwaproj} from [OSHWA Certification List](https://certification.oshwa.org/list.html) ({} % of all its projects)
- {thingiproj} from [Thingiverse.com](https://www.thingiverse.com/) ({} % of all its projects)
- {approproj} from [Appropedia.org](https://appropedia.org/) ({} % of all its projects)
- {okhproj} from [Open Know-How](https://openknowhow.org/) ({} % of all its projects)
- {otherproj} from diverse other sources ({} % of all its projects)

…as illustrated in @fig:data-input-count, totalling data from {platform-count} platforms. According to how LOSH works, this equals {data-source-count} different data sources.

<!--- NOTE: the list up there is, what is following abbreviated as {platforms} -->

<!--- a bar chart with the above mentioned values, each bar splitting into accepted and rejected projects (rejected projects on top) -->
{#fig:data-input-count}

@fig:data-input-method-dist shows the distribution of upload methods that have been used for this data set.

<!--- bar chart showing the distribution of uploading methods used for LOSH (auto, manifest, manifest-script, manual) -->
{fig:data-input-method-dist}

### History

Since the first report, published back in February 2022, data input has developed as following:

<!--- combined historical line diagram of total count of projects per year & for for each {platform} -->

Looking into the recent past @fig:data-hist-grow2 shows the grow rates for the past two years.

<!--- horizontal bar chart with grow rates per {platform} per each of the past 2 years + a bar for the total grow rate -->
{#fig:data-hist-grow2}

## Licenses

What separates a piece of open source hardware from a proprietary one is primarily its license.

<!--- add more info, also linking the OSH legal issues guideline and the tl;dr -->

The following @fig:license-dist-ind shows the distribution of licenses under which the _hardware_ has been published per platform.

<!--- 1 pie chart per {platform} showing the distribution of `spdxLicense` --> 
{#fig:license-dist-ind}

Totalled, @fig:license-dist-total is the overall distribution of licenses used for the _hardware_.

<!--- pie chart showing the overall distribution of `spdxLicense`, sorted by strongly, weakly an non-reciprocal licensing schemes --> 
{#fig:license-dist-ind}

## Hardware Types

### Open Technology & Documentation Readiness

Open Technology and Documentation Readiness Levels (OTRL, ODRL, as defined in [ref](https://docs.google.com/document/d/1-l6DI91unnAshzjKhjotpAfy_8RsS-9T7YmdYuwL4RI/edit#)) give a good approximation:

1. how mature the hardware design itself is (OTRL) and
2. how mature and open the documentation is (ODRL).

The different levels are:

[copy from publication]

So the two extreme cases would be:

- an OSH design with OTRL-6 and ODRL-1, meaning a safe-to-use product that could be circulated on the market, but barely barely has any documentation published appart from a README, maybe a few STEP files and bearing a free/open license;
- an OSH design with OTRL-1 and ODRL-4, so a design still in the ideation phase, but exeptionally well-documented, even with documents for a (future) CE-Certification published under a free/open license.

Among the whole knowledge base, the readiness levels distribute as shown in @fig-otrl-total and @fig-odrl-total

<!--- horizontal stacked bar chart for OTRL levels and (stacked) their distribution among the {platforms}, also include "undefined" -->
{#fig:otrl-total}

<!--- horizontal stacked bar chart for ODRL levels and (stacked) their distribution among the {platforms}, also include "undefined -->
{#fig:odrl-total}

@fig:otrl-odrl-heatmap shows the resulting heatmap for a combination of both scales.

<!--- heatmap of all OSH projects with OTRL AND ODRL defined; see p. 5 here: https://docs.google.com/document/d/1-l6DI91unnAshzjKhjotpAfy_8RsS-9T7YmdYuwL4RI/edit#--> 
{#fig:otrl-odrl-heatmap}

### Technology Categories

Classifying hardware by it's technology can be a non-trivial task – every online platform seems to run their own from-scratch-developed category system. LOSH tries to merge some of those category system into one established one that has been around for a while: patent classes, specifically the [Cooperative Patent Classification](https://www.epo.org/searching-for-patents/helpful-resources/first-time-here/classification/cpc.html) system (CPC). This may even help patent agents when searching for relevant open source designs (#defensive-publishing).

However, since LOSH can only process data that is provided in the first place, patents classes are only available for {projects-with-cpc-entry} OSH projects (that is {projects-with-cpc-entry/all-projects} % of the knowledge base). @fig:cpc-total shows the total distribution of top-level CPCs, @tbl:cpc-legend provides the full designation for those IDs.

<!--- stacked bar charts with 1 bar per used first level CPC (F, H etc.) and the next sublevel (e.g. H03) stacked -->
{#fig:cpc-total}

<!--- list of all CPCs used in the bar chart above with their full designation, e.g. "H03 – basic electronic circuitry" (https://worldwide.espacenet.com/patent/cpc-browser#!/CPC=H03); there's an ontology that may be useful for that-->
{#tbl:cpc-legend}

# Platform-specific Insights

## OSHWA

The Open Source Hardware Association (OSHWA) runs a certification program for OSH. Certified projects are officially deemed to be fully compliant to the OSHWA definition of OSH ([ref](https://www.oshwa.org/definition/)).

@fig:oshwa-cert-cumul shows the historical development of certificates issued in the past years

<!--- line plot of cumulated certifications over time (x-axis could be e.g. per quarter, but that's totally optional) -->
#fig:oshwa-cert-cumul

@fig:oshwa-cert-rate and @fig:oshwa-cert-growth show the derived certification rate and relative growth.

<!--- line plot of (certifications per year) over time -->
#fig:oshwa-cert-rate

<!--- horizontal bar chart with growth of (certifications per year) relative to the year before-->
#fig:oshwa-cert-growth

A total of {number-of-biggest-OSHWA-licensors-adding-up-to-50%} creators have combined to certify ~50 % of all currently OSHWA-certified projects. So {number-of-biggest-OSHWA-licensors-adding-up-to-50% / oshwa-unique-licensors-total} % of creators make half of OSHWA's database. On the other end we have {number-of-OSHWA-licensors-with-only-1-certificate} holders of a single certificate ( % of all creators). This calculates to a median of nearly {OSHWA-median-certificates-per-licensor} per participating individual or organization.

@fig:oshwa-cert-rate illustrates the distribution of certifications among creators.

<!--- vertical bar chart with certifications per licensor-->
#fig:oshwa-cert-rate

Since OSHWA also publishes the location of the certified OSH projects (or rather the corresponding team or organisation, presumingly), we can also see how these certifications distribute among countries, as shown in @fig:oshwa-cert-country and @fig:oshwa-cert-country-map.

<!--- vertical bar chart with certifications per country -->
#fig:oshwa-cert-country 

<!--- world map with certifications per country (see https://i0.wp.com/oshdata.wpcomstaging.com/wp-content/uploads/2020/09/cert-density-by-country.png?resize=768%2C467&ssl=1)-->
#fig:oshwa-cert-country-map.

<!--- NOTE: the world map is totally optional; if that's to hard to implement → no biggy -->

## Wikifactory

Wikifactory is an online platform dedicated to OSH. It is designed to need specific needs and offer specialised services that arise in the development (and production) process of OSH. The platform itself is not open source, but free to use (however, there are some cool premium features).

@fig:wif-proj-hist-cumul illustrates the historical growth of OSH projects on Wikifactory; @fig:wif-proj-tag-cloud shows the most popular tags of those projects in a word cloud.

<!--- line plot of cumulated project creations over time (`dateCreated`) (x-axis could be e.g. per quarter, but that's totally optional) -->
#fig:wif-proj-hist-cumul

<!--- word cloud of most used tags -->
#fig:wif-proj-tag-cloud

These projects are downloaded {average-archiveDownloadCount-WIF} times; [{name-of-WIF-project-with-most-downloads}]({repoURL-of-WIF-project-with-most-downloads}) is currently the most downloaded project with now totalling {archiveDownloadCount-of-project-with-most-downloads-WIF} downloads. @fig:wif-downloads-dist shows the distritubion of downloads per project, @fig:wif-downloads-top20 the top 20 of most downloaded projects on wikifactory.

<!--- horizontal bar chart with distribution of downloads per project-->
#fig:wif-downloads-dist

<!--- vertical bar chart with top 20 projects with most downloads-->
#fig:wif-downloads-top20 

On average an OSH project on Wikifactory consists of {average-number-of-contributions-per-project} contributions; [{name-of-WIF-project-with-most-contributions}]({repoURL-of-WIF-project-with-most-contributions}) is currently the project with most contribution ({number-of-contributions-of-WIF-project-with-most-contributions}).

<!--- horizontal bar chart with distribution of contributions per project-->

[some text]

<!--- vertical bar chart with top 20 projects with most contributions-->

<!--- NOTE: the same repeats for contributors ↓-->

That average of contributions per project comes from averagely {} contributors per project; {} is currently the project with most contribution ({}).

<!--- vertical bar chart with top 20 projects with most contributors-->

It is important to mention that lots of projects on Wikifactory are not open source and hence do not appear in this (or the following) statistics.

Since some users on wikifactory also specify the location of their project, we can also see how those projects distribute among countries, as shown in @fig:wif-proj-country and @fig:wif-proj-country-map.

<!--- vertical bar chart with projects per country (`createdInRegion`) -->
#fig:wif-proj-country

<!--- world map with projects per country (see https://i0.wp.com/oshdata.wpcomstaging.com/wp-content/uploads/2020/09/cert-density-by-country.png?resize=768%2C467&ssl=1)-->
#fig:wif-proj-country-map

<!--- NOTE: the world map is totally optional; if that's to hard to implement → no biggy -->

# Outro

<!--- add brief & friendly outro -->

See also

- https://stateofoshw.oshwa.org/

# Undeficed contents 

[to be (maybe) deleted (maybe not)]

```

# git-based platforms, OKH and Appropedia

- some detailled statistics based on manifest files
	+ OKH(v1) count + historical grow rate (2 years)
		* fields used (vertical bar chart) <!--- would require parsing the original YAML files-->
	+ appropedia count + historical grow rate (2 years)
		* fields used (vertical bar chart) <!--- would require parsing the original TOML files-->
	+ on git-based platforms OKH-LOSH (manifest) count + historical grow rate (2 years)
		* fields used (vertical bar chart) <!--- would require parsing the original TOML files-->

## Community-based Assessment according to DIN SPEC 3105-2

- CAB data
	+ project count:
		- attested/in progress + historical grow rate (2 years)
		- OHO / OSEG
	* certification per organisation
	* average assessment time (first submission…final attestation) + variance
	* average number of comments per asssessment + variance for top & bottom 10% of assessment time
```