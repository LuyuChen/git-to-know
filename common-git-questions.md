1. How to abort git commit --amend?
 Saving the file with no contents will abort the amend.

2. How to move the content of repo1 to repo2 while preserving history?
`cd repo2
git checkout master
git remote add r1remote **url-of-repo1**
git fetch r1remote
git merge r1remote/master --allow-unrelated-histories
git remote rm r1remote`
[Stackoverflow link](https://stackoverflow.com/questions/17371150/moving-git-repository-content-to-another-repository-preserving-history)

