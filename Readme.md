# Code
## A
git init
git remote add origin https://github.com/kangwuing/Hanyang.git
git status
git add .
git commit -m "Initial commit"
git pull --rebase origin main
git add <file_name>
git rebase --continue
git push origin main

## B
git clone https://github.com/kangwuing/Hanyang.git
git pull origin main

# Data DVC

pip install dvc

## A
dvc init
dvc add data/
git add data.dvc .gitignore
git commit -m "Add data to DVC"

dvc add data/
git add data.dvc .gitignore
git commit -m "Add data to DVC"

## B
dvc pull

# Conda(env)
## A
conda env export > environment.yml

git add environment.yml
git commit -m "Add environment.yml"
git push origin main

## B
conda env create -f environment.yml
conda activate <environment_name>
