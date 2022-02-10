
# Book Crossing Recommender System

This project is developed in Python + Scikit-learn + Scikit-surprise for building a recommender system for [book crossing](http://www2.informatik.uni-freiburg.de/~cziegler/BX/) dataset. 

In this project, these recommender systems are implemented:
- User-based collaborative filtering
- Item-based collaborative filtering -> Weighted Slope One
- Content-based filtering
- Machine Learning based filtering -> Baseline
  

## Environment

- Python: 3.9.0
- Numpy: 1.22.1
- Pandas: 1.3.5
- Matplotlib: 3.5.1
- Plotly: 5.5.0
- Scikit-learn: 1.0.2
- Scikit-surprise: 1.1.1

  
## Setup Guide

Clone the repository:

```
git clone https://github.com/mohsenMahmoodzadeh/Book-Crossing-Recommender-System.git
```

Create a virtual environement (to avoid conflicts):

```
virtualenv -p python3.9 recsys

# this may vary depending on your shell
. recsys/bin/activate
```

Install the dependencies:

```
pip install -r requirements.txt
```

If you want to work on jupyter notebook, you may need to setup a kernel on your virtual environment to make sure all your modules execute correctly.
```
python -m ipykernel install --name recsyskernel

# Now you get a kernel named `recsyskernel` in your jupyter notebook
```  

## Usage Guide

First of all, run the cells of [Data_Preprocessing.ipynb](https://github.com/mohsenMahmoodzadeh/Book-Crossing-Recommender-System/blob/master/Data_Preprocessing.ipynb) to generate preprocessed data files. Then you can use [Recommendation.ipynb](https://github.com/mohsenMahmoodzadeh/Book-Crossing-Recommender-System/blob/master/Recommendation.ipynb) to make recommendations and test recommenders.


## Future Works

- Improve content-based recommender system so that it takes multiple fields(not just `bookTitle`) for TF-IDF representation.

- Build a hybrid recommender system which combines collaborative and content-based filtering recommender systems.
  
- Build a neural recommender system(something like [this](https://blog.tensorflow.org/2020/09/introducing-tensorflow-recommenders.html)).

- Modify the models so that be evaluable with evaluation metrics(maybe [this](https://github.com/statisticianinstilettos/recmetrics) can help).

## Contributing

Fixes and improvements are more than welcome, so raise an issue or send a PR!
