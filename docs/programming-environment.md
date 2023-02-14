# Anaconda environments

## Create environment: ds


We install some modules in a new Anaconda environment. We call this new environment `ds` (data science). 

> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 

> On *macOS*: Open a terminal ([learn how to open a terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac)) 


- Copy this code and run it in your terminal: 


```bash
conda create -n ds python=3.9 pandas openpyxl jupyter scikit-learn altair vega_datasets matplotlib seaborn requests tweepy beautifulsoup4 streamlit sqlalchemy psycopg2 xgboost
```

<!--
```bash
conda create -n dsws22 python=3.9 pandas openpyxl ipython scikit-learn altair matplotlib seaborn requests tweepy beautifulsoup4 sqlalchemy psycopg2
```
-->


Activate the new environment:

```bash
conda activate ds
```

---

## Create environment: tf

We install some modules in a new Anaconda environment. We call this new environment `tf` (TensorFlow). 

> On *Windows* open the Start menu and open the "Anaconda Command Prompt". 

> On *macOS*: Open a terminal ([learn how to open a terminal](https://support.apple.com/guide/terminal/open-or-quit-terminal-apd5265185d-f365-44cb-8b09-71a064a42125/mac)) 


- Copy this code and run it in your terminal: 


```bash
conda create -n tf python=3.10 pandas jupyter tensorflow altair pydot --y
```

Activate the new environment:

```bash
conda activate tf
```

### Install Graphviz

Graphviz is open source graph visualization software. We use it to visualize Deep Learning Architectures.

#### Windows

- Install [Graphiz](https://graphviz.gitlab.io/download/#windows)

#### Mac

- Install [MacPorts](https://www.macports.org/install.php). The MacPorts Project is an open-source community initiative to design an easy-to-use system for compiling, installing, and upgrading either command-line, X11 or Aqua based open-source software on the Mac operating system. 


- Install Graphviz using MacPorts. In your temrinal: 

```bash
sudo port install graphviz
```

---

## How to select your environment

In Visual Studio Code:

1. [Create or open a Jupyter Notebook](https://code.visualstudio.com/docs/datascience/jupyter-notebooks#_create-or-open-a-jupyter-notebook)

1. Next, select a kernel using the kernel picker in the top right (select the Anaconda environment)

![](https://code.visualstudio.com/assets/docs/datascience/jupyter/native-kernel-picker.png)


If you can't see your newly created environment:

You can also manually specify an interpreter if Visual Studio Code doesn't locate your kernel automatically.

1. Show command palette: Press `cmd+shift+p` (Mac) or `strl+shift+p` (Windows)

1. Search for `Python: Select Interpreter´

1. Select it and you should see a list of your virtual environments

1. Select the environment of your choice and you are ready to go.



If the steps described above should not work for you, take a look at other tips at [StackOverflow](https://stackoverflow.com/questions/43351596/activating-anaconda-environment-in-vscode).