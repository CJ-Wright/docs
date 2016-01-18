.. NSLS-II arch documentation master file, created by
   sphinx-quickstart on Sun Jan 18 10:00:09 2015.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

NSLS-II Software Documentation
******************************

We are deploying an event-based data collection and analysis framework.

.. image:: _static/collection-overview.png
   :align: center

Software Packages
=================

The following software packages work together to handle different aspects of
data collection and analysis. They interoperate by sharing a common
`event-based model <architecture>`_. Each package has its own detailed
documentation, linked below.

* Data Collection Packages
    * `bluesky <http://nsls-ii.github.io/bluesky>`_ -- a framework for specifying and executing experiments
    * `ophyd <http://nsls-ii.github.io/ophyd>`_ -- a collection of Python objects that represent hardware, providing a common high-level interface
* Data Access Packages
    * High-level Data Access
        * data broker -- a simple interface that pulls together data from all sources
    * Low-Level Data Storage and Access
        * metadataclient (preferred), metadatastore (deprecated)
        * filestore
* Data Munging Packages
    * datamuxer
* Scientific Data Processing Packages
    * the built-in subscriptions in `bluesky <http://nsls-ii.github.io/bluesky>`_
    * Beamline-specific \*tools repositories:
        * `csxtools <https://nsls-ii-csx.github.io/csxtools/>`_
        * `chxtools <https://github.com/NSLS-II-CHX/chxtools>`_ (undocumented)
        * `hxntools <https://github.com/NSLS-II-CHX/hxntools>`_ (undocumented)
        * `xpdtools <https://github.com/NSLS-II-XPD/xpdtools>`_ (placeholder)

Table of Contents
=================

.. toctree::
   :maxdepth: 2

   architecture-overview
   collection-quick-start
   analysis-quick-start
   sandbox
   deployment-details
   resources
   technologies
