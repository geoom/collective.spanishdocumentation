.. -*- coding: utf-8 -*-

.. _glosario:

========
Glosario
========

A continuación una serie de terminos usados en las tecnologías Python / Zope / Plone

.. glossary ::
    :sorted:
    
    Cheese shop
        Ver :term:`PyPI`.
    
    Collective
        Es un repositorio de código comunitario, para Productos Plone y productos
        de terceros, y es un sitio muy útil para buscar la ultima versión de código
        fuente del producto para cientos de productos de terceros a Plone. Los
        desarrolladores de nuevos productos de Plone son animados a compartir su
        código a través de Collective para que otros puedan encontrarlo, usarlo, y
        contribuir con correcciones / mejoras. 
        
        En la actualidad la comunidad ofrece dos repositorio Collective un basado 
        en **Git** y otro **Subversion**.
        
        Si usted quiere publicar un nuevo producto en el repositorio *Git de Collective* 
        de Plone necesita `obtener acceso de escritura`_ y `seguir las reglas en github/collective`_, 
        también puede consultarlo en la cuenta en `github.com`_.
        
        Si usted quiere publicar un nuevo producto en el repositorio *Subversion de 
        Collective* de Plone necesita `obtener acceso de escritura al repositorio`_ 
        y `crear su estructura básica de repositorio`_ para su producto, también 
        puede consultarlo vía Web consulte el siguiente `enlace`_.
    
    Egg
        Ver :term:`paquetes Egg`.

    PYTHONPATH
        Una lista de nombre de directorios, que contiene librerías Python, con la misma 
        sintaxis como la variable ``PATH`` del shell de su sistema.
    
    Python Package Index
        Ver :term:`PyPI`.
    
    PyPI
        Del Ingles Python Package Index, es el servidor central de :term:`paquetes Egg` Python 
        ubicado en la dirección http://pypi.python.org/pypi/.
    
    buildout
        En la herramienta buildout, es un conjunto de partes que describe como ensamblar 
        una aplicación.
    
    part
        En la herramienta buildout, es un conjunto opciones que le permite a usted 
        construir una pieza de la aplicación.
    
    recipe
        En la herramienta buildout, es el software usado para crear una parte basada 
        en sus opciones.
    
    Paquete Python
    Paquetes Python
        Es un termino generalmente usando para describir un módulo Python. en el
        más básico nivel, un paquete es un directorio que contiene un archivo
        ``__init__.py`` y algún código Python.

    Productos
        Es una terminología usada por la comunidad Zope / Plone asociada a
        cualquier implementación de módulos / complementos y agregados que amplíen la
        funcionalidad por defecto que ofrece Zope/Plone. También son conocidos como
        *"Productos de terceros"* del Ingles `Third-Party Products`_.

    Producto Plone
        Es un tipo especial de paquete Zope usado para extender las funcionalidades
        de Plone. Se puede decir que son productos que su ámbito de uso es solo en el
        desde la interfaz gráfica de Plone.

    Productos Zope
    Producto Zope
        Es un tipo especial de paquete Python usado para extender Zope. En las
        antiguas versiones de Zope, todos los productos eran carpetas que se ubican
        dentro de una carpeta especial llamada ``Products`` de una instancia Zope;
        estos tendrían un nombre de módulo Python que empiezan por "**Products.**".
        Por ejemplo, el núcleo de Plone es un producto llamado CMFPlone, conocido en
        Python como `Products.CMFPlone`_.

        Este tipo de productos esta disponibles desde la interfaz administrativa de
        Zope (ZMI) de `su instalación`_ donde deben acceder con las credenciales del
        usuario Administrador de Zope. Muchas veces el producto simplemente no hay
        que instalarlo por que se agregar automáticamente.

    paquete Egg
    paquetes Egg
        Es una forma de empaquetar y distribuir paquetes Python. Cada Egg contiene
        un archivo ``setup.py`` con metadata (como el nombre del autor y la correo
        electrónico y información sobre el licenciamiento), como las dependencias del
        paquete. La herramienta del ``setuptools``, es la librería Python que permite
        usar el mecanismo de paquetes egg, esta es capaz de encontrar y descargar
        automáticamente las dependencias de los paquetes Egg que se instale. Incluso
        es posible que dos paquetes Egg diferentes necesiten utilizar simultáneamente
        diferentes versiones de la misma dependencia. El formato de paquetes Eggs
        también soportan una función llamada ``entry points``, una especie de
        mecanismo genérico de plug-in. Mucha más detalle sobre este tema se encuentra
        disponible en el `sitio web de PEAK`_.
        
    Temas / Apariencias
        Por lo general si un producto de Tema esta bien diseñado y implementado
        debe aplicarse de una ves al momento de instalarlo. En caso que no se aplique
        de una puede acceder a la sección `Configuración de Temas`_ y cambiar el
        **Tema predeterminado** por el de su gusto.

    Tipos de contenidos
        Los tipos de contenidos son productos que extienden la funcionalidad de
        **Agregar elemento** que permite agregar nuevos tipos de registros
        (Contenidos) a tu sitio. Esto quiere decir que si instala un tipo de
        contenido exitosamente debería poder acceder a usarlo desde el menú de
        **Agregar elemento** en el sitio Plone. Opcionalmente algunos productos
        instalan un panel de control del producto que puede acceder a este en la
        sección `Configuración de Productos Adicionales`_.
    
    Instalación de Zope
        El software propio del servidor de aplicaciones.
    
    Instancia de Zope
        Un directorio específico que contiene una configuración completa del 
        servidor Zope.
     
    ZCML-slug
        Los así llamados "ZCML-slugs", era configuraciones que estaban destinados 
        a enlazar dentro de un directorio una configuración especial en una 
        instalación de Zope, por lo general se ven como ``collective.foo-configure.zcml``. 
        Estas configuraciones ya no están más en uso, pueden ser eliminados agregando 
        las configuraciones del paquete `z3c.autoinclude`_.
         
.. _Third-Party Products: http://plone.org/documentation/kb/add-ons/tutorial-all-pages
.. _Products.CMFPlone: http://pypi.python.org/pypi/Products.CMFPlone
.. _sitio web de PEAK: http://peak.telecommunity.com/DevCenter/setuptools
.. _obtener acceso de escritura al repositorio: http://plone.org/countries/conosur/documentacion/obtener-acceso-de-escritura-al-repositorio-svn-de-plone
.. _crear su estructura básica de repositorio: http://plone.org/countries/conosur/documentacion/crear-un-nuevo-proyecto-en-el-repositorio-collective-de-plone
.. _enlace: http://svn.plone.org/svn/collective/
.. _obtener acceso de escritura: http://collective.github.com/#how-to-get-access
.. _seguir las reglas en github/collective: http://collective.github.com/#rules-on-github-collective
.. _github.com: http://github.com/collective
.. _Configuración de Temas: http://localhost:8080/Plone/@@skins-controlpanel
.. _Configuración de Productos Adicionales: http://localhost:8080/Plone/prefs_install_products_form
.. _su instalación: http://localhost:8080/manage
.. _z3c.autoinclude: http://pypi.python.org/pypi/z3c.autoinclude
