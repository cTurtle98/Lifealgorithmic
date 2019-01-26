==================
Account Access FAQ
==================

.. contents:: Questions
   :local:

What's My username and password?
--------------------------------

Your username and password are a combination of your name and your student ID.

======== ============================================================================
Code     Meaning
======== ============================================================================
``fff``  The first three letters of your first name. (lower case).
``lll``  The first three letter of your last name. (lower case)
``Ff``   The first two letters of your first name. (uppercase, lowercase)
``Ll``   The first two letters of your last name. (uppercase, lowercase)
``nnnn`` The last four digits of your student ID
``ccc``  The course number. (e.g. cis-191ab becomes ``191``, cis-15 becomes ``15``)
======== ============================================================================

The formula is:

:Username: ``lllfffccc``
:Password: ``FfLlnnnn``

Here's an example:

:Name: ``Michael Matera``
:Student ID: ``1234567``
:Class: ``CIS-191AB``
:Username: ``matmic191``
:Password: ``MiMa4567``

Your username and password are used for:

* `VMware vSphere Server <https://vcentre.cis.cabrillo.edu/ui/>`_
* `Cloud9 IDE <https://957903271915.signin.aws.amazon.com/console>`_
* `NetLab+ Server <https://openlab.bayict.cabrillo.edu/>`_ (Username only)
* Opus
  
How do I access Opus?
---------------------

You access opus using the SSH protocol. SSH allows you to run commands on the Linux command line as well as transfer files back and forth. 

How do I get a command line on Opus?
------------------------------------

On Mac and Linux you can use any UNIX shell in the Terminal. On Windows use PowerShell.

``$ ssh -p 2220 <your-user-name>@opus.cis.cabrillo.edu``

  **Note:** On Windows use PowerShell

How do I move files to/from Opus?
---------------------------------

SSH to the rescue! On all platforms you can use the scp program from the command line. The general form of the command is:

``scp <source> <destination>``

This example copies a file to your home directory on Opus from the local machine:

``$ scp -P 2220 myfile.txt <your-user-name>@opus.cis.cabrillo.edu:``

This example does the reverse:

``$ scp -P 2220 <your-user-name>@opus.cis.cabrillo.edu:myfile.txt .``

Linux users can do drag-and-drop copies by putting an SSH URL into Nautilus like this one:

``ssh://username@opus.cis.cabrillo.edu:2220/home/username``

`Filezilla <https://filezilla-project.org/>`_ does drag-and-drop for Windows. `Cyberduck  <https://cyberduck.io/>`_ does drag-and-drop for Mac.

How do I access VLab?
----------------------------------

Follow this link:

* https://vcentre.cis.cabrillo.edu/ui/

We used a self-singed certificate so it's safe to ignore the security warning. 
 
How do I access Netlab+?
------------------------

Follow this link:

* https://openlab.bayict.cabrillo.edu/

What's my Netlab+ username and password?
----------------------------------------

Your username will be the same as the one in the first answer. You will have an initial password of `Cabri11o`, which you will have to change when you first log in. 

How do I access Cloud9 IDE?
---------------------------

Follow this link:

* https://957903271915.signin.aws.amazon.com/console

When is my homework due?
------------------------

Due dates are in Canvas.

How do I access Canvas?
-----------------------

Canvas is located at:

* https://cabrillo.instructure.com/login/ldap
