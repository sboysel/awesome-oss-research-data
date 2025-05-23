# Awesome Open Source Software Research Data 

![GitHub](https://img.shields.io/github/license/sboysel/awesome-oss-research-data)
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This is a (curated) list of relevant datasets, data sources, and empirical research in the space of Open Source Software development.  We prioritize sources in which (1) the raw data is made publicly accessible or (2) the published metrics are derived from public sources.  We also include data sources for which only high level insights are available.

An excellent list of datasets used for empirical software engineering / mining software repositories exists at [dspinellis/awesome-msr](https://github.com/dspinellis/awesome-msr). Several relevant data sources from this list are included here.

Contributions are welcome and greatly appreciated! Please open an issue or pull request if you have suggestions for new data sources and research.

**Topics**

- [Development activity](#development-activity)
- [Dependency networks](#dependency-networks)
- [Package download statistics](#package-download-statistics)
- [Security](#security)
- [Community and project health](#community-and-project-health)
- [Community discourse](#community-discourse)
- [Valuation](#valuation)
- [Funding](#funding)
- [Surveys](#surveys)
- [Source code analysis](#source-code-analysis)
- [Bounty platforms](#bounty-platforms)
- [Public policy](#public-policy)
- [General web archives](#general-web-archives)
- [Other resources](#other-resources)

## Development activity

**Datasets**

| Source | Description |
|:-------|:------------|
| [GHTorrent](http://ghtorrent-downloads.ewi.tudelft.nl/) | Offline mirror of historical data offered by GitHub's REST API |
| [GH Archive](https://www.gharchive.org/) | Records GitHub's public timeline of activity |
| [Ecosyste.ms](https://ecosyste.ms/) | Tools and open datasets to support, sustain, and secure critical digital infrastructure |
| GitHub [REST API](https://docs.github.com/en/rest) and [GraphQL API](https://docs.github.com/en/graphql) | GitHub's APIs for accessing data |
| [GitHub Innovation Graph](https://innovationgraph.github.com/) | High level insights on worldwide GitHub activity over time. [Blog post](https://github.blog/2023-09-21-announcing-the-github-innovation-graph/) and [repo](https://github.com/github/innovationgraph) |
| [Census II of Free and Open Source Software](https://data.world/thelinuxfoundation/census-ii-of-free-and-open-source-software) | Survey of OSS library production usage at the application library level. [Report](https://www.linuxfoundation.org/research/census-ii-of-free-and-open-source-software-application-libraries) and [data appendix](https://data.world/thelinuxfoundation/census-ii-of-free-and-open-source-software) |
| [Census III of Free and Open Source Software](https://www.linuxfoundation.org/research/census-iii) | [Report](https://www.linuxfoundation.org/hubfs/LF%20Research/lfr_censusiii_120424a.pdf?hsLang=en) and [open data](https://data.world/thelinuxfoundation) |
| [OSSRank](https://ossrank.com/) | Ranking that provides useful mappings between top projects, project types, and contributors (individuals and private companies) |
| [Open Source Contributor Index (OSCI)](https://opensourceindex.io/) | Measures active and total GitHub contributors by private organizations. Drawn from [GH Archive](https://www.gharchive.org/) (events from GitHub's public timeline) |

**Research**

General contribution patterns

- Choudhary, Samridhi; Bogart, Christopher; Rose, Carolyn; Herbsleb, James (2020): Modeling Productivity in Open Source GitHub Projects: A Dataset and Codebase. Carnegie Mellon University. Dataset. https://doi.org/10.1184/R1/6397013.v1
- Marco Ortu, Giuseppe Destefanis, Daniel Graziotin, Michele Marchesi, Marco Tonelli, 2020. Dataset - How do you propose your code changes? Empirical Analysis of Affect Metrics of Pull Requests on GitHub. https://doi.org/10.5281/zenodo.3825044
- Champion, K. and Hill, B.M., 2021. Underproduction: An approach for measuring risk in open source software. In _2021 IEEE International Conference on Software Analysis, Evolution and Reengineering (SANER)_ (pp. 388-399). IEEE.
  - [Replication data](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/PUCD2P)
- Wachs, J., Nitecki, M., Schueller, W. and Polleres, A., 2022. The geography of open source software: Evidence from github. Technological Forecasting and Social Change, 176, p.121478.
  - [data collection scripts](https://github.com/n1tecki/Geography-of-Open-Source-Software) and [output data](https://github.com/johanneswachs/OSS_Geography_Data)
- Ekaterina Levitskaya, Gizem Korkmaz, Daniel Mietchen, Lane Rasberry, 2022. Analysis of Linked GitHub and Wikidata https://doi.org/10.5281/zenodo.7443339

Enterprise driven contribution

- Spinellis, Diomidis, Kotti, Zoe, Kravvaritis, Konstantinos, Theodorou, Georgios, & Louridas, Panos. (2020). Enterprise-Driven Open Source Software (1.1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.3742962
- Angermeir, F., Voggenreiter, M., Moyón, F. and Mendez, D., 2021, May. Enterprise-driven open source software: a case study on security automation. In _2021 IEEE/ACM 43rd International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP)_ (pp. 278-287). IEEE.
- Shimels Garomssa, Rathimala Kannan, Ian Chai, Dirk Riehle, 2022. How Software Quality Mediates the Impact of Intellectual Capital on Commercial Open Source Software Company Success. Available at: https://dx.doi.org/10.21227/3rwb-vg72.

Contributor experience

- Denivan Campos, Luana Martins, & Ivan Machado. (2022). An empirical study on the influence of developers' experience on software test code quality [Dataset]. Zenodo. https://doi.org/10.5281/zenodo.7110141
- Perez, Quentin, Urtado, Christelle, Vauttier, Sylvain, 2022. Dataset of Open-Source Software Developers Labeled by their Experience Level in the Project and their Associated Software Metrics. https://doi.org/10.5281/zenodo.6966195

Project characteristics

- Munaiah, N., Kroh, S., Cabrey, C. and Nagappan, M., 2017. Curating github for engineered software projects. _Empirical Software Engineering_, _22_(6), pp.3219-3253. [project website](https://reporeapers.github.io/results/1.html)
- Dabic, Ozren, Aghajani, Emad, Bavota, Gabriele, 2021. GHS (GitHub Search): Sampling Projects in GitHub for MSR Studies. https://doi.org/10.5281/zenodo.4588464

## Dependency networks

**Datasets**

| Source | Description |
|:-------|:------------|
| ecosyste.ms: Dependency parser for [repositories](https://parser.ecosyste.ms/) | An open API service to parse dependency metadata from many open source software ecosystems manifest files. |
| ecosyste.ms: Dependency resolver for [packages](https://resolve.ecosyste.ms/) | An open API service to resolve dependency trees of packages for many open source software ecosystems. |
| [Libraries.io](https://libraries.io/) | Data on software package depdency relationships over time. Sourced from a number of different ecosystems. |
| Open Source Insights / [deps.dev](https://deps.dev/) | A Google project to develop a software dependency graph across ecosystems. Versioning and vulnerabilty information included. |
| [Repology](https://repology.org/) | Monitors software package vintages (i.e. versioning) across a number of ecosystem repositories. |
| [Data for Software Ecosystem Analysis (DaSEA)](https://dasea-project.github.io/DASEA/) | A continuously updated dataset of software dependencies covering various package manager ecosystems. |

## Package download statistics

**Datasets**

| Source | Description |
|:-------|:------------|
| [PyPI](https://packaging.python.org/en/latest/guides/analyzing-pypi-package-downloads/) | Python package index download statistics. Accessible via [BigQuery dataset](https://console.cloud.google.com/marketplace/product/gcp-public-data-pypi/pypi?q=search&referrer=search&project=ghtorrent-293822) or [simple interface](https://pypistats.org/) |
| [CRAN](https://cran.r-project.org/) | R package download statistics. [CRAN logs](http://cran-logs.rstudio.com/) |
| [RubyGems](https://ui.honeycomb.io/ruby-together/datasets/rubygems.org/result/7WeAgPYyjTH) | Ruby package traffic statistics. Tons of information created by [Honeycomb](https://docs.honeycomb.io/quickstart/) |
| [Julia](https://discourse.julialang.org/t/announcing-package-download-stats/69073) | Julia download statistics since October 2021 |
| [npm](https://www.npmjs.com/package/npm-stats-api) | Node.js download statistics API |
| [NuGet](https://nugettrends.com/) | Historical .NET/C# download numbers. [GitHub project](https://github.com/dotnet/nuget-trends) |
| [PECL](https://pecl.php.net/package-stats.php) and [Pear](https://pear.php.net/package-stats.php?cid=3&pid=40&rid) | PhP download statistics |
| [crates.io](https://crates.io/data-access) | Rust download statistics |
| [Clojars API](https://github.com/clojars/clojars-web/wiki/Data#download-stats) | Clojure package download statistics. |

## Security

**Datasets**

| Source | Description |
|:-------|:------------|
| [CVE Program](https://www.cve.org/) | CVE list bulk downloads available in [CVEProject/cvelistV5](https://github.com/CVEProject/cvelistV5) |
| [NIST National Vulnerability Database](https://nvd.nist.gov/) | A Common Vulnerabilities and Exploits (CVE) database. **Timeframe:** October 1988 - present. |
| [CISA Known Exploited Vulnerabilities Catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) | CISA maintained database of known exploited vulnerabilities in the wild. [Each KEV is linked to a CVE](https://www.cve.org/About/RelatedEfforts#KEV) |
| [GitHub Advisory Database](https://github.com/advisories) | A database of CVEs and security issues affecting GitHub packages. Drawn from [a variety of sources](https://github.com/github/advisory-database#sources) and recorded using [Open Source Vulnerability Format](https://ossf.github.io/osv-schema/). **Timeframe:** October 2017 - present. |
| [Open Source Vulnerability (OSV) Database](https://osv.dev/) | Draws from a variety of [sources](https://github.com/google/osv.dev#current-data-sources) across ecosystems. GCS bucket: [https://osv-vulnerabilities.storage.googleapis.com/](https://osv-vulnerabilities.storage.googleapis.com/). **Note:** encompasses GitHub Advisory Database |
| CVEfixes Dataset | Bhandari, Guru, Naseer, Amara, Moonen, Leon, 2021. CVEfixes Dataset: Automatically Collected Vulnerabilities and Their Fixes from Open-Source Software. [DOI](https://doi.org/10.5281/zenodo.4476564) |
| [GitHub Issue Dataset](https://doi.org/10.5281/zenodo.5048542) | Anas Nadeem, 2021. GitHub Issue Dataset From Top Repositories of Top Languages. [DOI](https://doi.org/10.5281/zenodo.5048542) |

## Community and project health

**Datasets**

| Source | Description |
|:-------|:------------|
| [CHAOSS](https://chaoss.community/) | Linux Foundation project to establish OSS community health metrics. [Metric definitions](https://chaoss.community/kbtopic/all-metrics/) |
| [OpenSSF Best Practices Badge Program](https://bestpractices.coreinfrastructure.org/en) | [Listing of projects](https://bestpractices.coreinfrastructure.org/en/projects), [high-level project statistics](https://bestpractices.coreinfrastructure.org/en/project_stats), [high-level criteria statistics](https://bestpractices.coreinfrastructure.org/en/criteria_stats) |
| OpenSSF Criticality Scores | An effort by [OpenSSF Securing Critical Projects WG](https://github.com/ossf/wg-securing-critical-projects). [Algorithm: "Quantifying Criticality"](https://github.com/ossf/criticality_score/blob/main/Quantifying_criticality_algorithm.pdf) by Rob Pike and [data respository](https://github.com/ossf/criticality_score) |

**Tools**
| Source | Description |
|:-------|:------------|
| [isitmaintained.com](https://isitmaintained.com/) | Quick status checks for public GitHub repositories (e.g. median issue resolution time, percentage of open issues). |
| [GitWhois](https://gitwhois.com/) | High-level glance into GitHub repositories |

**Research**

- Goggins, S., Lumbard, K. and Germonprez, M., 2021, May. Open source community health: Analytical metrics and their corresponding narratives. In _2021 IEEE/ACM 4th International Workshop on Software Health in Projects,Ecosystems and Communities (SoHeal)_ (pp. 25-33). IEEE.

## Community discourse

| Source | Description |
|:-------|:------------|
| [StackExchange](https://stackexchange.com/) | Public Q&A data across the StackExchange network. [SO's Data Explorer](https://data.stackexchange.com/stackoverflow) and [latest data dump hosted by Internet Archive](https://archive.org/details/stackexchange). [Older vintages](https://meta.stackexchange.com/a/224922/619295) can be tracked down. |
| [Linux Kernel Mailing List](https://lkml.org/) | The Linux kernel mailing list. |
| [Apache Mail Archives](https://lists.apache.org/) | Mailing list archives for Apache projects |
| [GNU Mail Archives](https://lists.gnu.org/archive/html/) | Mailing lists used by various GNU projects |
| [Python Mailing Lists](https://mail.python.org/mailman/listinfo) | Mailing lists used by various Python projects |
| [The Mail Archive](https://www.mail-archive.com/) | Catalogs a number of public mailing lists for collaborative projects. [FAQ](https://www.mail-archive.com/faq.html) |
| [Mailing list ARChives](https://marc.info/) | |

## Valuation

**Research**

- Blind, K., Böhm, M., Grzegorzewska, P., Katz, A., Muto, S., Pätsch, S. and Schubert, T., 2021. The impact of Open Source Software and Hardware on technological independence, competitiveness and innovation in the EU economy. Final Study Report. European Commission, Brussels, doi, 10, p.430161.
- Bayoán Santiago Calderón, Robbins, Guci, Korkmaz, and Kramer. 2022. Measuring the Cost of Open-Source Software Innovation on GitHub. Ann Arbor, MI: Inter-university Consortium for Political and Social Research [distributor], 2022-05-26. https://doi.org/10.3886/E158823V2
	- [BEA link to report](https://www.bea.gov/research/papers/2022/measuring-cost-open-source-software-innovation-github)
	- [dataset](https://www.openicpsr.org/openicpsr/project/158823/version/V2/view)
- Wright, N.L., Nagle, F. and Greenstein, S., 2023. Open source software and global entrepreneurship. Research Policy, 52(9), p.104846.
- Hoffmann, Manuel and Nagle, Frank and Zhou, Yanuo. 2024. The Value of Open Source Software. Harvard Business School Strategy Unit Working Paper No. 24-038. http://dx.doi.org/10.2139/ssrn.4693148. Available at SSRN: https://ssrn.com/abstract=4693148 

## Funding

**Datasets**

| Source | Description |
|:-------|:------------|
| [GitHub Sponsors](https://github.com/sponsors) | [List of dependencies for projects owned by the currently authenticated user](https://github.com/sponsors/explore) (i.e. you). CSV export available. |
| [jonathimer/awesome-oss-investors](https://github.com/jonathimer/awesome-oss-investors) | List of VCs investing in commercial open-source startups |
| [Kivach](https://kivach.org/) | "cascading funding": donations to a project redistrbuted upstream |
| [Ko-fi](https://ko-fi.com/) | |
| [Liberapay](https://en.liberapay.com/) | |
| [Open Collective](https://opencollective.com/) | transparent budgeting |
| [oss.fund](https://www.oss.fund/) | Aggregator for OSS funding opportunities, programs, and platforms |
| [StackAid](https://www.stackaid.us/) | Donations redistributed evenly across project's dependencies. Provides a helpfule [simulation of funding allocation](https://simulation.stackaid.us/projects) |
| [Secure Open Source Rewards (sos.dev)](https://sos.dev/) | |
| [ralphtheninja/open-funding](https://github.com/ralphtheninja/open-funding) | Guide to OSS funding options |

**Research**

- Boysel, S., Nagle, F., Carter, H., Hermansen, A., Crosby, K., Luszcz, J., Lincoln, S., Yue, D., Hoffmann, M., Staub, A., 2024. Open Source Software Funding Report. [https://opensourcefundingsurvey2024.com/](https://opensourcefundingsurvey2024.com/)
- Conti, A., Peukert, C. and Roche, M., 2025. Beefing IT Up for Your Investor? Engagement with Open Source Communities, Innovation, and Startup Funding: Evidence from GitHub. Organization Science.

## Surveys

- [Linux Foundation surveys](https://data.world/thelinuxfoundation?entryTypeLabel=dataset&tab=resources)
	- [2020 FOSS Contributor Survey](https://www.linuxfoundation.org/resources/publications/foss-contributor-survey-2020)
		- access: high level insights public
		- timeframe: 2020
	- [2021 Diversity, Equity, and Inclusion in Open Source](https://data.world/thelinuxfoundation/2021-diversity-equity-and-inclusion-in-open-source)
		- access: [high level insights](https://www.linuxfoundation.org/research/the-2021-linux-foundation-report-on-diversity-equity-and-inclusion-in-open-source#:~:text=Additional%20Resources-,Presentation%20Data,-Open%20Data) and [survey data](https://data.world/thelinuxfoundation/2021-diversity-equity-and-inclusion-in-open-source)
		- timeframe: 2021
	- [2022 State of Open Source Security](https://snyk.io/reports/open-source-security/)
		- In collaboration with Snyk.io
		- access: high level insights public
		- timeframe: 2022
	- [Annual Jobs Survey]()
		- access: high level insights and survey data available ([2022](https://data.world/thelinuxfoundation/2022-10th-annual-jobs-survey), [2021](https://data.world/thelinuxfoundation/open-source-jobs-report-2021))
		- timeframe: 2012-2022
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

## Source code analysis

**Datasets**

| Source | Description |
|:-------|:------------|
| [Software Heritage](https://archive.softwareheritage.org/) | Historical archive of source code |
| [NIST National Software Reference Library](https://www.nist.gov/itl/ssd/software-quality-group/national-software-reference-library-nsrl) | A collection of hashes and metadata for to uniquely identify individual files across a set of software projects. Forensic use cases include identifying software based solely on file contents, malicious elements. |

## Bounty platforms

| Source | Description |
|:-------|:------------|
| [IssueHunt](https://issuehunt.io/) | A platform for funding open source projects. |
| [Bountysource](https://www.bountysource.com/) | A platform for funding open source projects. |
| [boss.dev](https://www.boss.dev/) | A platform for funding open source projects. |

## Public policy

- [CSIS Government Open Source Software Policies](https://www.csis.org/programs/strategic-technologies-program/resources/government-open-source-software-policies)
	- Dataset of various public policy and legislation dealing with open source software from governments around the world.


## General web archives

| Source | Description |
|:-------|:------------|
| [Common Crawl](https://commoncrawl.org/) | Raw page data, metadata, and extracted text from publicly accessible segments of the internet. Timeframe: 2008 - present, monthly since March 2014. Data hosted on Amazon S3: [getting started docs](https://commoncrawl.org/the-data/get-started/) |
| [Internet Archive](https://archive.org/) | Less systematic crawls with a longer history. Access via the [Wayback Machine](https://web.archive.org/) or its [API](https://archive.org/help/wayback_api.php) |
| [Archive Team](https://archiveteam.org/) | A group of volunteers that archives web pages and other content. Data is available via the [Wayback Machine](https://web.archive.org/) or its [API](https://archive.org/help/wayback_api.php) |
| Wikipedia | [data dumps](https://dumps.wikimedia.org/enwiki/) and [SQL access](https://quarry.wmcloud.org/) |
| [Wikidata](https://www.wikidata.org/) | A free and open knowledge base that can be read and edited by both humans and machines. Data is available via the [Wikidata Query Service](https://query.wikidata.org/) or its [API](https://www.wikidata.org/wiki/Wikidata:Data_access) |
| [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) | A free media repository. Data is available via the [Commons API](https://commons.wikimedia.org/wiki/Commons:Database_download) or its [API](https://www.mediawiki.org/wiki/API:Main_page) |


## Other Resources

- [NBER Economics of Digitization](https://www.nber.org/programs-projects/projects-and-centers/economics-digitization/economics-digitization-research-projects)
- [Linux Foundation Research](https://www.linuxfoundation.org/research)
- [BigQuery Introduction for GitHub data](https://github.com/dinalav/Data-Science-Slides-and-Notebooks)
- [GitHub Data Dictionary](https://github.com/github/developer-policy/blob/data-dictionary/data_dictionary.md)
- [Google Search for Research Datasets](https://datasetsearch.research.google.com/)