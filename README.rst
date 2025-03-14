`dirty_cat`
===========


**dirty_cat has migrated** to `skrub <https://github.com/skrub-data/skrub>`__ .
**This repository will no longer be maintained.**

**Use skrub**, it has all the features of dirty-cat and more.

.. image:: https://dirty-cat.github.io/stable/_static/dirty_cat.svg
   :align: center
   :alt: dirty_cat logo

|

Do not use dirty_cat, but rather the skrub package
----------------------------------------------------

`dirty_cat <https://dirty-cat.github.io/>`_ was a Python library
to facilitate machine-learning on dirty categorical variables.

Its functionalities are merged in the `skrub <https://skrub-data.org>`_

|

Dirty categories
-------------------

For a detailed description of the problem of encoding dirty categorical data, see
`Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.


What can `dirty_cat` do?
------------------------

`dirty_cat` provides tools (``TableVectorizer``, ``fuzzy_join``...) and
encoders (``GapEncoder``, ``MinHashEncoder``...) for **morphological similarities**,
for which we usually identify three common cases: **similarities, typos and variations**

`The first example notebook <https://dirty-cat.github.io/stable/auto_examples/01_dirty_categories.html>`_
goes in-depth on how to identify and deal with dirty data using the `dirty_cat` library.

What `dirty_cat` does not
~~~~~~~~~~~~~~~~~~~~~~~~~

`Semantic similarities <https://en.wikipedia.org/wiki/Semantic_similarity>`_
are currently not supported.
For example, the similarity between *car* and *automobile* is outside the reach
of the methods implemented here.

This kind of problem is tackled by
`Natural Language Processing <https://en.wikipedia.org/wiki/Natural_language_processing>`_
methods.

`dirty_cat` can still help with handling typos and variations in this kind of setting.

Installation
------------

Please do not use dirty-cat anymore, but rather skrub, which has the same
features, replaces dirty-cat and can be easily installed via `pip`::

    pip install skrub

Dependencies
~~~~~~~~~~~~

Dependencies and minimal versions are listed in the `setup <https://github.com/dirty-cat/dirty_cat/blob/main/setup.cfg#L26>`_ file.

Related projects
----------------

`skrub <https://skrub-data.org>`_

Contributing
------------

If you want to encourage development of these functionality, the best
thing to do is to *spread the word* around `skrub <https://skrub-data.org>`_

And please contribute to `skrub <https://github.com/skrub-data/skrub>`_

Additional resources
--------------------

* `Introductory video (YouTube) <https://youtu.be/_GNaaeEI2tg>`_
* `Overview poster for EuroSciPy 2022 (Google Drive) <https://drive.google.com/file/d/1TtmJ3VjASy6rGlKe0txKacM-DdvJdIvB/view?usp=sharing>`_

References
----------

.. [1] Patricio Cerda, Gaël Varoquaux, Balázs Kégl. Similarity encoding for learning with dirty categorical variables. 2018. Machine Learning journal, Springer.
.. [2] Patricio Cerda, Gaël Varoquaux. Encoding high-cardinality string categorical variables. 2020. IEEE Transactions on Knowledge & Data Engineering.
