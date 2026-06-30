Quickstart: First Run
=====================

Run AthenaK with an example input file and confirm your build works.

Prerequisite
------------

Complete :doc:`build` so ``build/src/athena`` exists.

Step 1: Parse an input file (no simulation run)
-----------------------------------------------

Use ``-n`` to validate parsing only:

.. code-block:: bash

   ./build/src/athena -i inputs/hydro/rt2d.athinput -n

This should print a parameter dump and exit successfully.

Step 2: Run a short simulation
------------------------------

Start from an input file and override runtime limits from the command line:

.. code-block:: bash

   ./build/src/athena \
     -i inputs/hydro/rt2d.athinput \
     job/basename=rt2d_smoke \
     time/tlim=0.05 \
     time/nlim=50

Expected outputs
----------------

Depending on the input file ``output*`` blocks, AthenaK writes files such as:

- ``*.hst`` history files
- ``*.bin`` binary outputs
- ``*.tab`` table outputs
- ``*.vtk`` visualization outputs

Troubleshooting
---------------

- ``No such file or directory`` for executable:
  Build step was not completed; run :doc:`build`.
- Input parse errors:
  Re-run with ``-n`` and inspect reported parameter block names and values.
- Wrong run directory:
  Use ``-d <directory>`` to choose output location.

Next steps
----------

- Explore additional problem setups in ``inputs/``
