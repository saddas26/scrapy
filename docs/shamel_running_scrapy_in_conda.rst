============================
Shamel: Running Scrapy in Conda
============================

This document provides instructions to set up and run Scrapy in a dedicated Conda environment (`scrapy-env`). It also includes steps to activate, deactivate, and switch between the `base` and `scrapy-env` environments.

Creating the `scrapy-env` Environment
======================================

To create a new Conda environment named `scrapy-env` and install Scrapy, use the following commands:

.. code-block:: bash

    conda create -n scrapy-env python=3.10 scrapy

- **`-n scrapy-env`**: Creates an environment named `scrapy-env`.
- **`python=3.10`**: Ensures the Python version in the environment is 3.10.
- **`scrapy`**: Installs the Scrapy package and its dependencies.

Activating the `scrapy-env` Environment
=======================================

To activate the `scrapy-env` environment, use the following command:

.. code-block:: bash

    conda activate scrapy-env

You will see the prompt change to indicate that the environment is active (e.g., `(scrapy-env)` appears at the beginning of the line).

Deactivating and Switching Back to `base`
=========================================

To deactivate the current environment and return to the `base` environment, use:

.. code-block:: bash

    conda deactivate

To switch to the `base` environment explicitly, use:

.. code-block:: bash

    conda activate base

Verifying the Environment and Scrapy Installation
==================================================

To verify that you are in the correct environment and Scrapy is installed:

1. Ensure the environment is active:
   .. code-block:: bash

      conda activate scrapy-env

2. Check that Scrapy is installed by running:
   .. code-block:: bash

      scrapy

   If installed correctly, this will display the Scrapy command-line interface help text.

Launching Spyder in `scrapy-env`
===============================

If you plan to use Spyder with Scrapy, install Spyder in the `scrapy-env` environment:

.. code-block:: bash

    conda install spyder

To launch Spyder from the `scrapy-env` environment:

.. code-block:: bash

    spyder

Note: Ensure the `scrapy-env` environment is active before launching Spyder.

Troubleshooting
===============

- If you encounter issues with missing dependencies or errors, ensure you are in the correct environment by running:
  .. code-block:: bash

      conda info --envs

- For additional help, refer to the Scrapy documentation.

