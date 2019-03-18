# Kaggle global terorrism analysis
Subject realized as (data exploration) course during studies.

The aim of those project classes is to mine data and do some processing on it, then visualize results.

## Prepare environment

Scrpits wrote on Linux Ubuntu 18.04LTS with Python3.6.7.

Update system
```bash
sudo apt-get update
sudo apt-get upgrade
```

Prepare Python 3.6 env
```bash
sudo apt-get install python3.6
sudo pip3 install virtualenv

(it's my favorite way to manage python's virtualenvs, it's not obligatory or something, one more popular way is to storage env in project)
mkdir ~/venvs
cd ~/venvs/

virtualenv kgta -p $(which python3)
```

Clone repo with https

```bash
cd directory
git clone https://github.com/paniks/kaggle-global-terrorism-analysis.git
```

Activate virtualenv and install requirements
```bash
(in project dir)

source path/to/venv/bin/activate
pip install -r requiments.txt
```

The run jupyter notebook, see my solution and just enjoy it!
```bash
(in project dir)

jupyter notebook
```

## Informations from lectuer 

### Instructions:
1. Download data set, Global Terrorism Database, from https://www.kaggle.com/START-UMD/gtd
2. Take a quick look at the data set. Check what's inside, how the data is structured, and where the data is corrupted (missing values, bad structure, etc).
3. Think and create 5 questions to the data. Try to ask yourself what's really interesting in the data set. What's not so obvious. E.g. some trends, patterns, correlations.
4. Create a jupyter notebook and use python, numpy, pandas, matplotlib (at least) to provide all the answers to your questions.
5. Create a new github repository, and put your jupyter notebook there.
6. Create readme.md file as well in your github root directory with all necessary instructions (what is in the repo, what libs are necessary to run the code, where to find data set and where to save it  - this is necessary because the dataset is too big for github repo).
7. Provide the necessary documentation and introduction in your notebook using markdown language, at least: data source description, data structure, importing process, data processing process.
8. Put some data visualization in your notebook. Sometimes it's much easier to present the answer using a chart rather than numbers
9. Check if your notebook run smoothly - use 'Reset & Run All' command from the menu. Save it.
10. Export the notebook as HTML as well, and save the file in the repo.
11. Do not forget to commit/push all the changes to your repo on hithub.
12. Smile :) You did a good job!
    

### FAQ:
1. Can I take a look at different solution provided at kaggle?  Yes, you can. But check more than one solution. Try to understand what the authors are trying to solve, and how could it be used in your project. Try to find really good examples - easy to understand and not so complicated. Remember - you create the notebook as an instruction to someone else! Try to not complicate the process.
2. Can I take a look at my friend's solution, that he/she has just put on github? Yes, you can. But it's the smart way of solving the project. I'm sure that you want to be smarter in the next semester - so try to create a better solution and your own one :)
3. Jupyter notebook provide R kernel, so can I use R instead? Nope, R sucks. Even if you love R, try to solve the project using Python.\n


## Troubleshooting 

You may face troubles with basemap toolkit for matplotlib, so I recommend to firstly install libgeos lib and basemap repo strict from git.
```bash
sudo apt-get install libgeos-dev	#its global install for your machine 
pip install https://github.com/matplotlib/basemap/archive/master.zip	#run with activated virtualenv
```	
