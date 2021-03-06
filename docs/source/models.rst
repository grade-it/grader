Models
======

.. py:currentmodule:: grader.models

Grader consists of several classes that represent different apsects of
the grader. Namely:

* :class:`Grader` - The whole shebang. This object has
  members that allow for all kinds of high-level assignment
  manipulation: creation, grading, etc. The grader can be configured
  with a YAML file (which is represented with a
  :class:`GraderConfig`)
* :class:`Assignment` - A single assignment
* :class:`GradeSheet` - A grade sheet for a single
  assignment. Grade sheets describe how an assignment should be
  graded, which includes:

    * Grading scripts
    * A Dockerfile for building the execution environment
    * Assignment-specific configuration (via
      :class:`AssignmentConfig`) for running and
      evaluating submitted assignments.


Grader
------

.. autoclass:: Grader
   :members:

   .. automethod:: __init__


Assignment
----------

.. autoclass:: Assignment
   :members:

   .. automethod:: __init__


GradeSheet
----------

.. autoclass:: GradeSheet
   :members:

   .. automethod:: __init__


Submission
----------

.. autoclass:: Submission
   :members:

   .. automethod:: __init__


Configuration
-------------

.. autoclass:: grader.models.config.Config
   :members:

    .. automethod:: grader.models.config.Config.__init__
    .. automethod:: grader.models.config.Config.__getitem__


.. autoclass:: GraderConfig
   :members:

.. autoclass:: AssignmentConfig
   :members:


Mixins
------

.. autoclass:: grader.models.mixins.DockerClientMixin
   :members:
