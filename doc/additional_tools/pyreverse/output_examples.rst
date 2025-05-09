Example Output
##############

Example diagrams generated with the ``.puml`` output format are shown below.

Package Diagram
...............

.. image:: ../../media/pyreverse_example_packages.png
   :width: 344
   :height: 177
   :alt: Package diagram generated by pyreverse
   :align: center

Class Diagram
.............

.. image:: ../../media/pyreverse_example_classes.png
   :width: 625
   :height: 589
   :alt: Class diagram generated by pyreverse
   :align: center

Creating Class Diagrams for Specific Classes
''''''''''''''''''''''''''''''''''''''''''''

In many cases creating a single diagram depicting all classes in the project yields a rather unwieldy, giant diagram.
While limiting the input path to a single package or module can already help greatly to narrow down the scope, the ``-c`` option
provides another way to create a class diagram focusing on a single class and its collaborators.
For example, running::

  pyreverse -ASmy -c pylint.checkers.classes.ClassChecker pylint

will generate the full class and package diagrams for ``pylint``, but will additionally generate a file ``pylint.checkers.classes.ClassChecker.dot``:

.. image:: ../../media/ClassChecker_diagram.png
   :width: 757
   :height: 1452
   :alt: Package diagram generated by pyreverse
   :align: center
