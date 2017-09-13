---
layout: post
title: Using Git and GitHub
thumbnail: git.png
tile-name: Using Git and GitHub
date: 2017-09-05

author: OctoCat
tags: [gitHub]
---

GitHub is a really useful tool for software development, particularly when collaborating with lots of folks, and a great thing to learn to use.
> GitHub is a web-based hosting service for software development projects that use the Git version control system. GitHub offers free accounts for open source projects. As of May 2011, GitHub was the most popular open source code repository site. The site provides social networking functionality such as feeds, followers and the network graph to display how developers work on their versions of a repository. [[Wikipedia](http://en.wikipedia.org/wiki/GitHub)]

Below are some recommended resources for getting to know source-code control with Git and GitHub. The quickest way to get started is with the Desktop tools that GitHub has created, but if you want to use the command line, which gives you more power and control, by all means!

### Starting points
- Read up a little on what [version control is](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)
- Setup an GitHub account at [education.github.com](https://education.github.com) and get the educational discount!
- Either install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) or download the [desktop App](https://desktop.github.com). __Note:__ If you install the desktop app for Mac it's then [rediculously easy to install the Git command line tools](https://github.com/blog/1510-installing-git-from-github-for-mac)
- Learn about GitHub using their [fantastic guides](https://guides.github.com). Below are the ones you need to pay attention to: 
  - [Understanding the GitHub Flow](https://guides.github.com/introduction/flow/)
  - [Hello World ](https://guides.github.com/activities/hello-world/) - or learning the basics of git and github 
  - [Forking Projects](https://guides.github.com/activities/forking/)
  - [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)
  
### Major Things
This is guide has all of the basics you need to know: [Collaborating on projects using issues and pull requests](https://help.github.com/categories/collaborating-on-projects-using-issues-and-pull-requests/)
1. __[Fork the Repo](https://help.github.com/articles/working-with-forks/).__ Fork in Git speak means to take a working copy of the original repository. This lets you work on your copy while other things happen in the main repository. This avoids conflicts but allows you to contribute to the repository over time. Find out more [here](https://help.github.com/articles/working-with-forks/)
  
2. __[Work in Branches](https://git-scm.com/book/no-nb/v1/Git-Branching-What-a-Branch-Is).__ Branches are another way to isolate your work from other aspects of the repository. Normally for each new feature or element that you're working on, it's useful to create a branch. For example, if you were making changes to your project's code at the same time as writing your tutorial assigment, it would be really helpful to have two branches in your repo, one for each. Keeping things clear. Find out more [here](https://help.github.com/desktop/guides/contributing/making-changes-in-a-branch/)
 
3. __[Commiting and Syncing Changes](https://help.github.com/desktop/guides/contributing/committing-and-reviewing-changes-to-your-project/).__ As you make changes to your files, git will track them and keep note of them. At some point when you've either finished some aspect of your work, hit a milestone or just want to record progress at a point, you'll _commit_ your changes. You do this by adding a descriptive label (of what the changes are about) and pushing the 'Commit' button. This adds the changes in your files and examines the differences from the last time you committed changes. Once committed, you then 'Sync' your local copy to the main online repository and they're saved! Then, at any point, you can find, search, view and rollback to this version of the files.

4. __[Pull Requests](https://yangsu.github.io/pull-request-tutorial/).__ Pull requests let you tell others about changes you've pushed to a GitHub repository. Once a pull request is sent, interested parties can review the set of changes, discuss potential modifications, and even push follow-up commits if necessary. Read more [here](https://help.github.com/articles/proposing-changes-to-a-project-with-pull-requests/) and [here](https://www.atlassian.com/git/tutorials/making-a-pull-request/)
