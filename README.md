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



### Flujo de Trabajo

1. **Importación de Imágenes:** Cargar las imágenes DICOM en OsiriX MD para su revisión inicial.
2. **Reconstrucción 3D:** Utilizar InVesalius para convertir las imágenes seleccionadas en un modelo 3D.
3. **Edición del Modelo:** Refinar y preparar el modelo utilizando Meshmixer, asegurando la calidad y la precisión del diseño.
4. **Preparación para Impresión:** Generar el G-Code usando Slic3r y realizar ajustes finales en la configuración de la impresora.
5. **Impresión 3D:** Producir el modelo físico utilizando la impresora 3D.

Cada paso está detalladamente descrito en los documentos adjuntos a este repositorio, con guías paso a paso para facilitar el proceso a los usuarios nuevos.

