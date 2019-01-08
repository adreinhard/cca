# cca
CCA Github ReadMe
Andrew Reinhard
January 8, 2019

The files included in this repository and its subdirectories were either used or created by Andrew Reinhard in his Colossal Cave Adventure case study for the archaeology PhD at the University of York (UK). The goal of the case study was to determine if is possible to conduct stylometric and text analysis on game-code, and to see if any meaningful conclusions could be drawn from the resulting data. Users of this repository are welcome to use the tools, files, and data to either reproduce or challenge Reinhard’s results, or to use them for other text analysis projects with code.

CCA Full Versions (subdirectory):

This subdirectory contains all of the various full versions of Colossal Cave Adventure as downloaded from the Adventure Family Tree website maintained by Nathanael CJE Culver. At the time of this repository’s creation, his latest update was on November XXX, 2017. Most of the files in this subdirectory are compressed and can be extracted with WinZIP, WinRAR, B1 Free Archiver, and other utilities for either Macs or Windows computers. Once extracted, many files can be read with a simple text editor. Filenames correspond to the names assigned to each version by Culver and are widely used by the CCA community to cite these derivative works.

CCA Corpora (subdirectory):

In order to use the three statistics packages for R against Colossal Cave Adventure files, these files needed to be prepped by saving them as TXT files (simple text) and dividing them into three sets of corpora for analysis:

FORTRAN Corpus: 12 FORTRAN files containing CCA source code from separate versions of the game written between 1975 and 2017.

Narrative Data Corpus: 38 files containing nothing but the narrative data from versions of CCA that used a file separate from the source code file(s) containing hint text, legal vocabulary, and exposition.

ReadMe Corpus: 48 versions of CCA came bundled with ReadMe files written by each version’s author. ReadMe files often contained installation and gameplay instructions, the author’s name and contact details, and sometimes a brief history of CCA.

R Packages and Data (subdirectory):

This subdirectory contains the installation files and instructions for the tools I used to conduct text and stylometric analysis on versions of CCA. It also contains the CSV files with CCA data used in those packages, as well as visual output. All files pre-date the creation of this repository on January 8, 2019.

Gephi: Installation information for this app and a subdirectory for data files and output split into six additional subdirectories based on visualizations of CCA data returned in both Stylo and TextReuse. The Gephi application was created in 2010 by students at the University of Technology of Compiègne in France, which is now managed by the non-profit Gephi Consortium and open source user community. The program is a network analysis and visualization tool further developed over several years by additional students at the annual Google Summer of Code event.

R: Installation package for R statistics software. R is a statistics programming environment and language largely replacing S as the modern standard for data analysis and statistical computing. Originally written by Ross Ihaka (statistical computing) and Robert Gentleman (bioinformatics) of the University of Auckland in 1993, R is now overseen by various international consortia and user groups (including R-Ladies to promote gender diversity in the R community), has its own peer-reviewed journal, and a curated open source archive (CRAN) for user-created, mission-specific packages based on an R backbone. This open source community (like other open source groups) self-polices and vets R code and packages.

Stylo: Installation file and instructions for installation and use, plus returned stylometric CCA data. Stylo was created in August 2015 by Maciej Eder (Institute of Polish Language, Polish Academy of Sciences), Jan Rybicki (Institute of English Studies, Jagiellonian University), and Mike Kestemont (Department of Literature, Antwerp University), for the purpose of using R to determine authorship attribution through stylometric analysis. 

TextNets: Installation file and instructions for installation and use, plus returned data sets and visualizations of CCA versions. Chris Bail is an Associate Professor of Sociology and Public Policy at Duke University where he also directs the Polarization Lab. His Textnets package for R allows one to detect and visualize networks of documents and authors based on the examination of a corpus of texts.

TextReuse: Installation file and instructions for installation and use, plus returned text analysis CCA data. Lincoln Mullen developed TextReuse for R in 2015 as a way to measure similarity among documents and detecting passages that have been reused between them. Mullen currently holds a dual appointment at George Mason University as Assistant Professor in the Department of History and Art History, and Director of Computational History at GMU’s Roy Rosenzweig Center for History and New Media. Originally created to compare 19th-century legal documents, TextReuse can be applied to any corpus of documents to see what (and how much) text was borrowed, shared, or plagiarized.

ExifTool: The ExifTool allows users to extract metadata from a variety of files, largely digital images. It was created in 2005 by Phil Harvey of Queens University’s (Canada) Department of Physics, who currently manages its imaging project for the Sudbury Neutrino Observatory. 

table2list.xla: Visual Basic macro created by Michael Tanne used in Microsoft Excel to translate Stylo and TextReuse table data into a list that can be more easily used by the Gephi data visualization software

Contact

If you have questions or want to share your own CCA stylometric and text analysis results with me, please email adr520@york.ac.uk.
