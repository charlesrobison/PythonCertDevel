.. _language_topics:

**********************
Python Language Topics
**********************

The Python Glossary:
====================

If you find yourself confused about any of terms in this document or elsewhere, the python glossary is a good place to start:

https://docs.python.org/3/glossary.html#term-parameter

Names and Values
================

Python is all about names and values. But it can get a bit confusing sometimes.

Ned Batchelder's talk: `Facts and Myths about Python names and values  <https://www.youtube.com/watch?v=_AEJHKGk9ns>`_

And a related note about mutability:
`Python Tuples are Immutable Except when they're Mutable <https://inventwithpython.com/blog/2018/02/05/python-tuples-are-immutable-except-when-theyre-mutable/>`_

Sequences and Slicing
=====================

Iterators
=========

* `What's the difference between interators and generators? <https://stackoverflow.com/questions/2776829/difference-between-pythons-generators-and-iterators>`_


Working with text
=================

String Formatting
-----------------

https://www.digitalocean.com/community/tutorials/how-to-use-string-formatters-in-python-3


Arguments and Parameters
========================

Things can get a little confusing about positional vs keyword arguments vs default parameters, etc.. And, of course the dreaded `*args` and `**kwargs`. A good place to start for definitions of terms is the glossary:

https://docs.python.org/3/glossary.html#term-parameter

and then a nice discussion of what all that means:

http://stupidpythonideas.blogspot.com/2013/08/arguments-and-parameters.html


Python Style:
=============

Of course, PEP8 (https://www.python.org/dev/peps/pep-0008/) is the place to start with coding style, but if you want to go beyond that, here's a good start:

https://github.com/amontalenti/elements-of-python-style


Comprehensions:
===============

http://treyhunner.com/2015/12/python-list-comprehensions-now-in-color/


Object Oriented Programming: classes
====================================

Magic Methods
-------------

A good reference:

http://minhhh.github.io/posts/a-guide-to-pythons-magic-methods

And with a bit more explanation:

https://www.python-course.eu/python3_magic_methods.php


``super()``
-----------

``super`` is a pretty confusing topic! Here are some good resources:

Raymond Hettinger's PyCon2015 talk: "Super Considered Super"

https://youtu.be/EiOglTERPEo

and the original blog post:

`Super Considered Super <https://rhettinger.wordpress.com/2011/05/26/super-considered-super/>`_

Which was in response to this original post:

`Super Considered Harmful <https://fuhm.net/super-harmful/>`_

Functional Programming
======================

Programming paradigms
---------------------
* https://en.wikipedia.org/wiki/Comparison_of_programming_paradigms
* https://dev.to/ericnormand/programming-paradigms-and-the-procedural-paradox

Functional programming
----------------------
Some links for you that may help with the concepts (in no particular order):
* https://maryrosecook.com/blog/post/a-practical-introduction-to-functional-programming
* https://www.dataquest.io/blog/introduction-functional-programming-python/
* https://www.vinta.com.br/blog/2015/functional-programming-python/
* https://marcobonzanini.com/2015/06/08/functional-programming-in-python/
* https://github.com/sfermigier/awesome-functional-python

Concurrency
===========

Concurrency is a pretty big topic, but here are few good ones:

General introduction to the concept with examples of both threads and processes:

`Intro to Threads and Processes in Python <https://medium.com/@bfortuner/python-multithreading-vs-multiprocessing-73072ce5600b>`_.

Threading
---------

Threading and GUI programming:

https://www.blog.pythonlibrary.org/2013/06/27/wxpython-how-to-communicate-with-your-gui-via-sockets/

Understanding the GLobal Interpreter Lock:

`Groc the GIL: <https://opensource.com/article/17/4/grok-gil>`_

Asynchronous Programming
------------------------

Recent versions of Python have added support for asynchronous programming. It is a whole new way to deal with program flow.

Here are some resources to help you "get" it:

Asynchronous Python -- Await the Future

https://hackernoon.com/asynchronous-python-45df84b82434#.kpwejkin2

Async Through the Looking Glass -- Adventures in Python Land

https://hackernoon.com/async-through-the-looking-glass-d69a0a88b661#.sd3xk0ru0

How the heck does ``asyc-await`` Work in Python?

https://snarky.ca/how-the-heck-does-async-await-work-in-python-3-5/

Nicholas Tollervey `Lessons Learned with asyncio <https://speakerdeck.com/pycon2015/nicholas-tollervey-lessons-learned-with-asyncio-look-ma-i-wrote-a-distributed-hash-table>`_


Asyncio for the working Python developer
----------------------------------------
This one talks about why you might want to do async development.

https://hackernoon.com/asyncio-for-the-working-python-developer-5c468e6e2e8e#.dlhcuy23h

Assorted from David Beazley
---------------------------

David Beazley is scary smart, and types much faster than most of us can think. But on video, you can pause and take the take to catch up with him, and learn a lot:

http://www.dabeaz.com/talks.html

This one in particular -- ALL live demo. Really hard to keep up -- but really informative!

Python Concurrency From the Ground Up: LIVE!

http://pyvideo.org/pycon-us-2015/python-concurrency-from-the-ground-up-live.html


Logging
-------

`A guide to logging in Python <https://opensource.com/article/17/9/python-logging>`_

Corners of Python
=================

This is a nice collection of little bits of Python that may be surprising:

`WTF Python? <https://github.com/satwikkansal/wtfpython>`_

Metaprogramming
===============

Metaprogramming is writing programs that write programs... it is a large topic, starting with fairly simple things like the use of ``getattr`` or ``setattr``, through decorators, and all the way up to metaclasses.

This lecture by David Beazley is a great overview:

https://youtu.be/sPiWg5jSoZI

decorators
----------

Decorators are a way to "wrap" functions to alter their behavior one way or another. THere are lot of resources out there about them, but here's some stuff from a guy that really wants to get it right:

The ``wrapt`` package that does a lot for you:

https://github.com/GrahamDumpleton/wrapt

And the author's blog posts about it all:

https://github.com/GrahamDumpleton/wrapt/tree/develop/blog


Command Line Scripting
======================

Python is a great tool for making command line programs. As soon as a command line program gets a bit beyond the basics, you need to provide an interface that allows users to set options, etc.

The built-in ``argparse`` module does a lot for you, and is a while lot better than writing a bunch of custom code, but there are a couple of third party packages that make it even easier -- these are well worth checking out:

``docopt``
----------

"Create *beautiful* command-line interfaces with Python"

``docopt`` lets you write the docs for your interface, and it automatically builds the code to implement it -- very cool.

http://docopt.org/


``click``
---------

  Click is a Python package for creating beautiful command line interfaces in a composable way with as little code as necessary. It’s the “Command Line Interface Creation Kit”. It’s highly configurable but comes with sensible defaults out of the box.

http://click.pocoo.org/

