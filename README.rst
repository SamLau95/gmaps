.. Automatically generated from LONG_DESCRIPTION keyword in
.. setup.py. Do not edit directly.

gmaps (forked for Python 3)
=====

gmaps is a plugin for including interactive Google maps in the IPython Notebook.

Let's plot a heatmap of taxi pickups in San Francisco:

::

    In [1]: import gmaps

    # load a Numpy array of (latitude, longitude) pairs
    In [2]: data = gmaps.datasets.load_dataset('taxi_rides')

    In [3]: map = gmaps.heatmap(data)
            gmaps.display(map)

Installation
------------

Development version
^^^^^^^^^^^^^^^^^^^

The development version can be installed by cloning the git repository:

    $ git clone https://github.com/samlau95/gmaps.git

Change to the project's root directory and run::

    $ python setup.py install

Alternatively, if you are planning on doing development with `gmaps`, install `gmaps` in
development mode using::

    $ python setup.py install_data
    $ python setup.py develop

Getting started
---------------

Currently, only heatmaps are supported. Draw a heatmap by passing a list of (latitude, longitude)
pairs to the heatmap command.

There are example notebooks in the examples directory. You can view these on `nbviewer
<http://nbviewer.ipython.org/github/pbugnion/gmaps/blob/master/examples/ipy3/>`_,
but note that you need to download the notebook to actually see the Google Map.

Issue reporting and contributing
--------------------------------

Report issues using the `github issue tracker <https://github.com/pbugnion/gmaps/issues>`_.

Contributions are welcome. Read the CONTRIBUTING guide to learn how to contribute.
