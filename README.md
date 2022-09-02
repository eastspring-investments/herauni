# Hera Uni

Open-source learning materials catered for Data Engineers, Data Scientists, AI Engineers, AI Scientists, and Quants from Eastspring Investments Group.

To quickly get started, all you need is a Google account and you can just press on the `Open in Colab` button that allows you to run the notebook without setting up the environment locally or ensuring that you are on the latest branch.

## Topics
- [Eigenvector Centrality, Page Rank with Eigendecomposition, Page Rank with Power Iteration, and Google Page Rank](https://github.com/eastspring-investments/herauni/blob/main/notebooks/page_rank.ipynb) 
  - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eastspring-investments/herauni/blob/main/notebooks/page_rank.ipynb)
- [Linear Programming (Optimisation)](https://github.com/eastspring-investments/herauni/blob/main/notebooks/linear_programming.ipynb)
  - [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eastspring-investments/herauni/blob/main/notebooks/linear_programming.ipynb)

## (Optional) Getting Started: First Time

### Step 1: Install Miniconda

Head to [Miniconda website](https://docs.conda.io/en/latest/miniconda.html). Download and install the relevant installers. There are installers available for Linux, macOS, and Windows.

### Step 2: Clone Repository

Proceed to clone the repository so you can have the repository available locally.

```
git clone https://github.com/eastspring-investments/herauni
```

### Step 3: Create Environment

```
conda env create -f environment.yml
```

## (Optional) Getting Started: Subsequent Time

### Activate Environment and Run Jupyter

You need to run 2 separate commands to activate the environment and run Jupyter lab.

```
conda activate herauni
jupyer lab
```

### Tip on Avoiding Branch Conflicts

Our suggestion is to just copy the notebook with a separate name so that there will never be clashes when you make changes and add your notes.

For example the original notebook is `page_rank.ipynb`, make a copy `page_rank_custom.ipynb` where you run and make notes without touching the original notebook `page_rank.ipynb`.

### Getting Latest updates

If you want to pull latest updates, you can run the following command which stashes your local work (puts in aside) and pulls the latest commit.

```
git stash
git pull
git stash pop
```

This essentially results in the following logic:

```
Remote: A--B--C

Local before: A--B--(uncommitted changes)
Local after: A--B--C--(uncommitted changes)
```

There may be conflict locally, particularly if you ran the notebooks and added your own notes, and you have to resolve accordingly. This is more advanced and you can search for this online and can be painful as you have to make a decision with every conflict. Please refer to the tip avoid on avoiding branch conflicts for avoiding this.

## Contributors
- Ritchie Ng, Head of Data & AI, Eastspring Investments Group

## License
MIT
