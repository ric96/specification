####################################################
96Boards Specifications
####################################################


Build Instructions
==================

Requirements
^^^^^^^^^^^^

* Sphinx version 1.5 or later: http://sphinx-doc.org/en/master/contents.html
* LaTeX (and pdflatex, and various LaTeX packages)

On Debian and Ubuntu
^^^^^^^^^^^^^^^^^^^^
::

  # apt-get install python3-sphinx texlive texlive-latex-extra libalgorithm-diff-perl \
                    texlive-humanities texlive-generic-recommended texlive-generic-extra \
                    latexmk

If the version of python-sphinx installed is too old, then an additional
new version can be installed with the Python package installer::

  $ apt-get install python3-pip
  $ pip3 install --user --upgrade Sphinx
  $ export SPHINXBUILD=~/.local/bin/sphinx-build

Export SPHINXBUILD (see above) if Sphinx was installed with pip3 --user, then follow Make commands below.

On Fedora
^^^^^^^^^

::

  # dnf install python3-sphinx texlive texlive-capt-of texlive-draftwatermark \
                texlive-fncychap texlive-framed texlive-needspace \
                texlive-tabulary texlive-titlesec texlive-upquote \
                texlive-wrapfig texinfo latexmk

On Mac OS X
^^^^^^^^^^^

* Install MacTeX_
* Install pip if you do not have it::

  $ sudo easy_install pip

* Install Sphinx::

  $ pip install --user --upgrade Sphinx

.. _MacTeX: http://tug.org/mactex

Make Targets
^^^^^^^^^^^^

To generate PDF::

  $ make latexpdf

To generate hierarchy of HTML pages::

  $ make html

To generate a single HTML page::

  $ make singlehtml

Output goes in `./build` subdirectory.

License
=======

This work is licensed under the Creative Commons Attribution-ShareAlike 4.0
International License (CC-BY-SA-4.0). To view a copy of this license, visit
http://creativecommons.org/licenses/by-sa/4.0/ or send a letter to
Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.

A copy of the license is included in the LICENSE_ file.

.. image:: https://i.creativecommons.org/l/by-sa/4.0/88x31.png
   :target: http://creativecommons.org/licenses/by-sa/4.0/
   :alt: Creative Commons License

.. _CONTRIBUTING.rst: ./CONTRIBUTING.rst
.. _LICENSE: ./LICENSE

Writers Guide
=============

All documentation in this repository uses reStructuredText_ markup
with Sphinx_ extensions.

All files in this project must include the relevant SPDX license identifier
tag. Generally this means each ``.rst`` file should include the line

    ``.. SPDX-License-Identifier: CC-BY-SA-4.0``

.. _reStructuredText: http://docutils.sourceforge.net/docs/user/rst/quickref.html
.. _Sphinx: http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html

.. SPDX-License-Identifier: CC-BY-SA-4.0

