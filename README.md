# Place-the-Title-of-Your-Thesis-Here

This LaTeX package is used to create theses at Carleton University.

Important to Note

* In the FINAL submission No internal links is allowed in the thesis final-PDF.
* They can be disabled by commenting-out the hyperref[--option--] {} in the "SBNth.sty" file!
* Keeping it is helpful in the writing process though!
* The acknowledgments, preface, contributions, and dedication sections are not required, but the ABSTRACT section is.


Sections in the Thesis:
The following sections will mainly be created automatically:
1) Title page, Will be generated automatically
2) Signature page, Do not worry about this Department will take care of it!
3) Abstract Mandatory
4) Dedication Page Optional
5) Acknowledgments Optional
6) Preface Optional
7) Table of Contents
8) List of Tables
9) List of Figures
10) List of Acronyms
11) List of Symbols
12) Chapter 1: Background and Preliminaries
23) Chapters 2, 3, 4, ...
24) Chapter x: Conclusions and Future Work
25) List of References
26) Appendix 1,...



Options for cuthesis.sty:
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
This LaTeX package is used to create theses at Carleton University.
-- It has several options which are described below.
-- Multiple options can be included as a comma separated list.
-- See the examples for common uses.

Options:
-------
manuscript,standard: this specifies which format of thesis you will be creating. Manuscript format has the references at the end of each chapter, while standard format has one reference section for the whole document. standard is the default.

N.B.: Do NOT use ``Manuscript'' for the final submission. It may be useful if you are editting your thesis chapter-by-chapter

phd,masters: this specifies whether this is a PhD. dissertation or a masters thesis. masters is the default.

-- 1committee, 2committee, 3committee,4committee,5committee: 
this is the number of people on your committee (in addition to the department chair), which determines how many signature lines are needed. Remember that the chairman of the committee does not sign the thesis.
*** 1committee is the default.
NOTE: Due to the recent change (2019) to the theses handeling process the ``SIGNATURE PAGE'', including the committee, will be taken care of by the departments graduate secretary, so do NOT worry about this. Also, leave it to be the default value!

-- sequential,nonsequential: 
this specifies whether you want numbering of figures, equations, and tables reset to 1 at the beginning of each chapter (nonsequential), or if you want the numbers to be sequential throughout the whole document. The default is nonsequential for Manuscript format and sequential for Standard format.

N.B.: I found ``nonsequential'' prefereable as it makes it easier to trance the figures ... Since CU has not explicitly mentioned any specific standard for this option Following our preference and in favor of legibility, we set this option to nonsequential. (Dec.2020, Behzad)

*** Examples:

    ---------

For a standard format masters thesis:  \usepackage{cuthesis}

NOTE: Carleton does nor use the word Dissertation!

For a manuscript format PhD. dissertation: \usepackage[manuscript,phd]{cuthesis}
For a standard format PhD. dissertation with a four member committee: \usepackage[phd,4committee]{cuthesis}

*** Notes:
    ------
(1) The acknowledgements, preface, contributions, and dedication sections are not required, but the ABSTRACT section is.

(2) By default the department named on the title page is ``Department of Electronics'', but that can be changed by putting the command: \dept{My Department} in the main .tex file before any of the chapters are included.

(3) bibliography:
   (a) In compliance with the Carleton University Library's biblical Format the ``ieeetran.bst'' (IEEE Transactions) bibliography style is used. Generally, it is a part of    
       standard MikTeX distribution, and we do not to include it in our files.
   (b) It uses the same fontsize (10pt/12pt) defined in \documentclass[]().
