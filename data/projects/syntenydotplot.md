##### Rationale

Synteny is the conservation of gene order between chromosomes that descended from a common ancestor. Thus, visualization of synteny is a cornerstone in comparative genomics, and is essential with the abundance of genome sequences available. Dot plots are one of the most widely used methods to visualize synteny, by which the chromosomal locations of “orthologs”—corresponding genes between 2 species—are plotted. This allows for visualization of overall gene order conservation. But since inversions and translocations can substantially vary in size (from a few base pair long to millions of base pair long), the visualisation needs to be interactive—allowing for exploration of the data at multiple resolutions.

The [OMA (Orthologous Matrix) database](http://omabrowser.org/) is a leading bioinformatic resource of evolutionary relationships between genomes. The goal of this project is to use the pairwise orthologs predicted by OMA to create an interactive dot plot to display synteny between chromosomes. This web tool will be incorporated into OMA’s web browser, and will have a variety of features by which the user can customize their analyses. Several thousand researchers access the OMA resource every month, so new features can make a considerable impact.

![DotPlot](data/projects/images/syntenydotplot.png)

##### Approach

A prototype for the interactive synteny dot plot has already been made, but will be developed further by the summer intern. For this s/he will use Bokeh, a Python visualization library, to create an interactive synteny visualizer to be implemented the OMA browser. The candidate will retrieve the data from an HDF5 database and implement features including:

-	Display orthologs from either a pair of chromosomes or genomes
-	Filter orthologs based on a variety of metrics, including substitution rate, evolutionary distance, relationship cardinality, synteny and score
-	Selecting or hover over points on dot plot to export information
-	Apply a color scale to points based on user-selected features

##### Challenges

Javascript may be needed for customization beyond what is available with the bokeh library.

##### Requirements

The intern should have moderate to advanced knowledge in Python, and JavaScript is a plus. Web design and development skills are needed. Creativity for new features and ways to visualize the data available are also a plus.
