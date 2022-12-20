# CMSE-202-Project

This was my final project for CMSE 202, completed in a group with Matei Gheorghiu, Jared Bloch, and Cong Fu. The project simulates the spread of a disease using an agent-based model, and we compare the results with those found by a traditional SIR compartmental model. My primary role was in coding the base model (from which several variations were made), as well as running and recording the simulations.

To run the code, first ensure that the following packages are installed:
* numpy
* matplotlib
* scipy
* sympy
* IPython
* ipywidgets

Run all the cells in order under the "Infectivity Function", "Distance Function", and "Exposure Function" headers. Feel free to interact with any widgets; the widgets do not affect the final model, and are for demonstration purposes only. To modify the average values of the parameters (especially the inflection point in the exposure function), find the cell calling get_var_dist for that parameter, and change the input. Then rerun all cells again.

Run the cell containing the class definitions. Then, run the next cell which defines env as an Environment object (different parameters can also be passed in this cell). Then run the cell which begins the model. If frames are to be saved, ensure that the line plt.savefig("output/output"+str(env.time)) is uncommented and that a directory named output is present. Otherwise, comment this line. When you are ready to terminate the model, interrupt the kernel in Jupyter.

In the case that frames were saved, various softwares can use this to form a video, such as VirtualDub (https://www.virtualdub.org/).

Our simulations in video form are publically available at https://www.youtube.com/playlist?list=PL2anvfQdkVC6YSsrAosSeLdKwS_g0H3Ts. To view these videos in the Jupyter Notebook, run the subsequent cells containing calls to YouTubeVideo.

Finally, to see the SIR models (both the original and the one for reinfection, run the remaining two cells. To obtain the same graphs shown in the images, change the values of the initial_conditions and beta accordingly. Note that the initial conditions if not specified are \[1000,1,0\].
