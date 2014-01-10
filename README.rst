Tournesol
=========

``tournesol`` is a light web framework for developing asynchronous servers in
Python. It strives to provide functions similar to Tornado_ but uses asyncio_
for its operation. At the beginning it will not have many functions but will
grow over time. The priority is on fast startup and small footprint.

``tournesol`` is different to the older and more mature asynchronous frameworks
Twisted_ and Tornado_. It does not support older Python versions. Python ≥ 3.3
is required. That enables ``tournesol`` to support asyncio_ (introduced with
`PEP 3156`_) and the ``yield from`` syntax for coroutines (introduced with
`PEP 380`_). Using coroutines enables developers to write asynchronous code
without deferreds_ or callbacks_.

Install ``tournesol`` from PyPI_ using ``pip install tournesol``.
On Python 3.3 the `asyncio`_ module has to be installed seperately with ``pip
install asyncio``. On Python ≥ 3.4 the module asyncio_ is part of the Python
Standard Library.

Bug reports, patches and suggestions welcome!
Just open an `issue`_ or send a `pull request`_.

.. _Twisted: http://twistedmatrix.com/
.. _deferreds: http://twistedmatrix.com/documents/current/core/howto/defer.html

.. _Tornado: http://www.tornadoweb.org/
.. _callbacks: http://www.tornadoweb.org/en/stable/ioloop.html#callbacks-and-timeouts

.. _PEP 380: http://www.python.org/dev/peps/pep-0380/
.. _PEP 3156: http://www.python.org/dev/peps/pep-3156/
.. _asyncio: http://docs.python.org/3.4/library/asyncio
.. _PyPI: https://pypi.python.org/

.. _issue: https://github.com/waldhol/tournesol/issues/new
.. _pull request: https://github.com/waldhol/tournesol/compare/

Why does the world need yet another web framework?
--------------------------------------------------

Because I did not find a web framework that fits my needs.

I need integration of HTTP and proprietary TCP and UDP servers in a single event
loop so that thay can share state without an additional database connection.

Tornado_ has excellent support for HTTP but does not excel in support for
regular TCP or UDP servers.

Twisted_ is the great grandfather of asynchronous frameworks and has all the
bells and whistles one could hope for. But it does not excel in HTTP support.

And both do not support `PEP 380`_ coroutines. And asynchronous programming
without coroutines is a pain.

And last but not least there is startup time and footprint. Big function
makes big resource usage. Here at ``tournesol`` we will stay light.

Where does the funny name come from?
------------------------------------

It seems to be convention to name asynchronous frameworks after something that
turns and begins with T. Tournesol_ is french for sunflower. A sunflower turns
its head during the day to follow the sun.

.. _Tournesol: http://fr.wikipedia.org/wiki/Tournesol
