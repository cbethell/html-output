# OpenPBTA-analysis 
## Filing a PR checklist

- [ ] [Fork](https://help.github.com/en/articles/fork-a-repo) the repo. You only need to do this step once, continue to the third step of this list if you have already done this. 
- [ ] Make the original repo, `AlexsLemonade/OpenPBTA-analysis`, an [upstream repository](https://help.github.com/en/articles/configuring-a-remote-for-a-fork).
- [ ] Checkout a [new branch](https://gist.github.com/markSci5/5916003) to make changes on. **WAIT** Is your master branch up to date with the upstream repo?  
Try `git status` to check. If it's not, go [here](https://help.github.com/en/articles/syncing-a-fork) before creating your new branch. Remember to `git push` when you are done. 
- [ ] Did you make numerous changes, too many for one pull request? Then let's create [stacked pull requests](https://github.com/AlexsLemonade/OpenPBTA-analysis/blob/master/CONTRIBUTING.md#creating-stacked-pull-requests). 
- [ ] Now that you have committed changes, be sure to write a detailed summary of the changes by following this [template](https://github.com/AlexsLemonade/OpenPBTA-analysis/blob/master/.github/PULL_REQUEST_TEMPLATE.md).     

Now check to make sure you have done the following before filing the PR: 

- [ ] Run a linter (using [styler](http://styler.r-lib.org/) for example)
- [ ] Set the seed (if applicable)
- [ ] Structure of analysis directory meets the [Project Structure](https://github.com/AlexsLemonade/OpenPBTA-analysis#folder-structure) guidelines
- [ ] Comments and/or documentation up to date
- [ ] Double checked paths
- [ ] Spell check any Rmd file or md file (using [mdspell](https://github.com/mtuchowski/mdspell) for example)
- [ ] Restart R and run all notebooks fresh and save (be sure to [run in the Docker container](https://github.com/AlexsLemonade/OpenPBTA-analysis#development-in-the-project-docker-container)) 
- [ ] Connect the pertinent issues on ZenHub
- [ ] Updated Dockerfile and built Docker image successfully
- [ ] Added analysis to [continuous integration](https://github.com/AlexsLemonade/OpenPBTA-analysis#adding-analyses-to-ci)


#### If you have completed all of the applicable steps above, you can request a suitable reviewer and file the PR/draft PR. 

#### Note: Upon approval of all Pull Requests for an analysis, [create a final Pull Request for a shell script](https://github.com/AlexsLemonade/OpenPBTA-analysis#adding-analyses-with-multiple-steps) that runs the entirety of scripts in your analysis directory.