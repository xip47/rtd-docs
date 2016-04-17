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

Para mayor información sobre los comandos se puede visitar la `documentación de sphinx`_.

.. _documentación de sphinx: http://www.sphinx-doc.org/en/stable/rest.html#rst-primer

Crear nueva página
++++++++++++++++++++++++++++++

En ``index.rst`` se puede crear la introducción del documento. Para crear una página nueva se debe crear un documento con extensión ``.rst``. Es importante que el documento contenga un Título para que la renderización tome el documento.

Para que Sphinx conozca el nuevo archivo debe ser registrado en el ``ìndex.rst`` en la sección del ``.. toctree::`` con el mismo nombre del archivo, pero sin la extensión.

.. code-block:: reStructuredText

   .. toctree::
      :maxdepth: 2
      
      nombre-archivo
      
.. note::
   
   El nombre del archivo debe ser identificado con la ruta, sin embargo la ruta es relativa al nivel donde se encuentra el archivo ``index.rst`` y ``conf.py``
