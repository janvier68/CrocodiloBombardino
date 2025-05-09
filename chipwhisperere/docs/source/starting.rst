.. _starting:

#####################
Running ChipWhisperer
#####################

After finishing the installation process, there are two different ways of
using the **chipwhisperer** software. You will most likely be using a Jupyter
server to run a Jupyter notebook inside of your browser. 

*****************
Jupyter Notebooks
*****************

Recommended reading for using Jupyter notebooks:

* `Jupyter Notebook ReadTheDocs <https://jupyter-notebook.readthedocs.io/en/stable/>`_

Here is a quick start guide based on you having finished the installation
of **chipwhisperer**. It only covers steps unique to our chipwhisperer/Jupyter
installation. 

If you've installed via the VirtualBox VM image:
------------------------------------------------

#. Open VirtualBox and start the virtual machine

#. Open your browser outside the VM

#. Connect to localhost:8888 in your browser


If you've installed via the Windows Installer:
----------------------------------------------

#. Run the ChipWhisperer shortcut (this shortcut is available in the
   ChipWhisperer install folder, the start menu, and optionally as a shortcut
   on the desktop.)

If you've installed natively:
-----------------------------

#. Make sure you are using a `bash`-like terminal. Many of the Jupyter
   notebooks use bash to run **make** or remove files for building
   firmware. This may be changed in the future but for now it is
   required. If you installed using the Virtual Machine (VM) the
   terminal is a bash like terminal and you should have no problem.
   If you installed on linux, same deal. However, if you installed
   on Windows/Mac you may have to install a bash like terminal. If
   you installed Git to install **chipwhisperer** you already have
   **git-bash** available to you. Here are a few bash-like terminals
   available on other windows:

   * (Recommended) `Git-Bash <https://git-scm.com/>`_ (make sure you select to
     install git bash during the installation of Git.)

   * `MinGW <http://mingw.org/>`_

   * `Cygwin <https://www.cygwin.com/>`_


Next:
-----

#. Start the bash terminal. Make sure you have access to
   **chipwhisperer** in the terminal using::

        python -c "import chipwhisperer as cw"

   This should exit without printing anything. If you get something
   like "module not found" then you should read up on PYTHONPATH and
   system PATH.

#. Navigate to the **chipwhisperer** directory. If you installed
   **chipwhisperer** to /home/user/chipwhisperer then use:

   .. code:: bash

       cd /home/user/chipwhisperer

#. Start the Jupyter Server in that directory:

   .. code:: bash

       jupyter notebook

   The Jupyter Notebook Server interface should be automatically opened in
   your browser. If not see next step.

#. Navigate to the Jupyter Notebook Server interface at **localhost:8888**
   using a browser and typing the address in the address bar.


#. You should see the **chipwhisperer** folder in your browser, the tutorials
   can be found in the **jupyter** folder. Follow the instructions there to get
   started!


Tutorials
---------

Tutorials are available as Jupyter Notebooks on 
our `chipwhisperer-jupyter <https://github.com/newaetech/chipwhisperer-jupyter>`__ Github
repository. 

Completed tutorial files, which were previously available on this page, are now stored on our
`test results Github page <https://github.com/newaetech/ChipWhisperer-Test-Results>`__ and
are available in reStructured text (which renders on Github) and html.


**************
Python Package
**************

The **chipwhisperer** software can also be used without Jupyter Notebooks if
you prefer. After you install **chipwhisperer** to the correct Python
interpreter, use **chipwhisperer** as you normally would any python package::

    import chipwhisperer as cw
    help(cw)

The :doc:`scope API <scope-api>` has all the information about what functions,
and classes are at your disposal.

