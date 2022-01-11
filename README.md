# LOSH-Reporter

A locally executable script + Apache Jena + Queries to generate (mostly statistical) reports on LOSH data in MD + PDF &amp; HTML exports

## Supported OSH-Platforms

- [Wikifactory.com](https://wikifactory.com/)
	+ per API
- [OSHWA Certification List](https://certification.oshwa.org/list.html)
	+ per API
- [Thinigverse.com](thingiverse.com)
	+ per API (+ workaround due to [#xxxx](URL-TO-TICKET))
- [GitHub.com](https://github.com/)
	+ per global search for manifest files
- [Appropedia.org](https://appropedia.org/)
	+ per script, exporting manifest files to GitHub.com
- [OKHv1](https://www.internetofproduction.org/open-know-how)
	+ per script, exporting manifest files to GitHub.com

Note on other platforms:

- [GitLab.com](https://gitlab.com/)
	+ does yet not support global file search ([#2263](https://forum.gitlab.com/t/search-code-across-all-projects/2263), [#14597](https://gitlab.com/gitlab-org/gitlab-foss/-/issues/14597)), which is a blocker

## How to read the template

- `TEMPLATE.md` is the template for the report to be generated
- `$dataField` is to be replaced by the value of the referenced data field
- diagrams are referenced using the `pandoc-fignos` syntax: inline in the text with `@fig:someRef` and directly under the diagram with `{#fig:someRef}`

Comment:

- While the report speaks of OSH _projects_, the `OKH-LOSH` specification defines OSH `modules`. In data specifications in this repo we'll use the `OKH-LOSH` notion.
- If not otherwise noted, numbers refer to modules, _ignoring their different versions_.
- …hence calculations are (if not otherwise noted) run on the total LOSH data

## References

- OKH-LOSH specification: <https://github.com/OPEN-NEXT/OKH-LOSH/>
- LOSH-Krawler: <https://github.com/OPEN-NEXT/LOSH-Krawler/>
- the raw data of LOSH (RDF): <https://gitlab.opensourceecology.de/verein/projekte/losh-rdf>
- Jena-based test implementation: <https://github.com/OPEN-NEXT/LOSH-RDF-DB-tester>
