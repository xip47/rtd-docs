=============================
Publicación en Read The Docs
=============================

Git
-----------------------------

Ingresar al directorio de documentación creado por Sphinx para inicializar el repositorio git.

.. code-block:: bash

   $ git init

Git Ignore
+++++++++++++++++++++++++++++

Incorporar al archivo ``.gitignore`` 

.. code-block:: bash

   _build
   _static
   _templates
   *~
   
Subir Proyecto a Repositorio
+++++++++++++++++++++++++++++

.. code-block:: bash

   echo "# Docs" >> README.md
   git add .
   git commit -m "Primer commit de documentación"
   git remote add origin git@github.com:<usuario>/<nombre-repo>.git
   git push -u origin master

Habilitar Servicio Read The Docs en github
+++++++++++++++++++++++++++++++++++++++++++

Se debe habilitar el acceso de Read The Docs a github:

#. Ir a las configuraciones del repositorio en la pestaña **settings**.
#. Abrir las opciones de **Webhoks & Services**.
#. Buscar en **Add service** ``Read The Docs`` para habilitar el acceso.

Read The Docs
-----------------------------

Ingresar con la cuenta de Read The Docs

Conectar con github y Publicar
+++++++++++++++++++++++++++++++++++++++++++

En cuenta ir a **My Projects** e importar proyecto, seleccionar el tipo de repositorio y sincronizar la cuenta.

Luego seleccionar el proyecto para iniciar la publicación de la documentación. Se realizará la instalación y posterior compilación hasta quedar completamente activo.
