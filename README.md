# This is the first End to End Class
# Steps:
1) Initialize the git
```
git init
```
2) Add the code
```
git add .
```
3) Commit the changes
```
git commit -m "This is the first commit"
```
4) Create the repo in GitHub directly in VS Code 
> Source Control -> Publish Branch -> Select Public or Private repo
5) Create a branch or rename the branch to main (the branch creates will be master)
* Rename the master branch to main branch
```
git branch -M main
```
* Create a new branch
```
git checkout -b pre_dev
```
* Check the branch
```
git branch
```
* Navigate to certain branch
```
git checkout <branch name>
```
6) If others do changes in repo like add or remove file, we need to pull the changes
```
git pull
```
7) Create a init_setup.sh file with commands to automate the environment creation and install requirements in linux. This file works in linux so terminal should be Git Bash. To run this file:
```
bash init_setup.sh
```
8) If step 7 doesnot work we can manually create the environment inside the folder which you are working and activate it
* To create the environment using conda:
conda create -p venv python==3.8 -y
* To activate the environment:
conda activate venv/
9) Create a template file to automate the creation of all the folders and files required for the project. This template file is called as boiler file.
10) Create the requirements.txt file and specify all the packages which are to be installed.
11) Write a setup.py to create a own package. To create package run the command
```
python setup.py install
```
12) But the prefered way to install this package is to write ```-e .``` in the requirements.txt file. Pip install the requirements.txt file. ```-e .``` will read the setup.py file.
12) We can check list of packages using
```
pip list
```