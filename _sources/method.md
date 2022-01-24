# Methodology 
_The EnzymeML format and toolbox_

EnzymeML is a machine-readable data exchange format to document enzymatic data, based on the Systems Biology Markup Language (SBML) {cite}`sbml_2003`, in compliance with the STRENDA guidelines {cite}`strenda_2014`. It aims to store all relevant metadata of an experiment, information on the involved enzymes together with measured results such as time-course data of substrate and product concentration {cite}`enzml_2_2021`, thus enabling the seamless exchange of data between experimentalists, modellers and databases as shown below. 

```{figure} ../images/Fig1.png
---
name: fig1
---
Schematic representation of the EnzymeML data format as a link between experimental platforms, modelling platforms and publication platforms.
```

EnzymeML is not meant to be read by humans but comes with a toolbox. One crucial software is PyEnzyme {cite}`pyenzyme_2021`, a Python package to read, write and edit EnzymeML. PyEnzyme can easily be integrated into every Python program and used inside a Jupyter Notebook. In addition, EnzymeML provides an application programming interface ([API](https://enzymeml.sloppy.zone/)) with a RESTful interface, offering the same functions as PyEnzyme. 

_Jupyter Notebooks_

Jupyter Notebook is an application to develop code in a low-entrance level environment. It was first introduced by the project [Jupyter](https://jupyter.org/) in 2015. In contrast to other development environments, a Jupyter Notebook is structured into various kinds of cells. Aside from the code cells containing the executable code, it offers markdown cells for descriptive text, equations, and images. This structure makes it possible for non-programmers to follow the code. In addition, Jupyter notebook unfolds its full strength in the ecosystem of sharing platforms such as [GitHub](https://github.com/about), Binder{cite}`binder_2018`, [Notebook Viewer](https://nbviewer.org/), and Google Colaboratory {cite}`colab_2019`, where developers can share their files for others to use. Furthermore, Colab and Binder lower entry barriers by providing cloud servers to run notebook files online without installing anything on a local machine. Thus, everyone with the link to a notebook file can run it and generate desired output without any prior programming experience. Links to Binder are also incorporated into the website version of this Jupyter Book.

_Implementation_

Jupyter Notebooks can run various programming languages, but the most common is Python, which is well established in the research community and comes with many packages for data transformation, visualisation and computation. All scenarios in this work are programmed in Python and use PyEnzyme. Data transformations are done with NumPy {cite}`numpy_2020` and pandas {cite}`pandas_2010`, which offer data structures for easy visualisation and calculation. The visualisations are plotted with Matplotlib {cite}`matplotlib_2007`, and tables are rendered from pandas data frames. Finally, the analysis with parameter estimation is done with SciPy {cite}`scipy_2020` and lmfit {cite}`lmfit_2021`, which offer many statistical functions, such as linear regression and minimisation methods. 

_Written report_

This report was written as a Jupyter Book {cite}`jupyterbook_2020`, consisting of markdown files and Jupyter Notebooks. From these, a website is automatically built and hosted as a GitHub page. In addition, Jupyter book provides the functionality to generate a LaTex file, which is only slightly edited for the final pdf. 