---
layout: post
title: "Heroku and Github, Project Integration"
description: ""
comments: false
keywords: "heroku, github, git, integration"
---

### Heroku and Github, Project Integration Log


	step 01: login to heroku and initialize a project
	
			heroku login
			heroku create YOUR-APP-NAME
			git clone https://git.heroku.com/YOUR-APP-NAME
			cd YOUR-APP-NAME
	
	step 02: Change the remote repo from heroku to github and push
             * make a github repo before proceeding			
			
			git remote -v
			git remote set-url origin YOUR-GIT-REPOSITORY.git
			git remote -v
			git pull
			git add .
			git commit -sm 'first commit to github'
			git push
			
	step 03: connect heroku's depoyment service to github
	
			shoulb be done on heroku's website
			
> This content was written based on the tutorial section of http://yoogomja.tistory.com