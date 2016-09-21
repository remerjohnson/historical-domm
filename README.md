# DOMM Metadata Repository README

This is a repository to test how our normal DOMM 'metadata wrangling' workflow would look like using git and GitHub.  

## Contents
+ xls_standard_input_template.xlsx - Our most recent template for our "Excel Standard Input stream". We use this template to populate the metadata for all the objects in a collection that are ingested into the DAMS.
+ Project folders (e.g. `mac-low`) - Folders for each project/collection, which contain the complete or in-progress metadata for that collection.
  + OLR - Contains the Object Level Record
  + CLR - Contains the Collection Level Record
  + provider_metadata - Contains the metadata that we initially receive from data providers. Also can contain the results of our 'cleaning' the data via OpenRefine or other methods

## Workflow

A proposed general workflow for DOMM is:  
+ If you are starting from scratch, `git clone` this repo. If you already have it, `git pull` to get the latest version.
+ `cd` into the repo on your local machine, make your project's directory, then make subfolders for the CLR, OLR, provider data, a README, etc.
  + For help on formatting READMEs and other Markdown tips, see GitHub's page on [GitHub Flavored Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
+ Add the provider's original metadata, along with any 'cleaned' versions (via OpenRefine etc.) in its own folder (my example is `provider_metadata`).  
+ Commit frequently and provide commit messages outlining important highlights of what this current commit did.
+ Make any and all pending commits, then `git push` to push to GitHub. (If we have someone managing the repo, it would be a pull request instead)    
+ Open issues on GitHub for problems you want to tackle or just long-term issues you need to solve about the repo in general.
+ If your present commit fixes an issue to the best of your knowledge, add the keywords `fixes #(issue number)` to the commit message and it automatically closes the issue.
+ If someone else outside of DOMM would like to download or edit the metadata, they would go through the normal GitHub process of `git clone` or fork from GitHub -> make changes and commit -> submit pull request.
+ Even after the files are deleted on staging, the metadata repository could remain updated and preserved. It still might not be "complete" if RDF edits have occurred on the live collection in production, however.
