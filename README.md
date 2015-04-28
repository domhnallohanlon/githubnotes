## Working with Git.

First, it's probably important to differentiate between Git, the language, and GitHub the platform. Git is a piece of software for managing different versions of code that you have written. Github is an online-platform where you can store your source code, and keep track of any changes that you have made to it. Being online means that it is accessible from anywhere in the world with an internet connection. 

## Creating a Repository

A repository, or repo, is simply another name for an archive or collection of code that you have written. Typically, for each project that you undertake you will want to create a new repo.

To create (initialise) a new local repo run the command:

```
git init
```

## Sync changes

Once you have a local respoitory, you will need to add a remote repo so that you can push your changes to it. You can accomplish this with the following command:

```
git remote add origin https://github.com/username/reponame.git
```

## Status update:

To check the status of your project run: 

```
git status
```

## Creating a README file

All repos should have a plain-text readme file. Github povides good support for Markdown, and this document is an example of a markdown document.

To create a file from the terminal use the `touch` command, i.e.:

```
touch README.md
```

You can then use an editor such as nano to edit the contents of the file:

```
nano README.md
```

## Staging

If you want to monitor specific filed for changes to need to specifically `add` them:

```
 git add README.md
```

To stage all files use `git add .` or `git add -A`.

## Committing

To commit changes use the following command. The `-m`flag specifies a commit message.

```
 git commit -m "added README file"
```

## Push Your Changes to GitHub

If you use the following command:

```
  git push -u origin master
```

Git will set the upstream branch to `origin master` so any subsequent pushes can be made the following:

```
 git push
```

## Try it yourself:

Add a few more files, stage, commit and push them to get used to this new workflow. 
