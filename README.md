<!--
SPDX-FileCopyrightText: 2022 Martin Haeuer <martin.haeuer@ose-germany.de>
SPDX-FileCopyrightText: 2022 Nicolas Traeder <nicolas@konek.to>
SPDX-FileCopyrightText: 2022 Robin Vobruba <hoijui.quaero@gmail.com>

SPDX-License-Identifier: CC0-1.0
-->

[![REUSE status](
    https://api.reuse.software/badge/github.com/OPEN-NEXT/LOSH-Reporter)](
    https://api.reuse.software/info/github.com/OPEN-NEXT/LOSH-Reporter)

# LOSH-Reporter

The LOSH reporter is couple of files that,
given the [LOSH OKH RDF data](https://gitlab.opensourceecology.de/verein/projekte/losh-rdf/),
produce a human-readable report
with statistical diagrams about selected aspects of the OSH projects,
together with some manually written prose around it.

Technolog wise,
it is Jupyter-Lab (ex Jupyter-Notebook) based.
It runs as a headless CLI script,
though one would usually [edit the template](#edit-the-template)
in the Jupyter-Lab Web UI.

The LOSH reporter generates its report
simultaneously in Markdown, PDF and HTML reports.

## Supported OSH Platforms

- [Wikifactory.com](https://wikifactory.com/)
  - per API
- [OSHWA Certification List](https://certification.oshwa.org/list.html)
  - per API
- [Thinigverse.com](thingiverse.com)
  - per API (+ workaround due to [#xxxx](URL-TO-TICKET))
  - We needed to be _very_ economical with data fields here,
    since due to API bugs,
    we can't filter their database –
    we're checking out _every_ thing on thingiverse
    and every datafield is a new request.
    There are 5+ Mio. things on Thingiverse
    × the number of data fields
    → you can do the math :)
- [GitHub.com](https://github.com/)
  - per global search for manifest files
- [Appropedia.org](https://appropedia.org/)
  - per script, exporting manifest files to GitHub.com
- [OKHv1](https://www.internetofproduction.org/open-know-how)
  - per script, exporting manifest files to GitHub.com

Note on other platforms:

- [GitLab.com](https://gitlab.com/)
  - does not yet support global file search
    ([#2263](https://forum.gitlab.com/t/search-code-across-all-projects/2263),
    [#14597](https://gitlab.com/gitlab-org/gitlab-foss/-/issues/14597)),
    which is a blocker for crawling.
    we currently only have manually indexed projects from this platform.

## Edit the template

1. Install [Jupyter-Lab](https://jupyter.org/)
2. Run it, and open the report file: `jupyter-lab report.ipynb`

Comment:

- While the report speaks of OSH _projects_,
  the `OKH-LOSH` specification defines OSH `modules`.
  In data specifications in this repo,
  we'll use the `OKH-LOSH` notion.
- If not otherwise noted, numbers refer to modules,
  _ignoring their different versions_.
- …hence calculations are (if not otherwise noted) run on the total LOSH data

## Installation

### Data server

To test and run the reporter locally
you can use a dockerized Apache Jena instance.

Start the Apache Jena database with `docker-compose up` within the `fuseki` folder.

### Environment variables

To start the reporter this environment variables need to be set:

- `FUSEKI_URL`
- `FUSEKI_DATASET_NAME`

An example can be found in `.env.example`.
Those values can be used for development.

## Running the reporter

Run the BASH shell script `generate`,
and the generated reports will appear in the _output_ folder.

## License

The LOSH Reporter is licensed under GPL-3.0-or-later,
the generated reports are licensed under CC-BY-4.0.

## References

- OKH-LOSH specification: <https://github.com/OPEN-NEXT/OKH-LOSH/>
- LOSH-Krawler: <https://github.com/OPEN-NEXT/LOSH-Krawler/>
- the raw data of LOSH (RDF): <https://gitlab.opensourceecology.de/verein/projekte/losh-rdf>
- Jena-based test implementation: <https://github.com/OPEN-NEXT/LOSH-RDF-DB-tester>
