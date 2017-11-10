# What does a sustainable open source project look like?

In a [recent blog post](https://medium.com/libraries-io/what-does-a-sustainable-open-source-project-look-like-bf9b8cf824f8) I wanted to articulate what a successful, sustainable open source project looks like, including what kinds of work do people do on it, and what kind of community of users and contributors it has. Then with that as an end point, we can work backwards to figure out how to bring that world to life.

Contributions and discussions are very welcome, just open an [issue](https://github.com/librariesio/sustainable-oss-attributes/issues) or a [pull request](https://github.com/librariesio/sustainable-oss-attributes/edit/master/README.md).

This document is licensed under [Creative Commons CC-BY-SA](https://creativecommons.org/licenses/by-sa/4.0/legalcode)

<hr>

So here’s the list of things that make up the ideal sustainable open source project:

## Governance
- The project has structures in place for making high-level decisions and enforcing communication standards, codes of conduct etc.
- Decisions are publicly documented and communicated to all interested parties.
- The maintainers of the project have taken steps to ensure it does not rely on any single person to be able to get work done.
- Plans for future development direction, ideas, and goals are kept up to date in a roadmap document.
- Taking steps to ensure that the project fosters a good, diverse community and is welcoming and friendly to users and contributors alike.

## Documentation
- The project has good-quality documentation, covering all the public APIs and interfaces. They are updated with each release.
- Commit messages should describe what and why the change was made as per Chris’ great guidance.
- Human-focused release notes should be published with every release, listing notable changes and deprecations.
- If possible, documentation should be available in multiple languages or at least open to contributions from translators.

## Code Quality
- Code should have a consistent style throughout the project, ideally programmatically enforced with linters and documented with style guides where necessary.
- The project should have good test coverage, with tests being run automatically on a CI environment after every commit.
- There should be a documented code review process for all contributions involving both automated checks and human approval process to keep code quality levels high.

## Support
- Contributions and support requests and should be responded to in a timely manner even if a fix isn’t possible straight away.
- Outstanding tickets should be triaged on a regular basis to ensure stale issues don’t fall through the cracks.
- If there is a long-term support release available, the policies around it should be documented and future release dates included in roadmaps.
- The project should document all supported runtime/language versions and major external dependency version compatibility, which should also have automated testing setup.
- New release candidates should be tested against as many upstream dependency versions as realistically possible to ensure backwards compatibility or enable communication of breaking compatibility changes.
- It’s also a good practise to keep an eye out for posts on Q&A sites like Stack Overflow where users often go to get support with open source projects.

## Ecosystem Collaboration
- Maintainers should identify and coordinate with related projects to reduce potential for conflicts on new releases and breaking changes
- For projects that are heavily depended upon, automated integration testing against key downstream dependencies should be set up for early warning detection of unseen breakages and conflicts.
- Projects should have a clear process for proposing and discussing large changes such as an RFC.

## Security
- There should be a documented process for privately reporting security issues to the project's maintainers as well as clear guidelines for maintainers on how to handle reported security issues.
- Projects should acquire a CVE for all known security vulnerabilities and document which released versions the CVEs apply to.
- Commits and releases should be signed by the authors so that users can verify whether what they downloaded matches the same contents you released.
- Maintainers should have 2FA and strong passwords on all related accounts (GitHub, package manager registries, email etc)
- If releases include publishing compiled binaries, there should be a provenance chain for those binaries, ideally compatible with the Reproducible Builds program.
- If necessary a threat model should be documented to highlight where the software is most vulnerable to attack and how to mitigate those threats.
- Any reports produced whilst researching the security aspects of the project should be published within a reasonable timeframe.

## Legal
- The project should be made available under one of the OSI-Approved Licenses, that’s any license that fits with the Open Source Definition.
- All licenses and trademarks for the project should be properly documented and ideally available in machine readable format like SPDX as well.
- There should be a succession plan in place in case of the death of maintainer to allow other maintainers to legally take control of the assets of the project incase the worst happens.

## Finance
- As with any entity that is dealing with money and people, correct accounting and tax reporting should be done based on the laws of the countries that the maintainers reside in.
- In some cases a legal organisation should be set up to to protect the liabilities of individuals involved, either as a regular business or a not-for-profit organisation.
- With people being paid to work on the project, potentially from a variety of countries, policies around pay rates and expenses should be set up.
- For ultimate transparency, an open ledger of all project income and outgoings could be used to show exactly how funds are being spent on the project.

## Marketing
- Having a recognizable brand can help the project build a strong audience of users and contributors, that includes having a logo and website of it’s own to help users understand what the project is about and also control the brand of the project outside of the GitHub repository page.
- Projects should aim to keep their users and contributors up to date with what’s going on with the project, including larger announcements and highlighting interesting goings on in the development process as well as sharing useful related content via an email newsletter, blogging and twitter.
- Surveys can also be a useful tool to collect quantitative and qualitative information about how and why the use the project and what else they would find useful to help inform future roadmapping decisions

## Dependency Hygiene
- If the project has dependencies it should ensure that each dependency is properly licensed and that license is compatible with the project.
- Dependencies should also be checked for any potential security or compatibilities on a regular basis, including transitive dependencies.
