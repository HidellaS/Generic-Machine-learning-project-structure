# This is an End to End Generic Machine learning project. we can use this structure for any machine learning project in the future. we only have to change the dataset and the algorithm. all the other steps are similar.

# here in the bottom we have the complete step by step

#### 1- first create a repository in the github (and take a token for authentication if you don't have one already)

#### 2- create a folder in your PC for the project

#### 3- Use anaconda prompt to go to that specific folder

#### 4- after that use " code . " to open the vs code in side the folder

#### 5- now open a terminal inside the vs code using the terminal tab in the top toolbar (can use cmd or powershell)

#### 6- then create a python environment inside this folder using this command  " conda create -p [env name] python==[version u want] -y "   (in here we use -y at the end because then we don't have to manually put yes when creating the environment)

#### 7- then activate the environment using this command " conda activate [env name]/ "  (always remember to put / at the end)

#### 8- now initialize a git repo using " git init " using the terminal

#### 8- now do the normal step by step process to commit and push the files to github.

#### 8- Now go to git hub and create a .gitignore file and give the language as python and commit (use add file tab to put a new file)

#### 8- then in our vs code terminal type " git pull " to get the fils to our local pc

#### 9- now if your virtual env name is not a typical name like env or venv etc.. then go inside the gitignore file and find the #Environments location and put your Environments name to the list.