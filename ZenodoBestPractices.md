# Zenodo Best Practices for the CIG Community

[zenodo.org](https://zenodo.org)

CIG recommends that all developers and researchers obtain DOI's (digital object identifiers) for all of their research products.  This includes software, and observational and model data.

You may use your github account or orcid account as login.

CIG maintains a zenodo community at https://zenodo.org/communities/geodynamics.  Search for: "Computational Infrastructure for Geodynamics" or simply on the word "geodynamics"

Update: zenodo began supporting versioning on May 30, 2018. Please see their blog post and FAQs for more information.
* http://blog.zenodo.org/2017/05/30/doi-versioning-launched/

## Executive Summary

This document has three parts:
* **Creating Web hooks**. Create a zenodo entry automatically when issuing a new release.
* **Manual Upload**.  Uploading older versions of software packages or other files and datasets.
* **Metadata**. Guidelines for assigning metadata.

## Things You Should Know

Once your files have been uploaded and assigned a DOI the submission CANNOT BE CHANGED. You will not be able to add more files or edit the existing files.

You CAN edit the metadata.

## Creating Web Hooks
 
By creating a webhook into your repository, a zenodo entry will automatically be created with each new release. If versioned from a previous entry, the versions will be automatically associated. 

You will still need to:
* assign your code to the CIG community
* check your authors lists especially if all commit'ters are not considered authors for your project

Please see the github guide: https://guides.github.com/activities/citable-code/

Assign metadata using the guidelines below.

Metadata assignment can be overridden using a .zenodo.json file. This feature has not been officially released.

Please check records to ensure that metadata is correct.

## Manual Upload

1. **Login**
   * Use your GitHub or ORCID account or create a new login. Using GitHub will automatically associate it with your repository.
2. **Create**
   * Click on "Upload" on the browser header (between search bar and *Communities*).
   1. _**Adding a New Package**_
      * Click on the "New Upload" button on upper right hand side of the page.
   2. _**Adding a New Version to an Existing Package**_
      * Select the package from your Uploads directory. Click on "New Version".

At any time, you can select an uploaded package and edit its metadata. However, you CANNOT change the package's files without creating a new version.

3. **Upload**
   * Drag and drop your files into the window or choose files as directed.

Then proceed to the Metadata section.

## Metadata

Please use the following guidelines when assigning metadata. 

1. **Upload type**
   * Please assign "software" to all github releases.  There is a known BUG in the the display of this metadata field when viewing. In the citation field, this displays as "Data Set". Zenodo promises it will be fixed in the next release.
2. **Basic Information**
   * Add the mandatory data.
   * Reserve a DOI only when you are sure you are not changing, adding or deleting to the uploaded files.
   * Authors. WEBHOOK USERS: When generating a zenodo release using a webhook, the default is to assign all commit'ers as authors.  Default behaviors can be overridden using .zenodo.json file in the main directory. See PyLith and ASPECT for examples.
   * Description.  Please add an informative description of the software and changes to this release.  This is what the user will see.
   * Additional Notes. Add acknowledgements including funding here.
3. **License**
   * All CIG codes are "Open Access"
   * Please search for the correct "License". Most CIG codes are "GNU General Pubic License 2.0".
4. **Communities**
   * Please assign the community "Computational Infrastructure for Geodynamics". Sometimes you need to type in most of the string before zenodo finds it.
5. **Funding**
   * Choose from pick list of European and Australian funding agencies and NSF to add funding acknowledgements. If your grant is not listed, add it in *Additional Notes*.
6. **Related/alternate identifiers**
   * Add geodyanmics.org/software/*CodeName* as "references this upload"
   * Add the github repo e.g. https://github.com/geodynamics/aspect/tree/v1.5.0 as "is a supplement to this upload"
7. **Contributors**
   * Please don't forget to acknowledge others who contributed to this research product.
8. **References**
   * Add references you want users to cite here.
9. **Journal, Conference, Book/Report/Chapter, Thesis**
   * If this research product is part of one of the above, add the reference here.
 
When you are ready do not forget to **Publish** or just remember to **Save** your work.

Once you have published the release to Zenodo, a new DOI will be minted. Don't forget to add the DOI to the GitHub release!
* Clicking on the DOI badge on the Zenodo page will present copiable Markdown text (and other formats) that can be placed in the GitHub release text to display the badge on GitHub.

Please feel free to add to these instructions.
