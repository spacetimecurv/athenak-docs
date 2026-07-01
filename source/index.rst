AthenaK documentation
=====================

.. figure:: /_static/athenak_hero.png
   :alt: AthenaK simulation
   :align: center
   :width: 100%

   Rayleigh--Taylor instability computed with AthenaK, showing the adaptive
   mesh refinement (AMR) block structure tracking the turbulent mixing layer.

AthenaK is a block-based AMR framework with fluid, particle, and numerical relativity
solvers implemented with `Kokkos <https://kokkos.org/>`_ for performance portability.

This site covers how to obtain, build, and run the code.

.. toctree::
   :caption: Getting Started
   :maxdepth: 1

   requirements
   download
   build

.. toctree::
   :caption: Quickstart
   :maxdepth: 1

   quickstart

.. toctree::
   :caption: Running
   :maxdepth: 1

   running_the_code
   input_file
   outputs
   analysis
   notes_specific_machines

.. toctree::
   :caption: Grid and Initial Conditions
   :maxdepth: 1

   smr
   amr
   problem_generators
