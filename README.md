# DICOM a Impresión 3D

**Autor:** Javier Díaz Valderrama  
**Contacto:** [jadiazvalderrama@gmail.com](mailto:jadiazvalderrama@gmail.com)

## Descripción del Repositorio

Este repositorio presenta un flujo de trabajo simplificado para convertir imágenes médicas en formato DICOM, obtenidas mediante tomografía computarizada (CT), en representaciones físicas impresas en 3D. El objetivo principal es facilitar la creación de modelos para estudios académicos y la planificación quirúrgica.

## Objetivos

- **Educación:** Proporcionar a estudiantes y profesionales una herramienta para estudiar anatomía y patologías de manera tangible.
- **Planificación Quirúrgica:** Ayudar en la preparación y planificación de procedimientos quirúrgicos, permitiendo a los cirujanos explorar y planear intervenciones con modelos físicos.

## ¿Cómo empezar?

Para comenzar a utilizar este workflow, sigue los pasos detallados en la sección de [Documentación](#documentación) donde encontrarás instrucciones paso a paso para convertir tus archivos DICOM a modelos 3D listos para imprimir.

## Documentación

En esta sección encontrarás toda la información necesaria para entender y ejecutar el proceso de transformación de imágenes DICOM a modelos 3D. Se abarcan desde los conceptos básicos hasta detalles técnicos específicos del flujo de trabajo.

### Alcances

Este proyecto está diseñado para ser utilizado en contextos académicos y de planificación quirúrgica. Los modelos 3D generados pueden servir como herramientas educativas para estudiantes del area d la salud y como apoyo en la visualización y planificación de intervenciones quirúrgicas. No se recomienda el uso de estos modelos para procedimientos diagnósticos o terapéuticos sin la validación adecuada por profesionales certificados.

### Definiciones

- **DICOM:** Digital Imaging and Communications in Medicine, un estándar internacional para el almacenamiento y transmisión de información médica radiológica.
- **CT:** Tomografía Computarizada, técnica de imagen que utiliza procesamiento computarizado para generar representaciones seccionales de áreas corporales a través de rayos X. Ideal para representacion de secciones anatomicas oseas.
- **Malla 3D**: Serie de poligonos unidos que representan una estructura tri dimensional.
- **Modelo 3D:** Representación tridimensional de una estructura anatómica, creada a partir de imágenes médicas y destinada a la impresión 3D.

### Programas Utilizados

En este proyecto, se han seleccionado dos herramientas principales que funcionan en la plataforma Windows 11 para simplificar el flujo de trabajo y maximizar la eficiencia en la conversión de imágenes DICOM a modelos 3D imprimibles. A continuación se detallan los programas utilizados:

- **[Radiant](https://www.radiantviewer.com/es/):** Este software se especializa en la visualización y manejo de imágenes en formato DICOM. Su interfaz intuitiva y su robusto conjunto de herramientas permiten una óptima revisión y manipulación de datos radiológicos.
- **[Meshmixer](https://meshmixer.com/download.html):** Es una herramienta avanzada para editar y preparar modelos 3D para la impresión. Proporciona funcionalidades para modificar, optimizar y reparar modelos 3D, asegurando que estén listos para una impresión de alta calidad.

Aunque en este proyecto se optó por Radiant y Meshmixer debido a su compatibilidad y facilidad de uso, existen varias alternativas para la visualización de DICOMs y la segmentación 3D. Entre estas se incluyen:

- **[OsiriX MD](https://www.osirix-viewer.com/osirix/osirix-md/):** Ampliamente reconocido por su poderoso motor de renderizado 3D y su uso en entornos clínicos.
- **[3D Slicer](https://download.slicer.org/):** Software libre que ofrece herramientas avanzadas para la análisis y visualización de imágenes médicas.
- **[ITK-SNAP](http://www.itksnap.org/pmwiki/pmwiki.php?n=Downloads.SNAP4):** Frecuentemente utilizado para la segmentación semiautomática de estructuras anatómicas en imágenes médicas.
- **[InVesalius](https://invesalius.github.io/download.html):** Desarrollado por el gobierno brasileño, se destaca por su accesibilidad y herramientas específicas para la creación de modelos 3D a partir de imágenes médicas.

Cada uno de estos programas ofrece diferentes ventajas y desventajas, y la elección dependerá de las necesidades específicas del proyecto y las preferencias del usuario.

- ### Bases de Datos DICOM

Para la creación de modelos 3D de regiones anatómicas a partir de imágenes médicas, es esencial comenzar con la adquisición de datos DICOM de Tomografía Computarizada (CT). A continuación, se listan algunas bases de datos confiables y accesibles que ofrecen imágenes DICOM gratuitas para fines académicos y de investigación:

- **[The Cancer Imaging Archive (TCIA)](https://www.cancerimagingarchive.net/):** Un recurso vasto que proporciona acceso a una gran cantidad de imágenes médicas de dominio público, incluidas imágenes de CT utilizadas en estudios de investigación del cáncer.
- **[DICOM Library](https://www.dicomlibrary.com/):** Permite subir, compartir y visualizar tus propias imágenes DICOM, así como descargar imágenes de casos anónimos proporcionados por otros usuarios.
- **[OpenNeuro](https://openneuro.org/):** Plataforma dedicada a la libre distribución de datos de neuroimágenes, incluyendo algunos conjuntos de datos en formato DICOM.
- **[National Biomedical Imaging Archive (NBIA)](https://imaging.nci.nih.gov/nbia/):** Repositorio mantenido por el National Cancer Institute que ofrece imágenes y datos relacionados para fomentar la investigación biomédica.
- **[Visible Human Project CT Datasets](https://central.xnat.org/app/template/XDATScreen_report_xnat_projectData.vm/search_element/xnat:projectData/search_field/xnat:projectData.ID/search_value/HumanCT):** Parte del renombrado Visible Human Project, este recurso incluye conjuntos de datos completos de CT, permitiendo exploraciones detalladas del cuerpo humano en diferentes estados y configuraciones.

Estas bases de datos son útiles tanto para profesionales que buscan mejorar sus habilidades en la manipulación y análisis de imágenes médicas como para investigadores en busca de datos para estudios más extensos.

### Datos Específicos Utilizados en el Proyecto

![Pelvis Model Visualized in Radiant](/Imagenes/0_Pelvis_Radiant.png)

Para el desarrollo de este proyecto, se utilizó específicamente el conjunto de datos de la **pelvis de un hombre** del Visible Human Project. Este conjunto de datos ha sido clave para el modelado detallado de la anatomía pélvica en 3D. 

El conjunto de datos específico empleado está disponible para consulta y uso mediante el siguiente enlace: [Visible Human Project - Pelvis Male](https://central.xnat.org/app/action/DisplayItemAction/search_element/xnat%3ActSessionData/search_field/xnat%3ActSessionData.ID/search_value/CENTRAL04_E04390/popup/false/project/HumanCT).


Este recurso fue seleccionado por su calidad y detalle, proporcionando una base sólida y precisa para la creación de modelos anatómicos 3D. El uso de estos datos específicos facilita la exploración y comprensión de las complejidades anatómicas de la región pélvica, lo que es crucial para aplicaciones académicas y de planificación quirúrgica.



### Flujo de Trabajo

1. **Importación de Imágenes:** Cargar las imágenes DICOM en RADIANT para su revisión inicial.
![Inicio Radiant](/Imagenes/1_inicio_Radiant.png)
![Importar Radiant](/Imagenes/2_importar_Radiant.png)
![Importar 2 Radiant](/Imagenes/3_importar2_Radiant.png)
![Inicio Radiant](/Imagenes/4_CT_Image_Radiant.png)

2. **Reconstrucción 3D:** Utiliza la herramienta **3D Volume rendering**, que se encuentra en la barra de herramientas superior de Radiant, para convertir las imágenes seleccionadas en un modelo 3D. Dentro de esta función, encontrarás una opción llamada **3D Presets**, la cual te permite segmentar diferentes tipos de tejidos mediante filtros preestablecidos. Para nuestros propósitos, seleccionaremos el filtro para hueso **Bones B/W**.
![Visión 3D en Radiant](/Imagenes/5_Vision3D_Radiant.png)
![Filtros en Radiant](/Imagenes/6_Filtros_Radiant.png)

Para una segmentación más precisa y "manual" de tejidos, puedes manipular la vista del modelo 3D usando el ratón: mantén presionado el botón del scroll y mueve el ratón hacia arriba, abajo, izquierda o derecha para ajustar la visualización del modelo según sea necesario. Esta funcionalidad es especialmente útil para explorar y afinar detalles específicos del modelo anatómico.

3. **Edición del Modelo en RADIANT:** Refinar y preparar el modelo utilizando la herramienta de **Scapel** con la letra **S**, asegurando el reorte de las areas requeridas.
![Recorte Radiant](/Imagenes/7_Recorte3D_Radiant.png)

4. **Exportar modelo STL:** Posterio a la edicion dl modelo dentro de Radnaint, debemos exportar nuestro modelo con la herramienta ubicada en la esquina superior izquierda **Save 3D model as STL**, seleccionando la opcion **Full** para que la resolucion tenga la mayor calidad posible.
![Guardar STL](/Imagenes/8_GuardarSTL_Radiant.png)
![Guardar STL2](/Imagenes/9_GuardarSTL2_Radiant.png)    

5. **Edicion en Meshmixer:** Generar el G-Code usando Slic3r y realizar ajustes finales en la configuración de la impresora.
7. **Impresión 3D:** Producir el modelo físico utilizando la impresora 3D.

