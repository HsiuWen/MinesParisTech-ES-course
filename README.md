# MineParis-ES-course
Course material for ES maching learning course

## Installation
 * If your operation system is windows, read this link to activate [wsl](https://learn.microsoft.com/en-us/windows/wsl/install) and Linux distribution (I use Ubuntu) from Microsoft Store. If everything is correct, normally you can use terminal and key ```wsl``` to enter Ubuntu terminal. 

* Create virtual environmentL check this site for installation
[Miniconda](https://docs.conda.io/projects/miniconda/en/latest/), or simply run the following code

```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

* clone this repo, and we will call the directoy that you cloned as ${DL_course}
* Install dependencies, We use python 3.12 to make sure we have less troubles with opencv

```
conda create -n ML_course_env python=3.12
conda activate ML_course_env
cd ${DL_course}
pip install -r requirements.txt
```

* Add your environment to jupyter notebook
```
conda install -c conda-forge ipykernel
python -m ipykernel install --user --name=DL_course_env
```