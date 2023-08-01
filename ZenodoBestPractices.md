# Zenodo Best Practices for the CIG Community

[zenodo.org](https://zenodo.org)

CIG recommends that all developers and researchers obtain DOI's (digital object identifiers) for all of their research products.  This includes software, and observational and model data.

You may use your github account or orcid account as login.

CIG maintains a zenodo community at https://zenodo.org/communities/geodynamics.  Search for: "Computational Infrastructure for Geodynamics" or simply on the word "geodynamics"

Update: zenodo began supporting versioning on May 30, 2018. Please see their blog post and FAQs for more information.
* http://blog.zenodo.org/2017/05/30/doi-versioning-launched/

## Executive Summary

This document has five parts:
* **Things You Should Know**.  Words of caution and advice.
* **Creating Web hooks**. Create a zenodo entry automatically when issuing a new release.
* **Manual Upload**.  Uploading older versions of software packages or other files and datasets.
* **Metadata**. Guidelines for assigning metadata.
* **Save or Publish**. Once Publish'ed, you cannot add to or delete uploaded files.

## Things You Should Know

Once your files have been uploaded and _Publish_'ed, the submission CANNOT BE CHANGED. You will not be able to add more files or edit the existing files. Save the record instead if you might upload additional files.

You CAN still edit the metadata after Publishing.

If you embed the software DOI in the documentation (_recommended_), you can reserve a DOI before publishing.  On the upload page under Basic Information and Digital Object Identifier click the _Reserve DOI_ button. This will not register the DOI, nor will it publish your record so you can still update the files in your repository. See Zenodo FAQs under _General_ for more information: [help.zenodo.org](https://help.zenodo.org/)


Don't forget to add the DOI to the GitHub release!
* Clicking on the DOI badge on the Zenodo page will present copyable Markdown text (and other formats) that can be placed in the GitHub release text to display the badge on GitHub.

## Creating Web Hooks

By creating a webhook into your repository, a zenodo entry will automatically be created with each new release. If versioned from a previous entry, the versions will be automatically associated.

You will still need to:
* Assign your code to the CIG community.
* Check your authors lists especially if all committers are not considered authors for your project.
* If you embed the software DOI into your documentation, DO NOT USE this feature in conjunction with _Reserve DOI_.

Please see the github guide: https://guides.github.com/activities/citable-code/

Assign metadata using the guidelines below.

Metadata assignment can be overridden using a .zenodo.json file. This feature has not been officially released.

Please check records to ensure that metadata is correct.

## Manual Upload

1. **Login**
   * Use your GitHub or ORCID account or create a new login. Using GitHub will automatically associate it with your repository.
2. **Create**
   * Click on "Upload" on the browser header (between search bar and *Communities*).

    A. _**Adding a New Package**_
      * Click on the _New Upload_ button on upper right hand side of the page.

    B. _**Adding a New Version to an Existing Package**_
      * Select the package from your Uploads directory. Click on _New Version_.
3. **Reserve a DOI**
      * Under Basic Information -> Digital Object Identifier click the _Reserve DOI_ button.

4. **Upload**
   * Drag and drop your files into the window or choose files as directed.



Proceed to the Metadata section.

## Metadata

Please use the following guidelines when assigning metadata.

1. **Upload type**
   * Please assign _software_ to all github releases.  
2. **Basic Information**
   * Add the mandatory data.
   * Authors. WEBHOOK USERS: When generating a zenodo release using a webhook, the default is to assign all commiters as authors.  Default behaviors can be overridden using .zenodo.json file in the main directory. See PyLith and ASPECT for examples.
   * Description.  Please add an informative description of the software and changes to this release.  This is what the user will see.
   * Additional Notes. Add acknowledgements including funding here if your grant cannot be found in 5.
3. **License**
   * All CIG codes are _Open Access_
   * Please search for the correct _License_. Most CIG codes are _GNU General Pubic License 2.0_ or _GNU General Pubic License 3.0_. _or later_ is also supported.
4. **Communities**
   * Please assign the community "Computational Infrastructure for Geodynamics". You may need to type in most of the string before zenodo finds it.
5. **Funding**
   * Choose from pick list of funding agencies to add funding acknowledgements. NSF grants are now supported. If your grant is not listed, add it in *Additional Notes*. See 2.
6. **Related/alternate identifiers**
   * Add geodynamics.org/resources/*CodeName* as _references this upload_.
   * Add the github repo e.g. https://github.com/geodynamics/aspect/tree/v1.5.0 as _is a supplement to this upload_.
7. **Contributors**
   * Please don't forget to acknowledge others who contributed to this research product.
8. **References**
   * Add references you want users to cite here.
9. **Journal, Conference, Book/Report/Chapter, Thesis**
   * If this research product is part of one of the above, add the reference here.

## Save or Publish
When you are ready do not forget to **Publish** or just remember to **Save** your work.

* Save your work if you anticipate modifying the uploaded files.
* At any time, you can select an uploaded package and edit its metadata.
* Once Published, the DOI is minted and you CANNOT change the package's files without creating a new version.


Please feel free to add to these instructions.
