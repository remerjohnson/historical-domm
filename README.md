# DOMM Metadata Repository README

This is a repository to test how our normal [DOMM](https://github.com/orgs/ucsdlib/teams/domm) 'metadata wrangling' workflow would look like using git and GitHub.  

## Contents
+ `xls_standard_input_template.xlsx` - Our most recent template for our "Excel Standard Input stream". We use this template to populate the metadata for all the objects in a collection that are ingested into the DAMS.
+ `subject_import_template.xlsx` - Our most recent template to import subjects into the DAMS, which then create subject authorities if they don't match existing subjects, as well as point to external authorities from FAST, LoC, VIAF, Wikidata, etc.
+ Project folders (e.g. `mac-low`) - Folders for each project/collection, which contain the complete or in-progress metadata for that collection.
  + OLR - Contains the Object Level Record
  + CLR - Contains the Collection Level Record
  + provider_metadata - Contains the metadata (spreadsheets mostly) that we initially receive from data providers. Also can contain the results of our 'cleaning' the data via OpenRefine or other methods

## Workflow

A proposed general workflow for [DOMM](https://github.com/orgs/ucsdlib/teams/domm) is:  
+ If you are starting from scratch, fork this repo. If you already have it, `git pull` to get the latest version.
+ `cd` into the repo on your local machine, make your project's folder, then make subfolders for the CLR, OLR, provider data, a README, etc.
  + For help on formatting READMEs and other Markdown tips, see GitHub's page on [GitHub Flavored Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
+ Add the provider's original metadata, along with any 'cleaned' versions (via OpenRefine etc.) in `provider_metadata`.  
+ Commit frequently and provide commit messages outlining important highlights of what this current commit accomplished.
+ Make any and all pending commits, then submit a pull request to GitHub. Once the request is accpeted, your changes will now show up on GitHub.   
+ Open issues on GitHub for problems or concerns you want to tackle, or just long-term issues you need to solve about the repo itself.
+ If your present commit fixes an issue to the best of your knowledge, add the keywords `fixes #(issue number)` to the commit message and it automatically closes the issue.
+ If someone else outside of DOMM would like to download or edit the metadata, they would go through the same GitHub process of fork from GitHub -> make changes and commit -> submit pull request.

## Contributing

+ Open an issue or help on the Wiki :smile:
