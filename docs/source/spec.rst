Specification
=============

This specification is for configuring a mythical device. It does magically
things when defined in a configuration file which meets this specification.

The specification is as follows:

.. code-block:: json

   {
     "comm": {
       "param1": "<int>",
       "param1enabled": "<bool>"
     },
     "updates": {
       "release": "string",
       "version": "string"
     }
   }

comm Object
***********

The ``comm`` object defines how this mythical device communications. The
following table describes the parameters for this object block:

.. list-table:: comm Object
   :widths: 25 25 50
   :header-rows: 1

   * - Parameter
     - Type
     - Description
   * - **param1**
     - Integer
     - This parameter configures the ``param1`` interface on the mythical
       device
   * - **param1enabled**
     - Boolean
     - This tells the mythical device if the ``param1`` interface is enabled.

updates Object
**************

The ``updates`` object defines which updates a mythical device receives. The
options which can be configured are:

.. list-table:: updates Object
   :widths: 25 25 50
   :header-rows: 1

   * - Parameter
     - Type
     - Description
   * - **release**
     - string
     - This is the release channel to subscribe to for releases.
   * - **version**
     - string
     - The specific version which should be used.

