**Notebooks** for Lectures and Exercises for the [SPCE0038: Machine Learning with Big-Data](https://moodle.ucl.ac.uk/course/view.php?id=51562) Module at UCL


# Running python Jupyter notebooks 
The notebooks can either be run locally on your own machine or on the cloud.  The advantage with the cloud setup is that you do not need to configure a machine, although free compute is limited.

# Running on the cloud with Colab
The notebooks can either be run on Google's [Colab](https://colab.research.google.com/) cloud computing platform.  Follow the link at the top of each notebook or at the top of each lecture in the book to a version running on Colab. 

You will only have read access to the version of the notebook that is running on Colab but you can simply make a copy of the notebook on your own Google Drive in order to make and execute any changes.

# Running locally
A python environment is required to run the notebooks on a local machine. We present here instructions for using [Anaconda](https://www.anaconda.com/), although other Python setups could be used.  

An environment to run the notebooks can be set up with the versions of the libraries in requirements.txt *(included below)*, following the steps below in terminal *(MacOS)* or **anaconda prompt** *(Windows)*: 

1. Create an environment named `mlbd` with Python 3.11.
```bash
conda create --name mlbd python=3.11
```
2. Activate the `mlbd` environment and then install the libraries in the `requirements_new.txt` file. 
```bash
conda activate mlbd
pip install -r requirements.txt  
```
3.Finally, start **Jupyter lab**, which will open the explorer and let you run the notebooks.
```bash
jupyter lab
```
 
**Note for Windows users:** it has been reported that you might get an error message when opening any Jupyter notebooks, on the lines of `ImportError: DLL load failed while importing win32event` - this is related to Python 3.8 on Windows only. If you hit this issue, you can try to remove and reinstall the environment, or if that does not work, execute `pip install pywin32==225`. If the problem persists, feel free to reach out to any demonstrators and they will be happy to help you.

Try and bypass this problem by using **WSL**
