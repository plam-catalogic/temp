
============
 SPP Client
============

This project aims to build a Python client for IBM Spectrum Protect

This repo holds two components. 

- An SDK that can be used by anyone interested in integrating SPP
  operations in their workflow.

- A command line utility with which SPP operations can be performed.

Installation
============

::

$ pip install sppclient

Usage
=====

::

    $ sppcli --help
    
    # This connects to SPP on localhost.
    $ sppcli --user admin --passwd <PASSWORD> job list
    
    # To connect to a different host. Default user is "admin".
    $ sppcli --url https://1.2.3.4:8443 --passwd <PASSWORD> job list
    
Notes
=====

- After a successful login, the command "remembers" the login session
  so there is no need to pass user name and password with every
  run.

