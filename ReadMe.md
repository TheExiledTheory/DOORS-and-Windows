# Introduction
The following is a proof of concept or initial idea template for creating a DXL extension to be embedded directly into IBM's Rational DOORS utility which will allow for quickly parsing markdown and either editing or creating new modules. 

### 1. Process a markdown file. 
The utility must be able to parsing through a markdown file to find relevant fields. 

*There should be some standardized fields of data that are uniform across all input markdown files. Would also be useful if it indicated whether it was a change to existing reqs. or new reqs.*

### 2. Collect and track all changes/additions 

The utility should identify all requirements extracted from the markdown. 

### 3. Determine if the requirements exist already

The utility should search either the entire database structure or a particular subset of modules to determine whether or not the requirement unique identifiers exist. 

### 4. Use DOORS functions to either edit or create a module based off the data. 

The utility should then make the necessary changes inside of doors. 

*Ideally if a modification is happening, the user will be present with a viewable window of both new and old to diff.*


> PS: 
As seen in this [github](https://github.com/Mavrikant/DOORS-DXL-Scripts/tree/main "Open github") It seems to be a matter of simply dragging and dropping the dxl scripts into the installation folder for them to be recognized. I think the easiest thing to do would be to use a simple python installer which will find the users install location and copy the files down either from a remote or local repo. 


# Docs & help
* [IBM documentation](https://www.ibm.com/docs/en/engineering-lifecycle-management-suite/doors/9.7.0?topic=dxl-library)
* [TheCloudStrap](https://thecloudstrap.com/doors-dxl-tutorial-part-1/)
