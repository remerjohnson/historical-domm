# Intro

This is a repository to test how our normal workflow would look like in git and GitHub (or some other hosted/networked git repository).  

A proposed general workflow is:  
+ `git init` in the local directory you wish to have Git manage. You can do this first or at any point after adding files/directories.
+ Master branch is where all the edits happen: so add the Excel template, rename it, edit it some, etc.  
+ Add the original metadata, along with any 'cleaned' versions (via OpenRefine etc.) in its own folder that we most likely don't touch.  
+ Commit frequently and provide commit messages outlining important highlights of what this current commit did.
+ Set up the remote to GitHub, make any pending commits, then `git push` to push to GitHub or networked space.    
+ If someone else in DOMM would like to download or edit the metadata, they would go through the normal GitHub process of `git clone` or fork from GitHub -> make changes and commit -> submit pull request.
+ Even after the files are deleted on staging, the metadata repository could remain updated and preserved. It still might not be complete if RDF edits have occurred on the collection.

## Future Uses

If this were the normal workflow, this README could contain helpful notes about the metadata or data for this specific collection that the Metadata Analyst wants to keep tracj of. 
