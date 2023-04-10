# Awesome Open Source Software Research Data 

![GitHub](https://img.shields.io/github/license/sboysel/awesome-oss-research-data)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This is a (curated) list of relevant datasets and empirical research in the space of Open Source Software development.  We prioritize sources in which (2) the raw data is made publicly accessible or (2) metrics are derived from public sources.  We also include data sources for which only high level insights are available.

An excellent list of datasets used for empirical software engineering / mining software repositories exists at [dspinellis/awesome-msr](https://github.com/dspinellis/awesome-msr). Several relevant data sources from this list are included here.

### Contents

1. [Databases and archives](#databases-and-archives)
2. [Metrics](#metrics)
3. [Contribution patterns](#contribution-patterns)
4. [Platforms](#platforms)
5. [Survey data](#survey-data) 

## Databases and archives

### Software development activity

- [GHTorrent](http://ghtorrent-downloads.ewi.tudelft.nl/)
	- Offline mirror of historical data offered by GitHub's REST API
	- [GitHub org](https://github.com/ghtorrent): website code, tutorial
- [GH Archive](https://www.gharchive.org/)
	- Records GitHub's public timeline of activity

### Contributor communication

- [The Mail Archive](https://www.mail-archive.com/)
  - Catalogs a number of public mailing lists for collaborative projects
  - [FAQ](https://www.mail-archive.com/faq.html)
- [Common Crawl](https://commoncrawl.org/)
  - Raw page data, metadata, and extracted text from the publicly accessible segments of the internet   
  - Timeframe: 2008 - present, monthly since March 2014
  - Data hosted on Amazon S3: [getting started
    docs](https://commoncrawl.org/the-data/get-started/)

### Security

- [GitHub Advisory Database](https://github.com/advisories)
	- A database of CVEs and security issues affecting GitHub packages
	- Timeframe: October 2017 through present 
	- Drawn from [a variety of sources](https://github.com/github/advisory-database#sources) and recorded using [Open Source Vulnerability Format](https://ossf.github.io/osv-schema/)
- [Open Source Vulnerability (OSV) Database](https://osv.dev/)
  - Draws from a variety of [sources](https://github.com/google/osv.dev#current-data-sources) across ecosystems.  Note: encompasses GitHub Advisory Database  
  - GCS bucket: https://osv-vulnerabilities.storage.googleapis.com/
- Anas Nadeem, 2021. GitHub Issue Dataset From Top Repositories of Top Languages. https://doi.org/10.5281/zenodo.5048542

### Software dependency networks

- [Libraries.io](https://libraries.io/)
  - Data on software package depdency relationships over time. Sourced from a number of different ecosystems.
  - [Data releases](https://libraries.io/data)

## Metrics

### Community Health

- [CHAOSS](https://chaoss.community/)
	- Linux Foundation project to establish OSS community health metrics
  - [Metric definitions](https://chaoss.community/kbtopic/all-metrics/)
- [OpenSSF Best Practices Badge
  Program](https://bestpractices.coreinfrastructure.org/en)
  - [Listing of projects](https://bestpractices.coreinfrastructure.org/en/projects), [high-level project statistics](https://bestpractices.coreinfrastructure.org/en/project_stats), [high-level criteria statistics](https://bestpractices.coreinfrastructure.org/en/criteria_stats)
- OpenSSF Criticality Scores
  - An effort by [OpenSSF Securing Critical Projects WG](https://github.com/ossf/wg-securing-critical-projects)
  - Algorithm: ["Quantifying Criticality" by Rob Pike](https://github.com/ossf/criticality_score/blob/main/Quantifying_criticality_algorithm.pdf)
  - Data repository: [https://github.com/ossf/criticality_score](https://github.com/ossf/criticality_score)
- Goggins, S., Lumbard, K. and Germonprez, M., 2021, May. Open source community health: Analytical metrics and their corresponding narratives. In _2021 IEEE/ACM 4th International Workshop on Software Health in Projects,Ecosystems and Communities (SoHeal)_ (pp. 25-33). IEEE.

### Contributor Experience

- Denivan Campos, Luana Martins, & Ivan Machado. (2022). An empirical study on the influence of developers' experience on software test code quality [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.7110141
- Perez, Quentin, Urtado, Christelle, Vauttier, Sylvain, 2022. Dataset of Open-Source Software Developers Labeled by their Experience Level in the Project and their Associated Software Metrics. https://doi.org/10.5281/zenodo.6966195

### Project Characteristics

- Munaiah, N., Kroh, S., Cabrey, C. and Nagappan, M., 2017. Curating github for engineered software projects. _Empirical Software Engineering_, _22_(6), pp.3219-3253. [project website](https://reporeapers.github.io/results/1.html)
- Dabic, Ozren, Aghajani, Emad, Bavota, Gabriele, 2021. GHS (GitHub Search): Sampling Projects in GitHub for MSR Studies. https://doi.org/10.5281/zenodo.4588464

## Contribution patterns

- Marco Ortu, Giuseppe Destefanis, Daniel Graziotin, Michele Marchesi, Marco Tonelli, 2020. Dataset - How do you propose your code changes? Empirical Analysis of Affect Metrics of Pull Requests on GitHub. https://doi.org/10.5281/zenodo.3825044
- Champion, K. and Hill, B.M., 2021. Underproduction: An approach for measuring risk in open source software. In _2021 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER)_ (pp. 388-399). IEEE.
  - [Replication data](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/PUCD2P)

### OSS contribution by private firms

- [Open Source Contributor Index (OSCI)](https://opensourceindex.io/)
  - Tracks GitHub contribution by commercial firms
  - Measures active and total contributors
  - Drawn from [GH Archive](https://www.gharchive.org/) (events from GitHub's
    public timeline)
- Spinellis, Diomidis, Kotti, Zoe, Kravvaritis, Konstantinos, Theodorou, Georgios, & Louridas, Panos. (2020). Enterprise-Driven Open Source Software (1.1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3742962
- Angermeir, F., Voggenreiter, M., Moyón, F. and Mendez, D., 2021, May. Enterprise-driven open source software: a case study on security automation. In _2021 IEEE/ACM 43rd International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP)_ (pp. 278-287). IEEE.
- Shimels Garomssa, Rathimala Kannan, Ian Chai, Dirk Riehle, 2022. How Software Quality Mediates the Impact of Intellectual Capital on Commercial Open Source Software Company Success. Available at: https://dx.doi.org/10.21227/3rwb-vg72.

## Platforms

### Contribution and Bug Bounty platforms

- [IssueHunt.io](https://issuehunt.io/)
- [Bountysource](https://bountysource.com/)
- [boss.dev](https://www.boss.dev/): Bounties for Open Source

### Funding

- [GitHub Sponsors](https://github.com/sponsors)
	- [List of dependencies for projects owned by the currently authenticated user](https://github.com/sponsors/explore) (i.e. you). CSV export available.
- [Kivach](https://kivach.org/)
	- "cascading funding": donations to a project redistrbuted upstream
- [Ko-fi](https://ko-fi.com/)
- [Liberapay](https://en.liberapay.com/)
- [Open Collective](https://opencollective.com/)
	- transparent budgeting
- [oss.fund](https://www.oss.fund/)
	- aggregator for OSS funding opportunities, programs, and platforms
- [StackAid](https://www.stackaid.us/)
	- donations redistributed evenly across project's dependencies
	- [simulation of funding allocation](https://simulation.stackaid.us/projects)

### Wikipedia

- Wikipedia (open crowd sourcing platform)
 	- data dumps: https://dumps.wikimedia.org/enwiki/
 	- SQL access: https://quarry.wmcloud.org/ 
- Ekaterina Levitskaya, Gizem Korkmaz, Daniel Mietchen, Lane Rasberry, 2022. Analysis of Linked GitHub and Wikidata https://doi.org/10.5281/zenodo.7443339

### Q&A Platforms

- [StackExchange](https://stackexchange.com/)
  - Public Q&A data across the StackExchange 
  - [SE's Data Explorer](https://data.stackexchange.com/)
  - [(latest) data dump hosted by Internet Archive](https://archive.org/details/stackexchange)
  - [Older vintages](https://meta.stackexchange.com/a/224922/619295) can be tracked down

## Survey Data

- [Linux Foundation: FOSS Contributor Survey](https://www.linuxfoundation.org/resources/publications/foss-contributor-survey-2020)
	- access: high level insights public
	- timeframe: 2020
- [GitHub State of the Octoverse](https://octoverse.github.com/)
	- access: high level insights public
	- timeframe: ?-2022 (annual)
- [Github Open Source Survey](https://opensourcesurvey.org/2017/#data)
	- access:  (anonymized) individual responses public
	- timeframe: 2017
- [Stack Overflow Annual Developer Survey](https://insights.stackoverflow.com/survey)
	- access: (anonymized) individual responses public
	- timeframe: 2011-2022 (annual)
- [GitLab Global Developer Survey](https://about.gitlab.com/developer-survey/previous/)
	- access: high level insights public
	- timeframe: 2016-2020 (annual)
- [Tidelift](https://tidelift.com/about/resources/surveys?filter_topic=Survey)
	- access: high level insights
	- timeframe: 2018-2022 (annual, varying topics)
- [SlashData Developer Nation Survey](https://www.developereconomics.net/)
	- access: not distributed publicly
	- timeframe: ?
- [Snyk and the Linux Foundation: State of Open Source Security](https://snyk.io/reports/open-source-security/)
	- access: high level insights public
	- timeframe: 2022
- [O'Reilly: "The Value of Open Source in the Cloud Era"](https://www.oreilly.com/library/view/the-value-of/9781098103286/ch01.html)
	- access: high level insights public
	- timeframe:
	- [PDF copy of report](https://openjsf.org/wp-content/uploads/sites/84/2021/05/TheValueofOpenSourceinaCloudEra-FinalOReillyReport-1.pdf)
- [FINOS / Linux Foundation State of Open Source in Financial Services](https://www.finos.org/state-of-open-source-in-financial-services-2021)
	- access: high level insights public
	- timeframe: 2021-2022 (annual)
- [Open Source Programs Survey](https://github.com/todogroup/osposurvey) by [TODO Group](https://todogroup.org/#)
	-  access: firm-level responses public
	- timeframe: 2018-2022 (annual)
	- [additional resources on OSPOs](https://todogroup.org/guides/)
- [Open Source Initiative and OpenLogic: State of Open Source survey](https://www.openlogic.com/resources/2022-open-source-report)
	- access: high level insights public
	- timeframe: 2022
- Hertel, G., Niedner, S. and Herrmann, S., 2003. Motivation of software developers in Open Source projects: an Internet-based survey of contributors to the Linux kernel. _Research policy_, _32_(7), pp.1159-1177.
- Lakhani, K.R. and Wolf, R.G., 2003. Why hackers do what they do: Understanding motivation and effort in free/open source software projects. _Open Source Software Projects (September 2003).
- Georgia M. Kapitsaki, Maria Papoutsoglou, Daniel German, Lefteris Angelis, 2020. Dataset from "What do developers talk about open source software licensing? " - SEAA2020. https://doi.org/10.5281/zenodo.3871565
- Feitelson, Dror. (2021). Survey on Developer and Researcher Views on the Ethics of Experiments on Open-Source Projects [Data set]. Zenodo. https://doi.org/10.5281/zenodo.5752053

## Other Resources

- [NBER Economics of Digitization](https://www.nber.org/programs-projects/projects-and-centers/economics-digitization/economics-digitization-research-projects)
- [Linux Foundation Research](https://www.linuxfoundation.org/research)
- https://opensource.com/article/22/12/data-scientists-guide-open-source-community-analysis
- [GitHub Data Dictionary](https://github.com/github/developer-policy/blob/data-dictionary/data_dictionary.md)
- [Google Search for Research Datasets](https://datasetsearch.research.google.com/)
