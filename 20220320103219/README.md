# Git Commands for opensource contribution

### Do them once for each GH project

* **fork** repo to get it my_gh/repo
*
```
git clone my_gh/repo
```
* cd repo
* 
```
git remote add upstream native_repo
```

### Do them for each contribution to the project

* 
```
git pull upstream default_branch
```
* 
```
git switch -c my_branch
```
* git add, git commit ...
*
```
git push origin my_branch
```
* now just go to my_gh/repo and create a **PULL REQUEST**
* delete branch
* git checkout default_branch -> git branch -D my_branch -> git pull
upstream default_branch

