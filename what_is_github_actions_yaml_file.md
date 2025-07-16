---
layout: default
title: git actions and pypi
---
this is what i learned as beginner  , documenting it for later,so i dont have to relearn

### github actions
github actions are used for automation. it is a event handler and it contains virtual machines ( called runner),
when github events occur like pushing code then github will run repos workflow files,these files are in  (.github/workflows/*.yml).  
this files are called workflow files. it contains defnitions and instructions.github will read defnitions and runs instructions  using its own virtual machine,   
mac os, windows , and linux is avilable and we can define it in this file.  
if there is run commands in this files then it willbe executed.

### pypi publishing and github actions 
we can add workflow files to gituhub .so we can create commands to upload our project to pypi.   
now when github event occurs then our code canbe automattically published to pypi
* [guide to publish project to pypi from github using github actions](https://hackernoon.com/automate-python-package-publishing-with-github-actions)
  
![pyp_and_github_actions drawio](https://github.com/user-attachments/assets/62c61f7d-44c4-44d7-990b-7af83d21c011)

**flow of github actions for automattically publishing to pypi**
1. we write workflow file and commit into a githubs folder like (.github/workflows/helo.yml)
2. we write our python package that contain pypi compatible structre 
3. we push code to github
4. if there is any files in this folder (.github/workflows/*.yaml) then github internaly reads this files and executes its instructions
5. now code willbe automattcialy uploaded to pypyi from github

### the adwantage is. 
we dont have to upload  two times to github and pypi.  
when we upload code to github it will automattically published to pypi.  



