.. WildfireWiki documentation master file, created by
   sphinx-quickstart on Sun Jul 11 11:17:23 2021.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to WRF-Fire Wiki Page!
==============================

Introduction to WRF-Fire
------------------------

.. raw:: html 
 
   <a href="https://ral.ucar.edu/solutions/products/wrf-fire-wildland-fire-modeling" target="_blank">WRF-Fire</a> is a two-way coupled atmosphere - wildland surface fire simulation platform within the Advanced Research WRF (ARW) dynamical core. WRF-Fire is a Numerical Weather Prediction model (WRF-ARW) coupled with a semi-empirical fire spread model based on the Rothermel’s semi-empirical Rate of Spread (ROS) model, meaning it does not simulate the physical processes governing the combustion process. As a two-way coupled wildland fire-atmosphere model, WRF-Fire takes into account the coupling between the fire and the atmosphere. The fire behavior model receives the wind components from the WRF atmospheric model to propagate the fire, and feeds the sensible and latent heat flux back to the atmospheric model to disturb the atmosphere state allowing the fire to “create its own weather”. This feature results in more realistic wildfire propagation compared to other operational wildland fire simulation platforms such as FARSITE, which is an uncoupled surface fire propagation platform based on the same Rothermel’s ROS model and Huygen’s wave principle. Moreover, as a result of using the computationally efficient semi-empirical ROS model as well as parallelization and proper scalability, WRF-Fire has been used for operational simulation of wildland fire. <br><br>
 
How to Use this Wiki and Where to Begin?
----------------------------------------
This Wiki aims to tutor WRF-Fire using a variety of examples with incrementally increasing level of complexity, ranging from basic uncoupled models to nested coupled models in the LES mode. In addition, tutorials are provided on :ref:`Compiling WRF-Fire for Mac <compileMac>`, :ref:`Compiling WRF-Fire for Linux <compileLin>`, :ref:`Running WRF-Fire <runWRF>`, :ref:`Key WRF-Fire and WRF commands <keyCommands>`, and :ref:`Visualization tools <visualization>`.

**If you have preliminary experience with WRF and/or WRF-Fire,** start with the examples along with the commands tutorials to learn WRF-Fire. You can also review the visualization tutorials, which include Python codes developed exclusively for visualizing WRF-Fire outputs.

**If you are a new user to WRF world,** we suggest to pursue the following steps to get acquainted with WRF-Fire. 

 * :ref:`Step 1:<DCR>` Run WRF-Fire for idealized cases.
 * :ref:`Step 2:<idealized>` Compile ne of the test cases, namely “hill_simple” and “two_fires”, distributed with WRF-Fire.
 * :ref:`Step 3:<Ncview>` Visualize the outputs of test cases using Ncview.
 * :ref:`Step 4:<tutorials>` After getting acquainted with WRF-Fire, follow the examples and commands tutorials to learn how to create different WRF-Fire models. You can also follow visualization tutorials for more visualization tools and options.

Enjoy learning WRF-Fire! 

About Us 
--------
This Wiki has been developed through collaboration between teams from the University of Nevada, Reno and University Corporation for Atmospheric Research (UCAR). The development of this wiki page has been sponsored by the `NSF LEAP-HI Grant #1953333 <https://www.nsf.gov/awardsearch/showAward?AWD_ID=1953333&HistoricalAwards=false>`_ and UCAR funding.

The development team includes:

   * `Hamed Ebrahimian <https://www.unr.edu/cee/people/hamed-ebrahimian>`_, Assistant Professor, University of Nevada, Reno
   * `Kasra Shamsaei <https://www.linkedin.com/in/shamsaei/>`_, Ph.D. Student, University of Nevada, Reno
   * `Timothy Juliano <https://staff.ucar.edu/users/tjuliano>`_, Project Scientist I, NCAR
   * `Nataliia Igrashkina <https://www.linkedin.com/in/nataliia-igrashkina-87145598/>`_, Ph.D. Student, University of Nevada, Reno
   * Evan Chinn, B.Sc. Student, University of Nevada, Reno
   * `Branko Kosovic <https://staff.ucar.edu/users/branko>`_, Director of the Weather Systems and Assessment Program, NCAR
   * `Ertugrul Taciroglu <https://samueli.ucla.edu/people/ertugrul-taciroglu/>`_, Professor, University of California, Los Angeles (UCLA)

To read more about our project and progress, `visit here <https://packpages.unr.edu/wildfireproject>`_.

For questions and comment about this wiki page, please contact Dr. Hamed Ebrahimian at hebrahimian@unr.edu, or Kasra Shamsaei at kasra.sh@nevada.unr.edu. 

For technical questions about WRF-Fire, please contact Dr. Branko Kosovic at branko@ucar.edu.

How to Cite this Wiki?
----------------------
Please cite this work as:

.. code-block:: none

   Shamsaei, K., Juliano, T., Igrashkina, N., Ebrahimian, H., Kosovic, B., Taciroglu, E. (2022) WRF-Fire Wikipage. doi: 10.5281/zenodo.6667633 [access date]
    
.. note::

Please modify the above [access date] to the date you accessed this Wiki.

.. note::

   This project is under active development.

.. toctree::
   :maxdepth: 2
   :caption: Contents

   DCR
   input_files 
   csHome
   visuHome
   faq
   forum
