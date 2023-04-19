=====
Usage
=====
When you open the app you will be presented by the following screen

.. image:: images/initial.png
   :width: 600

To begin using the app,  click on the "Paste broadening simulation" button.

Preparation
===========

You will be presented the app interface where you can enter all the quantity you need for your case.

.. image:: images/rheometer_image.png
   :width: 600
   :align: center


-Loading experimental data 
----------------------------
The first step is to upload the experimental data in the upper part of the screen and click on Configure 

.. image:: images/rheometer_image_1.png
   :width: 600
   :align: center

-Simulation parameters
-------------------------
In the lower part of the screen you need to define the simulation parameters. 

.. image:: images/rheometer_image_2.png
   :width: 600
   :align: center

The parameters are described in more detail below:


* **Final time**: This parameter sets the duration of the simulation, starting from time 0. The simulation will run until the final time is reached.
* **Simulation deltaT**: his parameter sets the time step used in the simulation. A smaller time step will result in a more accurate simulation, but will require more computational resources.
* **Upward velocity**: This parameter sets the upward velocity induced by the grid being lifted. The velocity is depicted in the figure below, and is a key factor in the rheometer simulation.
* **writeinterval**: This parameter determines how often the simulation values will be saved. It must be larger than the time step.
* **Initial paste wide**: This parameter sets the initial size of the deposed paste. This is also depicted in the figure below, and is an important input for the simulation..
* **Run the rheometer app**: This option determines whether or not to run the parameter estimation and rheometer steps of the application. If left unchecked, the paste broadening app will run with default values.

.. figure:: images/define_quantities.png
   :width: 400
   :align: center
   
Once everything is set, you can click on the `Setup simulation` button.

Running
=======

A screen summarizing the simulation settings will appear, along with an option to run the simulation:

.. figure:: images/prepare2run.png
   :width: 400
   :align: center

when you click on the *Run simulation*, you will see the *Simulation Status* change from *CREATED* to *INPROGRESS*

.. figure:: images/running.png
   :width: 400
   :align: center

click on the *Refresh status* button, until the *Simulation Status* change from *INPROGRESS* to *COMPLETED*, 

.. figure:: images/running_completed.png
   :width: 400
   :align: center


Results
=======
When a simulation is completed you will be offered two option, *Dowload Simulation* or *Postprocessing*


-Download results
-------------------------
If you click on *Dowload Simulation*, you will see the screen below, which allows you to dowload the simualtion data and results.

.. figure:: images/download.png
   :width: 400
   :align: center


-Postprocessing
-------------------------
To access the default post-processed results, simply click on the "Postprocessing" button, as shown in the image below.

.. figure:: images/postprocess_button.png
   :width: 400
   :align: center

Once you've clicked on "Postprocess results," you will see a screen that looks similar to the one below:

.. figure:: images/post_process.png
   :width: 600
   :align: center

The resulting plots are described in more detail below:

* **Rheometer results** This section shows a comparison between numerical and  experimental rheometer data
   * **Moduli**: This plot compares G' and G''.    
   * **Viscosity**: This plot compares viscosity.

* **Paste simulation results**: This section displays the results from simulation.
   * **Paste broadening**: This plot shows the time evolution of the normalized paste broadening, which is calculated by dividing the paste width at time t by the initial width value.
   * **Interface comparison**: This plot compares the initial interface, with the interface at the end of the simulation.
