# MineParis-ES-course
Course material for ES maching learning course

## Installation

* Virtual environment: if you don't have it to create virtual environment, check this site for installation
[Miniconda](https://docs.conda.io/projects/miniconda/en/latest/)

```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

* clone this repo, and we will call the directoy that you cloned as ${DL_course}
* Install dependencies, We use python 3.13 and pytorch >=2.9.0
```
conda create -n DL_course_env python=3.13
conda activate DL_course_env
conda install pytorch torchvision cudatoolkit=10.2 -c pytorch
cd ${DL_course}
pip install -r requirements.txt
```

* Add your environment to jupyter notebook
```
conda install -c conda-forge ipykernel
python -m ipykernel install --user --name=DL_course_env
```