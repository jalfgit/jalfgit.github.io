# jalfgit.github.io Readme Page
website: https://jalfgit.github.io/
Most Used Commands


# creating a page generator
1. break down index.html into parts
2. three files are needed: header.html, footer.html
3. text_object: to hold the body of the page


## Git Helpful commands

### Global Setup
Global Setup in Git in case you have not initiated Git
```HTML
git config --global user.name "Your Name Here"
git config --global user.email "emailaddress@email.com"
```


### Creating Repo
Instructions when creating your repo locally
```HTML
git clone https://miami.bootcampcontent.com/GITUSERNAME/PROJECTNAME.GIT
cd projectname
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master
```

If you already have a folder you would like to initialize with GIT
```HTML
git init
git remote add origin https://miami.bootcampcontent.com/GITUSERNAME/my-first-project.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

Existing Repo and renaming it
```HTML
cd existing_repo
git remote rename origin old-origin
git remote add origin https://miami.bootcampcontent.com/GITUSERNAME/my-first-project.git
git push -u origin --all
git push -u origin --tags
```

Getting the status of the downloaded branch
```HTML
git status
```

Download latest copy of the master branch
```HTML
git pull origin master
git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done
git pull --all     #this will update all brancges.
```

### Working With Branches
Instructions to list branches
```bash
git branch
git branch -a
```

Create Branches
```bash
git branch BRANCHNAME
```
Delete Branches
```bash
git branch -d BRANCHNAME
```

Selecting Branches
```bash
git checkout BRANCHNAME
```

### Reset Repo to Remote Branch
Instructions when reset your local copy of the repo. The following will reset your local repo and match the server contents. 
> make sure you will not need the current work
```HTML
git fetch --all
git reset --hard origin/master
```

### Git Branch Configuration *config* file
The config is under '''HTML <code>repodir/.git/config/</code>

### Stashing modified code to THEN download master branch code
Instructions to list branches
```HTML
git stash           //this saves a copy of the code
git pull            //pull the code without erasing what you modified.
git stash pop       //this recovers the modified code
```
## Marking code sections

The prettyprinter looks for `<pre>`, `<code>`, or `<xmp>` elements with the
*prettyprint* class, and adds `<span>`s to colorize keywords, strings,
comments, and other token types.

```HTML
<pre class="prettyprint">
source code here
</pre>
```

## Python Helpful Section
Section to store code for python
```python
import PACKAGENAME
print("Hello Class")
```


## Contributions
This file has been created by Jorge Alfonso for the convenience of the class, and it is not intended to 
replace any content provided by the school, affiliates, and educational sponsors.
:octocat
