# images-as-signals
code and data for 'Intermediate Image Analysis - Images as Signals' workshop

This workshop covers the application of conventional signal processing techniques to digital images. It is geared toward those with low-to-moderate programming experience, but beginners should be able to follow along with the provided tutorial code and examples. Students will learn how to apply Fourier transforms to their images and how to use them to perform common image analysis tasks.

Lesson material is found in the lessons/ folder. 

References:

Sample accelerometer data contributed to Kaggle by Swayam Mittal (CC0): https://www.kaggle.com/swayammittal65/wearable-motion-sensors/

bear\_kidney.png was derived from public data made available by the Korstanje Lab at the Jackson Laboratory. https://images.jax.org/webclient/?show=project-59  DNA Res. 2019 Feb 1;26(1):37-44. doi: 10.1093/dnares/dsy036.

## Before you begin

This workshop assumes that you know the basics of dealing with images in Python (i.e., you are familiar with the material [here](https://github.com/TheJacksonLaboratory/PythonImagingBasic)). If you are not, please work through the prerequisite material prior to attending this workshop.

## Tools we will be using

You will need to use three software tools in addition to Python for this workshop: git, conda, and jupyter.

[git](https://git-scm.com) is only used in this workshop to copy the course notes and code to your local computer, although it is a very powerful tool for managing your projects!

[conda](https://conda.io/docs/) is a tool used for two purposes: to create [environments](https://conda.io/docs/user-guide/tasks/manage-environments.html) for your projects and to manage Python packages. It will be a very good idea to read up on conda before you begin this course, spefically how to use environments.

[jupyter](http://jupyter.org) is a tool for developing your code in \"notebooks\" (file extension \*.ipynb) in a web browser. This course is based around a series of such notebooks (you are looking at a notebook now!). The main utility of using notebooks for image analysis is that you can save all of your output on the same page as your code, which helps you, and your collaborators, to follow the steps of an analysis.

## Setting up for the class

1. Clone the git repository to your computer.
    
    ```bash
    git clone https://github.com/TheJacksonLaboratory/images-as-signals.git

    ```
    **Windows Users**: You will first need to install [git](https://git-scm.com/download/win). Then you can use Git Bash to use the command shown above

    **As an alternative to using git**, you can also download the repository as a zip file at https://github.com/TheJacksonLaboratory/images-as-signals/archive/master.zip.
    

2. Install [Anaconda](https://www.anaconda.com/download/) (or [Miniconda](https://conda.io/miniconda.html))
    * This gives you access to the `conda` Python package management system
    * **Windows Users**: You may want to opt for the full install of Anaconda. This will give you "Anaconda Prompt" which will make it easier for you to follow along here.
    
    
3. Using conda in a terminal window (or Anaconda prompt in Windows), navigate to the root directory of this workshop (should be called `images-as-signals` and create a virtual environment from the `environment.yml` file.
    ```bash
    conda env create -f environment.yml
    ```
  
4. Launch Jupyter from the Anaconda launcher or command line (`jupyter notebook`).