# Generic Machine Learning Project Template.

## This repository provides a generic template for creating end-to-end machine learning projects. By following this structure, you can reuse the same workflow for future projects by simply swapping datasets and algorithms. The other steps remain consistent.

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

#### 10- create 2 new files in the project folder named setup.py and requirements.txt

#### 11- setup.py is responsible in creating our machine learning project as a package and we can even install or use this package . we can deploy in pypi too

#### 12- requirements.txt for our packages

#### 13- once we created setup.py , how it going to find out how many packages are there and stuff. so for that we going to create another folder in the project called " src "

#### 14- now inside that src folder we going to create another file called " __init__.py "   we use this so that we can find the src as a package

#### 15 the __init__.py file marks the folder as a Python package, allowing imports to work correctly.

#### 16- now whenever the setup.py run the  find_package() , it will just go and see in how many folders does it have this __init__.py  . so it wil directly concider this src as a package and it will build it . now we can import it anywhere like we importing pandas , numpy etc. but for that we need to put into pypy package

#### 17- our entire project development will happen inside this src folder

#### 18- after coding the setup.py for requirements then we go to terminal and run 'pip install -r requirements.txt'  this will install all the pacakges and will create info files, dependencies etc.

#### 19- create another folder called components in the src folder and put '__init__.py' file inside it

#### 20- now create these files in it called data_ingestion.py and data_transformation.py and model_trainer.py . all these files in the components are mainly for training the model

#### 21- create another folder called pipeline inside the src and create the '__init__.py' in it

#### 22- create a file called 'train_pipeline.py' and 'predict_pipeline.py' inside the pipeline folder. this file will trigger all the components in the previous folder

#### 23- create these files inside the src folder named 'logger.py' , 'exception.py' , 'utils.py'   (we can use utils.py for  read data from database, or save model in cloud etc.)

#### 24- code all the logging, exception and utils files according to the project

#### 25- after completing the 'data_ingestion.py' code . we should add .artifact to the gitignore file. because we don't need it to go to github