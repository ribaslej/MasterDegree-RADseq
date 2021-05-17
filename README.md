Repository IN CONSTRUCTION............\
\
THIS REPOSITORY AIMS TO AGGREGATE SERIES OF METHODS APPLIED ON RADseq DATA OF A SUBTERRANEAN RODENT FOR MY CONTROL AND FOR WHO IT COULD HELP.\ 
THE MAJOR OBJECTIVE WAS TO ANALYSE DE GENETIC STRUCTURE OF A SPECIES THROUGHOUT THE DISTRIBUTION AS WELL AS EVOLUTIONARY HISTORY.

<h1> RADseq ANALYSIS </h1>\
\
<h2> 1. RAW DATA </h2>\
<h2> 2. QUALITY FILTERING </h2>\
<h2> 3. ANALYSIS </h2>\

<h2> 1. RAW DATA </h2>
    <h3>Raw data files received from the sequencing company was assembled using Stacks software via remote platform Galaxy: usegalaxy.eu</h3>
    <h3>Several combination of parameters was tested to achieve the optimal parameters, visualized with custom R scripts based on logfiles</h3>
\
<h2> 2. QUALITY FILTERING </h2>
    <h3>Assembled loci and variants were filtered to exclude those with low coverage and those that did not conform between 90% confidence interval</h3>
    <h3>Loci with variants that did not follow Hardy-Weinberg equilibrium in at least one population were excluded, as well as those with Minimum Allelic Frequency < 0.5</h3>
    <h3>Filters were applied using both vcfR and pegas package. Only one variant per sequence was retained</h3>

<h2> 3. ANALYSIS </h2>
    <h3> 1. EXPLORATORY ANALYSIS - Principal Components, Clusterization Algorithms, Non-negative Matrix of Factorization</h3>
    <h3> 2. OUTLIERS DETECTION - Detect outliers that could represent loci deviating from neutral expectation by selection pressures</h3>
    <h3> 3. SUMMARY INDEXES OF DIVERSITY - Basic stats, distance measures and coancestry matrix</h3>
    <h3> 4. PHYLOGENETIC RELATIONSHIPS - Minimum Spanning Network, Distance tree, Parsimony tree and Maximum-Likelihood tree</h3>
    <h3> 5. GEOGRAPHIC DISTANCE - Correlation of genetic and geographic distances and MonMonier algorithm</h3>
    
    <h3> Analysis were ran through adegenet, fpc, LEA, PCAadapt, hierfstat, phangorn and poppr packages. BayeScan was ran through command-line</h3>