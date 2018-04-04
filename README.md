# DOMM Metadata Repository README (Deprecated)

This is a now-defunct repository that tested how our 'metadata wrangling' workflow would look like using git and GitHub. It has been superceded by a new, private repo.  

## Workflow

A proposed general workflow is:  
+ If you are starting from scratch, fork this repo. If you already have it, `git pull` to get the latest version.
+ `cd` into the repo on your local machine, make your project's folder, then make subfolders for the CLR, OLR, provider data, a README, etc.
  + For help on formatting READMEs and other Markdown tips, see GitHub's page on [GitHub Flavored Markdown](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
+ Add the provider's original metadata, along with any 'cleaned' versions (via OpenRefine etc.) in `provider_metadata`.  
+ Commit frequently and provide commit messages outlining important highlights of what this current commit accomplished.
+ Make any and all pending commits, then submit a pull request to GitHub. Once the request is accpeted, your changes will now show up on GitHub.   
+ Open issues on GitHub for problems or concerns you want to tackle, or just long-term issues you need to solve about the repo itself.
+ If your present commit fixes an issue to the best of your knowledge, add the keywords `fixes #(issue number)` to the commit message and it automatically closes the issue.
+ If someone else outside of DOMM would like to download or edit the metadata, they would go through the same GitHub process of fork from GitHub -> make changes and commit -> submit pull request.

