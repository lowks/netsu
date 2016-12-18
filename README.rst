netsu Network Supervisor
````````````````````````

.. image:: https://travis-ci.org/netsu-project/netsu.svg?branch=master
    :target: https://travis-ci.org/netsu-project/netsu

.. image:: https://coveralls.io/repos/github/netsu-project/netsu/badge.svg?branch=master
    :target: https://coveralls.io/github/netsu-project/netsu?branch=master


Usage
-----

Get sources:

.. code:: shell

    git clone https://github.com/netsu-project/netsu
    cd netsu

Run checks and unit tests:

.. code:: shell

    pip3 install tox
    python3 -m tox

Install latest master release via pip:

.. code:: shell

    # install uwsgi and uwsgi-plugin-python3 via your favourite package manager
    pip3 install netsu

Install from sources:

.. code:: shell

    # install uwsgi and uwsgi-plugin-python3 via your favourite package manager
    python3 setup.py sdist
    cd dist
    pip3 install netsu-*

Some usage examples:

.. code:: shell

    # start service
    systemctl enable netsu-nm
    systemctl start netsud
    # query for running config
    netsu-ctl get running-config
    # set running config
    netsu-ctl set running-config '{}'
