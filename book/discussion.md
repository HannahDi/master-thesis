<div style="page-break-after:always;"></div>

# Discussion

TODO
* FAIR: Publication on GitHub, Zenodo, DaRUS
* Combination with other Modelling Tools, inside or outside of Jupyter Notebook, e.g. Copasi, PySCeS
* Most software is proprietary must be bought, is not always available -> makes reproduction hard
* Often the software is a black box, users often don't know underlying algorithm  
* often more than one software needed for different steps -> copy paste between these -> error prone (eg Excel -> Origin Pro -> written paper)
* Information losses: initial rates (no information of curve), 
* data can be scattered eg over several excel files
* Combination of code and explanatory text, given in Notebooks but not in Excel or other data-formats
* Problems with initial rates: no convention on which part of the time-course to take for calculation: - from beginning till arbitrary time (seconds or minutes later) vs - linear part of curve with sense of proportion again of arbitrary length
* even data formats like enzymeml can never be 100% complete for all scenarios: eg for now no information on modelling, no information on conversion from absorbance to concentration... these are all stored in Jupyter Notebook if this is used for these steps
* Problems that can't be solved: if experimenter decides to no save all data, but just the nice experiments, but hope to give incentive to report all data especially raw data such es absorbance
* Problem with Jupyter Nb: git diff not working very well with the json schema and all the metadata, but in Jupyter Notebook classic environment already a git nbdiff button, shows diff with only changes inside the code cells
* more and more common to share JNbs especially with Colab (Johann and Frank did this to show how to run their modelling tools)