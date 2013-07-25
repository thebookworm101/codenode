Codenode - Interactive Programming Notebook for the Web Browser
===============================================================

For complete documentation, please see: http://codenode.org/docs

Quickstart
----------

**Quick Install:**

::

  $ easy_install codenode


**Recommend Install:**

:: 

  $ easy_install -U virtualenv pip 
  $ virtualenv --no-site-packages mycodenode_env
  $ pip -E mycodenode_env install codenode


**Quick Start:**

::

  $ codenode-admin codenode_desktop
  
Now open browser to http://localhost:8000


**Plotting**

To use maplotlib, install matplotlib and numpy:

::

  $ pip install numpy
  $ pip install matplotlib

or if there are missing dependency issues, get the development libraries through the normal 
channels on your OS. For Ubuntu:

::
  $ sudo apt-get install  libfreetype6-dev   libpng-dev
  $ sudo apt-get install  python-numpy-dev
Now use pylab commands in a notebook, and call `show()` to render the plot.
  

Support
-------
Please ask any questions or give any feedback!
For help and feedback, go here: http://groups.google.com/group/codenode-devel


License
-------
Codenode is free software, licensed under the BSD. See the ``LICENSE`` file.


Changes 
-------

**v0.03** 
 - Jquery 1.4 update
 - Images saved as base64 in the cell contents in the database, rather than as files
 - Delete empty cell when pressing backspace (#49)
 - Suppress accidental back when pressing backspace (#51)
 - Save and restore open/closed state of cells (#55)

**v0.02**

Deleting cells:

- can delete cells by highlighting bracket and pressing backspace
- context menu action for cell deletion
- cell deletion causing notebook save

Django 2.1 Compatibility:

- Updated audit trail
- CSRF fixes

Chrome issues: 

- fixed width font
- notebook renaming partial fix

Other issues:

- ask user before navigating away from a page with unsaved changes
- hide save as buttons 
- empty revision list does not cause error with new notebook
- better image handling in engine output

**v0.01** 

Initial release
