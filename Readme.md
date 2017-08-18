Hitchhiker's Guide to Ethical Hacking
=====================================

A Field manual created by students and staff on the Coventry University Ethical Hacking course.


Working On the H2GH
====================

Below is an quick overview of how to contribute to the guide. 
Further details can be found in the guide itself (how meta is that)

Getting Started
----------------

1) Fork the repository
   In Github click "Fork" (top right) 

2) Download your Forked repository 

```bash
$ git clone <url>
```

3) <optional> Create a Feature Branch

```bash
$ git branch <feature>
$ git checkout <feature>
```

Setup the working environment
------------------------------

1) Create a new virtualenv http://docs.python-guide.org/en/latest/dev/virtualenvs/

```bash
$ python3 -m venv env
```

   1a) You may need to install the python3 venv package

   ```bash
   $ sudo apt-get install python3.4-venv
   ```
   

2) Enter the virtualenv

```bash
$ source env/bin/activate
```

3) Install any dependencies

```bash
(env)$ pip install nikola
```

4) Install Nikola orgmode plugin

```bash
(env)$ nikola plugin -i orgmode



Building the Documents
-----------------------

The documents can be compiled using the makefile.
Several build options exist, but for the moment we will use HTML

```bash
(env)$ nikola build
```

The output is available in *output*

Viewing without a web browser
-------------------------------

```bash
(env)$ nikola serve
```

Visit localhost:8000


Creating Posts
==================

```bash
(env)$ nikola new_post
Creating New Post
-----------------

Title: First
Scanning posts........done!
[2017-08-17T16:16:18Z] INFO: new_post: Your post's text is at: posts/first.rst
```

or using orgmode
```bash
(env)$ nikola new_post -f orgmode
...
```


TODO
====

Currently everything is setup so we get items as blog posts.
In the future we can rationalise things as pages and keep blog posts for specific vulns.


Contributors
=============

@djgoldsmith
