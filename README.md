# Mathematical Cartography 2023
These Jupyter notebooks support the <b> Mathematical Cartography LOOM.02.007 </b> MSc course and focus on the capabilities of the Python mathematical cartography and visualization library [Cartopy](https://scitools.org.uk/cartopy/docs/latest/).

The first tutorial gives an overview of creating a map window, using projections and constructing basic map elements (grid, text)
* https://github.com/holgervirro/mcarto2023/blob/master/Kaardiakna_juhtimine.ipynb (Estonian version)
* https://github.com/holgervirro/mcarto2023/blob/master/Map_Window_Management.ipynb (English version)

The second tutorial focuses on additional map elements, such as point symbols and different cartographic line objects (orthodrome, rhumb line, almucantar)
* https://github.com/holgervirro/mcarto2023/blob/master/Kaardielemendid.ipynb (Estonian version)
* https://github.com/holgervirro/mcarto2023/blob/master/Map_Elements.ipynb (English version)

## Lab session
During the live lab session we will go through the aforementioned notebooks in the [Binder](https://jupyter.org/binder) computing environment. Binder will create a Python environment based on the file `environment.yml`, which lists the libraries used in this session. It will also provide the computational resources needed to run the notebooks online. We can then run and edit the notebooks in the browser without setting up an Anaconda environment ourselves.

Click the Binder icon below to launch the environment and access the notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/holgervirro/mcarto2023/HEAD)

**NB** As Binder works online, edits made in the notebooks will not be saved if you close the browser or quit the environment. You might also get a timeout message if the notebook stays inactive, so Binder will ask to restart the kernel, which also resets your progress.

If you wish to save your task solution progress then you should either
* download the notebook (*.ipynb*) and then continue working using your own Anaconda setup (see below)
* copy the cell content of your solution somewhere (e.g. Notepad), so you could paste it when you restart Binder next time

![binder_download](https://github.com/holgervirro/mcarto2023/blob/1eb3f568488479606df9df23e7fc0f92786788d9/img/binder_download.PNG)

## Setting up Anaconda on your machine
We will use [Anaconda](https://conda.io/en/master/miniconda.html) for these exercises, which should already be installed in the computer class. For installing it on your own machine you can use the [tutorial](https://kodu.ut.ee/~kmoch/geopython2020/L0/Installing_Miniconda_GIS.html) provided by Alex Kmoch.

After installing Anaconda, download and unzip this repository into a folder you can find on your machine.

`Code -> Download ZIP`

Find and launch the Anaconda Prompt using the search bar.

Now move to the folder where you unzipped the GitHub repository.

`cd C:\Users\Holger\mcarto2023-main\mcarto2023-main`

You should be able to see the content of this folder with the `ls` command.

![folder](https://github.com/holgervirro/mcarto2023/blob/1eb3f568488479606df9df23e7fc0f92786788d9/img/folder.PNG)

We will start by creating an Anaconda environment using the existing environment file `environment.yml`, which installs all Python libraries needed for the two exercises.

`conda env create -f environment.yml`

The next command will activate the Anaconda environment we just created.

`activate mcarto2023`

Before we start Python coding we will make our newly created conda Python environment known to the Jupyter notebook system by installing the kernel, basically the execution engine link from Jupyter web notebook to our Python environment.

`python -m ipykernel install --user --name mcarto2023`

Finally, we can activate the Jupyter environment.

`jupyter lab`

A browser window will open where clicking on a Jupyter notebook file with the extension *.ipynb* allows you to start editing the notebook.
