Description of the workflow steps
=================================

.. _parameter_e:

1: Parameter estimation
-----------------------

Experimental rheometer data for a certain paste is taken as input for a parameter optimization script, 
which uses the Giesekus model equations to determine the constitutive properties required for the simulation. 

.. _rheometer:

2: Rheometer
------------

The second step is a simulation of the rheometer. The constitutive properties from the parameter optimization 
are used in an OpenFOAM simulation with rheotools, where the rheometer is simulated and the results are compared 
with the experimental data for validation of the obtained constitutive properties.


.. _paste_settling:

3: Paste settling
-----------------

Finally, the same constitutive properties are used for a full multiphase simulation of paste levelling, which is 
allowed to settle under gravity for the measurement of its spread.


The Paste Levelling App is built on top of this workflow, automating the three steps into a seamless sequence,
with no user input in-between each of the steps. To facilitate demonstration, the final levelling simulation 
is done with a two-dimensional version which can be simulated in a few minutes, instead of the days to weeks 
it can take for the full three-dimensional simulation.


