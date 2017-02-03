##### Rationale

Web development has been very exciting during the past few years and new javascript technology has been popping almost every week.

With desktops being more and more powerful, the common development strategy has been to enrich client applications to enhance the user experience.

[neXtProt](https://www.nextprot.org) embraces this trend using popular client side technology such as [AngularJS](https://angularjs.org/) and [Web Components](https://www.webcomponents.org/) / [Polymer](https://www.polymer-project.org/1.0/) (library developed by Google).

Web components enable the re-use of such libaries by the bioinformatics community. This follows the strategy of the neXtProt development team that has published many libraries already in [BioJS](https://biojs.net/). The most popular one, being the [feature viewer](https://github.com/calipho-sib/feature-viewer) shown in this picture.

![DotPlot](data/projects/images/feature-viewer.png)

##### Approach

Multiple web components can be developed in the scope of the Google Summer of Code 2017. The following examples, show visualizations that should be replaced by web components.

-	[Ancestor Graph](https://www.nextprot.org/term/TS-0079/parentGraph) (could be done in combination with [D3](https://d3js.org/)\)
-	[Tree browser](https://www.nextprot.org/term/TS-0564/browser)
-	[Genome exons visualisation](https://www.nextprot.org/entry/NX_P52701/exons)

##### Challenges

-	Organizing and testing a maintainable code
-	Integration of web components in [www.nextprot.org](https://www.nextprot.org) website with AngularJS
-	Publish to [BioJS](https://biojs.net/) and [Web Components](https://www.webcomponents.org/)

##### Requirements

-	The student should have some knowledge of html and javascript.
-	Polymer, AngularJS and D3 are a plus.
