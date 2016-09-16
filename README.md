# DOMM Metadata Repository README

This is a repository to test how our normal DOMM metadata wrangling workflow would look like in git and GitHub.  

A proposed general workflow is:  
+ If you are starting from scratch, `git clone` this repo. If you already have it, `git pull` to get the latest version.
+ `cd` into the repo on your local machine, make your project's directory, then make subfolders for the CLR, OLR, provider data, a README, etc.
+ Add the prodicer's original metadata, along with any 'cleaned' versions (via OpenRefine etc.) in its own folder (my example is `provider_metadata`).  
+ Commit frequently and provide commit messages outlining important highlights of what this current commit did.
+ Make any and all pending commits, then `git push` to push to GitHub. (If we have someone managing the repo, it would be a pull request instead)    
+ Open issues on GitHub for problems you want to tackle or just long-term issues you need to solve about the repo in general.
+ If your present commit fixes an issue to the best of your knowledge, add the keywords `fixes #(issue number)` without quotes and it automatically closes the issue.
+ If someone else outside of DOMM would like to download or edit the metadata, they would go through the normal GitHub process of `git clone` or fork from GitHub -> make changes and commit -> submit pull request.
+ Even after the files are deleted on staging, the metadata repository could remain updated and preserved. It still might not be "complete" if RDF edits have occurred on the live collection.
