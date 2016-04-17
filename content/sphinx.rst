=============================
Sphinx
=============================

Estructura
-----------------------------

Crear carpeta de documentación en el nivel del proyecto

.. code-block:: bash

   $ mkdir docs
   $ cd docs
   
Ejecutar el quickstart de sphinx para construir la estructura de directorios y el archivo de configuración

.. code-block:: bash

   $ sphinx-quickstart
   
Iniciará una serie de preguntas. Mantener en default las mayoria de las opciones, pues lo importante son:

* Project name
* Source file suffix
* Version
* Makefile
* Windows bat
   
Template
-----------------------------

En archivo ``conf.py`` editar y cambiar

.. code-block:: python

   html_theme = 'alabaster'
   
por

.. code-block:: python

   html_theme = 'sphinx_rtd_theme'
   
Renderizado
-----------------------------

Se ejecuta el comando:

.. code-block:: bash

   $ make html

Comandos
-----------------------------


Elementos reStructuredText
++++++++++++++++++++++++++++++


Crear nueva página
++++++++++++++++++++++++++++++


