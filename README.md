# Setting up Environments and Installing Packages Using Conda

## Summary of steps to complete

- [x] Fork this repository so you have your own copy to work on.
- [x] Clone the repository on your local machine. 
- [x] Edit this README.md file on your machine.
- [x] Run the Conda commands shown in the video and describe them in the table below.
- [x] Push your changes to your GitHub repository.
- [x] Submit a link to this GitHub repository in Canvas.

## 1. Fork & Clone this repository

* We did this in a previous assignment. Instructions are here: https://github.com/cmcntsh/exerGitPractice
* This can also be done directly in VSCode
  * Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
  * Copy the Clone or Download path for this repository from GitHub.
  * In VSCode from the command pallette (Ctrl-Shift-P) run Git: Clone
  * Paste the path into the path field which pops up
  * Select your new folder you created on your machine
  * A new folder for the repository with the repository files should be in the folder you selected showing in the Explorer window in VSCode on the left side.
  
## Edit your README.md file

* [x] In an editor of your choice (i.e. VSCode) edit this README.md file to add the answers requested in the tables.

## Follow along with this tutorial

* Conda What and Why? (27 min): https://www.youtube.com/watch?v=23aQdrS58e0&list=PLG9A6ovzPqX6d9uWzx0UYN9pm0zzl5ofA&index=13&t=0s
  * He installs Miniconda. We will be using Anaconda. Don't install Miniconda.
  * Follow along with the rest of the tutorial.
  * Go ahead and create the environments as he creates them in the tutorial.
  * (2021 update: I recommend managing environments as shown in the new Anaconda introduction video. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial) If you want to try creating the environments using the user interface for Anaconda Navigator instead of the command line shown in the Conda What and Why tutorial, that's fine. But watch the Conda What and Why tutorial to understand some of the differences between Conda environments and other types of virtual environments available in Python.

## Conda Concepts

* [x] Describe the Conda concepts used in the video and listed in the table below.

|   Concept   |         Description or short answer         |
|     ---     |                     ---                     |
|What is the purpose of having different environments?     |(To have purpose-built virtual machines customized to a specific project or use case and configured to avoid problems and invonvenience)|
|What is the default package manager in Python?            |(pip is Python's integrated package manager)|
|How do you manage environments and packages in Anaconda?  |(Conda is both a package and environment manager in Anaconda)|
|`conda list`       |(Lists all packages in the currently active environment)|
|`conda env list`       |(Lists all environments)|
|How do you keep your base environment unchanged?       |(Create, activate, and work in new environments)|
|What is the link to the Conda cheat sheet? (link in video notes is broken)      |(https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf)|
|`conda create --name XXXX`       |(Creates a new environment)|
|`source activate XXXX`       |(Activates a named environment for active use)|
|`conda install YYYY`       |(Installs named package in the active environment)|
|channels in Conda       |(Channels are different sources of packages and can be official, community supported, or private)|
|`conda install -c ZZZZ YYYY`       |(Installs a package YYYY if found within the specified channel ZZZZ)|
|`conda config --show channels`       |(Lists all channels that have been added to conda for package search)|
|`conda config --add channels ZZZZ`       |(Adds a channel for permanent search availability from default or base environment)|
|conda-forge.org       |(A community-supported channel for packages)|
|`source deactivate`       |(Deactivates the current channel and returns to base)|
|`conda config --get channels`       |(Allows user to set priority of channel search)|

* After creating the environments he created in the video on your computer, what would the results of running the command `conda env list` look like with the da35 environment activated. Paste the output from your command prompt in the code block below.

```
(da35) Joshuas-Mini:~ josh$ conda env list
# conda environments:
#
base                     /Users/josh/opt/anaconda3
ai37                     /Users/josh/opt/anaconda3/envs/ai37
da35                  *  /Users/josh/opt/anaconda3/envs/da35

(da35) Joshuas-Mini:~ josh$ 


```
* What command would you use to remove the environments you created for this exercise from your computer?

```
conda env remove --name ()

```
## 2021 Update
Python, Anaconda, and many programming languages are constantly evolving. The video Conda What and Why provides a great explanation of why you may want to use virtual environments for your Python projects, and it provides a nice demonstration of how to work in the command line. However, environment management using Anaconda Navigator is more user friendly than ever. I personally will be using Anaconda Navigator to manage environments and packages since it seems easier to see what is going on using the GUI. If you haven't done so already watch the introduction to Anaconda video and pay close attention to the section on using Anaconda Navigator to create environments and install packages. https://anaconda.cloud/tutorials/getting-started-with-anaconda-individual-edition%3Fsource%3Dindividual-edition-tutorial
