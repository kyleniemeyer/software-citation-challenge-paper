# software-citation-challenge-paper
Short challenge paper on challenge of software citation for *ACM Journal of Data and Information Quality* 

Outline:

1. Make the case for the importance and challenge of software citations
    - Importance: modern science & engineering relies heavily on software, but currently no accepted standard for crediting the efforts that go into such software akin to paper citations. Furthermore, since research results depend on specific software used (including the version), proper citation is necessary to ensure reproducability. 
    - Challenge: different communities have widely varying practices for citing software, with guidelines ranging from suggesting citations of associated software papers or the software directly via DOI (e.g., [American Astronomical Society](http://journals.aas.org/policy/software.html)) to no policy at all. Related challenge: some research communities have not yet adopted open-source mentality regarding research software. In addition, big questions about curating/reviewing software---if software will be cited at the same level as journal publications, should software go through peer code review? If so, how?
    - As a first step towards correcting the research software credit problem, ongoing efforts to establish citation practices for software used in research
2. Briefly discuss ongoing efforts in this area
    - WSSSPE & FORCE11 working group efforts to standardize citation practices; mention that some of these recommendations come from these groups
    - Codemeta: minimal metadata needed to cite software
    - Register DOI for software through Zenodo or fig**share**; the former has streamlined process for registering DOI for GitHub software releases.
    - similar efforts to standarize research data citation by DataCite and FORCE11 Data Citation Synthesis Group [*Joint Declaration of Data Citation Principles*](https://www.force11.org/datacitation)
    - Complementary efforts to provide credit for software development work in research
        * transitive credit via JSON-LD: assigns varying credit weights to contriponents---both contributors and research components, including software and data---depending on level of importance to the work.
        * [CRediT taxonomy](http://casrai.org/CRediT) for contributor roles includes a "software" category; related [Mozilla PaperBadger](https://badges.mozillascience.org/) project offers digital contributorship badge associated with each role. These associate roles for papers (identified via DOI) with people (identified via ORCID).
3. Our recommendations and remaining research challenges
    - Two (three? four?) main challenges: 
        * Standardize software citation format for scientific publications
        * Establish mechanism for software to cite other software
        * Develop infrastructure to support indexing of software citations akin to publication citation ecosystem
        * (Dan) depending on what we decide on the overall theme, I think we need to mention peer review as a challenge 
    - Metadata needed for software to be cited: software name, DOI, authors/contributors (with names & ORCIDs), software dependencies (ideally in form of DOIs), and any other people/artifacts that would be cited or acknowledged in a paper. This information should be provided in CITATION file, potentially in JSON or XML formats (rather than plaintext) to allow automatic processing/parsing.
    - Although citation format may vary based on the particular style of journals, conferences, or professional societies, at minimum citation of software in publications should include: software name, primary authors/contributors, DOI or other unique identifier, and location where software can be found (DOI or URL).
    - Additional research/efforts needed:
        * How to cite closed-source/commercial software? Can the above information be provided?
        * Indexing of software citations to create citation network akin to that of publications (e.g., Web of Science, Scopus, Google Scholar).
        * How to indicate direct use of software for research in citations, where results would not be possible without efforts of software authors? Should this citation be "weighed" higher than others? AAS suggests new "Software" section below acknowledgements: http://journals.aas.org/policy/software.html; other approaches include transitive credit.
        * Should citable software go through peer code review, and if so how can this be implemented/who would manage? Or, should citable software follow the arXiv model, with software "advertising" papers going through peer review in a relevant community?