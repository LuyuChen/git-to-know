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

3. How to solve issues with line endings preventing checking, merging, etc?
`git rm -r . --cached -q && git reset --hard`, but be sure you have not changes that you want to keep!
https://github.com/wrye-bash/wrye-bash/wiki/%5Bgit%5D-Issues-with-line-endings-preventing-checking,-merge,-etc

