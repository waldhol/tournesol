Tournesol
=========

``tournesol`` is a very light web framework for developing servers in Python.
It integrates HTTP with `asyncio`_ and provides an API similar to Tornado_.

Built on top on Python's asynchronous I/O support introduced in `PEP 3156`_,
it provides an API based on coroutines, making it easy to write highly
concurrent applications.

Installation is as simple as ``pip install tournesol``. It requires Python ≥
3.4 or Python 3.3 with the `asyncio`_ module, which is available with ``pip
install asyncio``.

Bug reports, patches and suggestions welcome! Just open an `issue`_ or send a
`pull request`_.

.. _Tornado: https://github.com/aaugustin/websockets/blob/master/compliance/README.rst
.. _PEP 3156: http://www.python.org/dev/peps/pep-3156/
.. _asyncio: http://docs.python.org/3.4/library/asyncio
.. _issue: https://github.com/aaugustin/websockets/issues/new
.. _pull request: https://github.com/aaugustin/websockets/compare/
