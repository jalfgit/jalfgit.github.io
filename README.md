# jalfgit.github.io Readme Page
Most Used Commands

# Git Helpful commands

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
git remote add origin https://miami.bootcampcontent.com/jalfgit/my-first-project.git
git add .
git commit -m "Initial commit"
git push -u origin master
```

Existing Repo and renaming it
```HTML
cd existing_repo
git remote rename origin old-origin
git remote add origin https://miami.bootcampcontent.com/jalfgit/my-first-project.git
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
```

### Reset Repo to Remote Branch
Instructions when reset your local copy of the repo. The following will reset your local repo and match the server contents. 
```HTML
git fetch --all
git reset --hard origin/master
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

