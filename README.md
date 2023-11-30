# Alt_Process_Jupyter_Notebooks
Jupyter Notebooks for processing curve data for use in producing curves for digital negative printing

## Introduction
Making digital negatives for alternative process photography is a time and labor intensive process.  Several methods have been implemented over the years, and one of the most prominent is [Easy Digital Negatives](http://www.easydigitalnegatives.com/)  This site allows you to upload scans of printed step charts, and it will yield correction curves for whatever process you are working with.  

One problem though, is that Easy Digital Negatives can generate curves that are jaggy and low-detail, and smoothing them out manually is not an easy process.  Furthermore, using an iterative process to refine the curve shape with successive tests can be done, but again may generate some severe artifacts due to the jaggy, low-detail curves.  

This collection of Jupyter Notebooks aims to help with some of these problems.
## Important Note
The Jupyter Notebooks contained here are easy to use, but will require you to do a few things via command prompt.  You will need to install a Miniconda environment (free) and install a few libraries (also free).  You will also be exposed to a bunch of Python code that could frighten you.  Don't worry - you will not be modifying any of the code unless you want to.  If you're OK with doing a few commands in a command prompt and clicking a "run" button a few times, then you will be fine. 

## Operating System
This Readme was written describing the procedures needed to get Jupyter Notebook running on a **Windows OS** system.  The Python code is operating system agnostic, so you can run it on any OS you wish, but you'll need to figure out the steps to install and run Jupyter Notebook yourself if you're not using Windows.
## Installation instructions
You will need to perform the following:
1. [Install Miniconda](https://github.com/MP120TC/Alt_Process_Jupyter_Notebooks/tree/main#install-miniconda)
2. [Install libraries](https://github.com/MP120TC/Alt_Process_Jupyter_Notebooks/tree/main#install-libraries)
3. [Copy Jupyter notebook .ipynb files to folder of your choosing](https://github.com/MP120TC/Alt_Process_Jupyter_Notebooks/tree/main?fbclid=IwAR2EDq2OzVhtLUIVt2Et8zPfzHBOJfsW4RC-Pgjt403yz0RdhxBBkuOA2Hc#copy-jupyter-notebook-ipynb-files-to-folder-of-your-choosing)
#### Install Miniconda
You'll want to do the following:
1. Create a new folder on your computer in a convenient location other than your desktop.  You'll be typing this path in the command prompt window, so make it easy, like C:\Miniconda
2. Visit https://docs.conda.io/projects/miniconda/en/latest/miniconda-other-installer-links.html and download an installer.  Python 3.9 is a good choice, but you can try any version available.
3. Run the Miniconda installer.  **Do not just accept the defaults!**  If you are knowledgeable, you can make these choices as you see fit, but if you don't know, do the following:
   - It is recommended to install for **All Users**
   - For the **Destination Folder** use the folder you created instead of the default suggestion
   - Do **NOT** Add Miniconda 3 to your PATH environment variable
   - Do **NOT** Register Miniconda 3 as your default Python
   - If you wish to Clear the Package cache, go ahead - it shouldn't cause issues
#### Install Libraries
Perform the following:
1. Open a command prompt window (If you run into permission problems installing packages, run cmd as administrator)
2. Type the following path in the command prompt window `<path where you installed Miniconda>\Scripts\activate`  **Example:** If you installed Miniconda into C:\Miniconda, you'd type `C:\Miniconda\Scripts\activate`
3. Type the following command: `conda install jupyter`  When prompted Y/n, choose Y to install
4. Type the following command: `conda install pandas`  When prompted Y/n, choose Y to install
5. Type the following command: `conda install scipy`  When prompted Y/n, choose Y to install
6. Type the following command: `conda install matplotlib`  When prompted Y/n, choose Y to install
7. You can close the command prompt window.  **You've done the hard part now, so pat yourself on the back!**
#### Copy Jupyter notebook .ipynb files to folder of your choosing
You may put the Jupyter notebook .ipynb files anywhere you wish.  It is recommended that you puth them somewhere convenient to type, like C:\Alt_Process\Notebooks. In other words, **not in a folder on your desktop**!  Make sure you remember where they are.  

While you're at it, you might want to create a sub-folder beneath the Jupyter Notebooks folder where you place .csv and .cube files you are working on.  This will help you save some digging around for files.
## Running Jupyter Notebook
The steps to run Jupyter notebook are:
1. Open a command prompt window
2. Navigate to the folder you wish to work in.  This is usually where you put your notebooks.  If, for example, you put your notebooks in a folder named C:\Alt_Process\Notebooks, you would type the following command: `cd C:\Alt_Process\Notebooks`  **If you forget this step, you may not be able to navigate to the folder you put the notebooks into!**
3. Type the following command: `<path where you installed Miniconda>\Scripts\activate` **Example:** If you installed Miniconda into C:\Miniconda, you'd type `C:\Miniconda\Scripts\activate`
4. Type the following command: `jupyter notebook`
5. Your web browser will open, and the Jupyter home page will open.  You can then choose whichever notebook you wish to use.
## Jupyter Notebook Execution
When you choose a notebook, it will open in a separate tab.  Code is organized into "cells".  There are also cells that contain notes, called Markdown cells.  Note the menu along the top.  You can select a cell in the notebook and click the Run button to run the cell.  When you are done running the notebook, choose File->Close and Halt.  You don't need to save the notebook unless you want to.  Even if you save it, you will still need to re-run all the cells next time you open it.
## License
This work is licensed under **CC BY-NC-SA 4.0**
You are free to:
* Share — copy and redistribute the material in any medium or format
* Adapt — remix, transform, and build upon the material
  
The licensor cannot revoke these freedoms as long as you follow the license terms.
Under the following terms:
* Attribution - You must give appropriate credit , provide a link to the license, and indicate if changes were made . You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
* NonCommercial - You may not use the material for commercial purposes .
* ShareAlike - If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
*No additional restrictions - You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
