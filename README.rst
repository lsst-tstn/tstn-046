.. image:: https://img.shields.io/badge/tstn--046-lsst.io-brightgreen.svg
   :target: https://tstn-046.lsst.io
.. image:: https://github.com/lsst-tstn/tstn-046/workflows/CI/badge.svg
   :target: https://github.com/lsst-tstn/tstn-046/actions/

#####################################
LOVE deployment configuration on k8s.
#####################################

TSTN-046
========

Here we describe the LOVE deployment configuration used on k8s.
We start with a brief description of how LOVE works, its different components and communication workflow.
From that we describe how the system is deployed on k8s, the different services that are part of the deployment and their role.
We proceed with a description of the issues we currently observe with the system as the number of users and traffic from the control system increases and finalize with a few ideas for future improvements.

**Links:**

- Publication URL: https://tstn-046.lsst.io
- Alternative editions: https://tstn-046.lsst.io/v
- GitHub repository: https://github.com/lsst-tstn/tstn-046
- Build system: https://github.com/lsst-tstn/tstn-046/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

.. code-block:: bash

   git clone https://github.com/lsst-tstn/tstn-046
   cd tstn-046
   make init
   make html

Repeat the ``make html`` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run ``make clean``.

The built technote is located at ``_build/html/index.html``.

Publishing changes to the web
=============================

This technote is published to https://tstn-046.lsst.io whenever you push changes to the ``main`` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://tstn-046.lsst.io/v.

Editing this technical note
===========================

The main content of this technote is in ``index.rst`` (a reStructuredText file).
Metadata and configuration is in the ``technote.toml`` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
