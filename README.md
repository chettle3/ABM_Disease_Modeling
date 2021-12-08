# CMSE-202-Project

This repository contains the code and results for CMSE 202 group Health 4 group. For the purpose of not deleting possibly-useful code and files, there is a directoy named "Old Files". None of the files contained inside are meant to be read, run, or interacted with. The code associated with this project is present in the FinalProject.ipynb notebook. This notebook also contains MarkDown descriptions of the project. For proper formatting, read the file in Jupyter Notebooks, rather than through GitHub.

To run the code, first ensure that the following packages are installed:
* numpy
* matplotlib
* scipy
* sympy
* IPython
* ipywidgets

Run all the cells in order under the "Infectivity Function", "Distance Function", and "Exposure Function" headers. Feel free to interact with any widgets; the widgets do not affect the final model, and are for demonstration purposes only. To modify the average values of the parameters (especially the inflection point in the exposure function), find the cell calling get_var_dist for that parameter, and change the input. Then rerun all cells again.

Run the cell containing the class definitions. Then, run the next cell which defines env as an Environment object (different parameters can also be passed in this cell). Then run the cell which begins the model. If frames are to be saved, ensure that the line plt.savefig("output/output"+str(env.time)) is uncommented and that a directory named output is present. Otherwise, comment this line. When you are ready to terminate the model, interrupt the kernel in Jupyter.

In the case that frames were saved, VirtualDub can be used to create a video. This software was not written by us; all credit goes to Avery Lee (a copy of the executable files was placed in this GitHub for convenience). For more details on how to use this software, visit https://www.virtualdub.org/.

Our simulations in video form are publically available at https://www.youtube.com/playlist?list=PL2anvfQdkVC6YSsrAosSeLdKwS_g0H3Ts. To view these videos in the Jupyter Notebook, run the subsequent cells containing calls to YouTubeVideo.

Finally, to see the SIR models (both the original and the one for reinfection, run the remaining two cells. To obtain the same graphs shown in the images, change the values of the initial_conditions and beta accordingly. Note that the initial conditions if not specified are \[1000,1,0\].

The work breakdown in our group was as follows:
* Matei Gheorghiu
	* Make SIR models
	* Write the writeup in a Jupyter Notebook
	* Add images to the Jupyter Notebook
* Jared Bloch
	* Code the model for reinfection
	* Help analyze the simulations
	* Help write and create the presentation
* Cong Fu
	* Code an initial model for disease spreading
	* Code the model for death
	* Help analyze the simulations
	* Help write and create the presentation
* William Chettleburgh
	* Code the main model for disease spreading
	* Run the model and save output as videos
	* Comment the code
	* Help analyze the simulations
	* Help write and create the presentation
