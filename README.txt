Build process
=============

Build development environment::

    git clone git@github.com:EUDAT-DPMT/dpmt_buildout.git
    cd dpmt_buildout
    virtualenv . (or virtualenv-2.7 .)
    bin/python bootstrap-buildout.py
    bin/buildout -c dev.cfg

Build production environment::

    git clone git@github.com:EUDAT-DPMT/dpmt_buildout.git
    cd dpmt_buildout
    virtualenv . (or virtualenv-2.7 .)
    bin/python bootstrap-buildout.py
    bin/buildout 

Starting Plone (production)::

    bin/zeo start
    bin/zeoclient1 start # port 8081
    bin/zeoclient2 start # port 8082
    bin/zeoclient3 start # port 8083

Starting Plone (dev)::

    bin/instance fg # port 8080

