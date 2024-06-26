SNUB (Systems Neuro Browser)
============================


.. image:: https://joss.theoj.org/papers/10.21105/joss.06187/status.svg
   :target: https://doi.org/10.21105/joss.06187
   
`Github Repository <https://github.com/calebweinreb/SNUB>`_

.. image:: ../media/use_case1.gif
   :align: center

|

**SNUB is a visual interface** for systems neuroscience. Using a set of linked data-views, users can explore relationships between raw video, 3D animal pose, behavior annotations, neural activity, or any other relevant time-series data.

Loading data is simple with the ``snub.io`` module. For example the following code creates a new project with paired electrophysiology and video data. 

.. code-block:: python

   import snub.io

   project_directory = 'path/to/new/project'

   snub.io.create_project(project_directory, duration=1800)
   snub.io.add_video(project_directory, 'path/to/my_video.avi', name='IR_camera')
   snub.io.add_spikeplot(project_directory, 'my_ephys_data', spike_times, spike_labels) 


We also support automatic conversion of NWB files to SNUB projects for a limited set of NWB neurodata types. 


SNUB Documentation
------------------

.. toctree::
   :maxdepth: 2

   install

   tutorials

   gui

   nwb

   api


