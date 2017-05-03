# Zenodo Best Practices for the CIG Community

zenodo.org

CIG recommends that all developers and researchers obtain DOI's (digital object identifiers) for all of their research products.  This includes software, data, and model data.

You may use your github account or orcid account as login.

CIG maintains a zenodo community.  Search for: Computational Infrastructure for Geodynamics" or simply on the word 'geodynamics"

## Executive Summary

This document has three parts:
* **Creating Web hooks**. Creating a zenodo entry automatically when issuing a new release.
* **Manual Upload**.  For older versions or other files and datasets.
* **Metadata**. Guidelines for assigning metadata.

## Things You Should Know

Once a file has been uploaded and assigned a DOI it CANNOT BE CHANGED. You will not be able to add more files or edit the files in the repository.

You CAN edit the metadata.

## Creating Web Hooks
 
By creating a webhook into your repository, a zenodo entry will automatically be created with each new release.

Please see the github guide: https://guides.github.com/activities/citable-code/

Assign metadata using the guidelines below

## Manual Upload

1. **Login**
  1. Use your GitHub or ORCID account or create a new login.
2. **Upload**
1. Click on "Upload" on the browser header (between search bar and *Communities*).
  2. Click on "New Upload" - green button on upper right hand side of window.
Note that your previous data packages are also shown. You can select these and edit your metadata.
3. Drag and drop your files into the window or choose files as directed.

See next section on Metadata

## Metadata

Please use the following guidelines when assigning metadata. 

1. **Upload type**
 1. Please assign software to all github releases.  There is a known BUG in the the display of this metadata field. In the citation field, this displays as "dataset". Zenodo promises it will be fixed in the next release.
2. **Basic Information**
  1. Reserve a DOI only when you are sure you are not changing, adding or deleting to the uploaded files.
  2. Description.  Please add an informative description of the software and changes to this release.  This is what the user will see.
3. **License**
  1. All CIG codes are "Open Access"
  2. Please search for the correct "License". Most CIG codes are "GNU General Pubic License 2.0"
4. **Communities**
  1. Please assign the community "Computational Infrastructure for Geodynamics". Sometimes you need to type in most of the string before zenodo finds it.
5. **Funding**
  1. If you are FP7 and Horizon 2020, your grant will be available here. If not, add funding acknowledgements in *Additional Notes*.
Addition of NSF grants is a feature coming soon!
6. **Related/alternate identifiers**
  1.  Add geodyanmics.org/software/*CodeName* as "references this upload"
  2.  Add the github repo e.g. https://github.com/geodynamics/aspect/tree/v1.5.0 as "Supplement to"
7. **Contributors**
Please don't forget to acknowledge others who contributed to this research product.
8. **References**
Add references you want users to cite here.
9. **Journal, Conference, Book/Report/Chapter, Thesis**
If this research product is part of one of the above, add the reference here.
 
When you are ready do not forget to **Publish** or just remembmer to **Save** your work.

Please feel free to add to these instructions.