# Signu

Signu es una aplicación para la firma digital múltiple de documentos PDF con o sin una marca visible.

La firma digital es tan valida como la firma manuscrita por lo que tiene las mismas consecuencias legales.

## Resumen

El objetivo de este proyecto es el desarrollo de una aplicación Android para facilitar el proceso de la realización de firmas digitales en documentos PDF, estas firmas digitales son tan validas como las firmas manuscirtas por lo que tienen las mismas consecuencias legales. Signu permite la firma múltiple de documentos PDF con un sello visible en el mismo documento si así se desea, tambien permite la firma de numeorosos documentos PDF de forma automatica. Esta aplicación contiene herramientas para gestionar claves privadas de manera segura dentro del dispositivo Android y mecanismos para crear certificados autofirmados. Debido a que las firmas digitales necesitan de una autoridad de sellado de tiempo (TSA) para dar validez a la marca de tiempo que se incluye en los documentos PDF, este trabajo incluye el desarrollo de un servicio web que nos proporciona los mecanismos para crear y comprobar estas marcas de tiempo. Así pues, a través de un desarrollo incremental guiado por pequeñas iteraciones, y dirigido por pruebas (inspirado en la conocida aproximación TDD - Testing Driven Development) se ha ido construyendo un sistema capaz de firmar documentos PDF de manera digital que puedes llevar en tu propio bolsillo.


## Pila del producto

### Obligatorio

- CRUD certificados autofirmados
- Importar y exportar certificados
- CRUD claves privadas de forma segura
- Guardar claves privadas de forma segura en la memoria interna del dispositivo
- Importar y exportar claves privadas de forma segura
- Firma digital multiple de un pdf
- Firma digital de un pdf con marca visible
- Crear X interfaces de firma para permitir la firma digital multiple de un documento pdf con marca visible
- Firmar interfaz de firma dejando una marca visible
- Importar y exportar PDFs
- Comprobar las firmas digitales de un PDF (información e integridad de las firmas)
- Cambiar de lenguaje (inglés y español)

### Deseable

- Firmar varios PDFs de manera automática
- Login para entrar en la aplicación
- Uso de huella digital para entrar en la aplicación
- Crear un servidor de tiempo (TSA - Autortidad de sellado de tiempo) haciendo uso del Network Time Protocol para incrustar marcas de tiempo validables en los documentos PDF firmados
- Firmar PDFs usando DNIe mediante OTG
- Generar e integrar códigos de barras a partir de un código alfanumérico
- Mostrar publicidad
- Publicar aplicación en el Play Store


Nota 1: la marca visible será personalizable, pudiendo añadir una imagen (jpg, png, ...), una marca de tiempo y/o autor de la firma.

Nota 2: El uso de interfaces de firma solo se usa para la firma multiple de PDFs con marca visible (util si se quiere imprimir el PDF)


## Objetivos y problemas abordados

El objetivo de este trabajo fin de grado es implementar una aplicación Android que permita la firma multiple de documentos PDF y el guardado seguro de claves privadas.

## Metodología (enfoque y herramientas)

- Desarrollo continuo incremental (similar al usado en Metodologias Ágiles)
- TDD (Test Driven Development)
- Android Studio
- SDK de Android
- VirtualBox/ GenyMotion
- Lenguaje Java y sus librerias estandar
- Libreria Java itext5

## Cronograma (fases del trabajo a realizar)

## Recursos e instalaciones necesarias

- Un alumno
- Un computador con Android Studio, VirtualBox, SDK de Android y conexión a internet

## Plazos y costes

- El plazo de finalización de ese proyecto es del 19 a 23 de Junio
- El proyecto debe poderse realizar por un alumno durante un plazo de 1 mes a razon de 40 horas semanales de trabajo
- Los recursos inicialmente comprometidos para este proyecto son un alumno durante 350 horas y un director durante 35 horas

## Implicados

- Javier Fabra Caro como Director
- Marcos Ruiz Garcia como Autor

## Riesgos del proyecto

- Tiempo de desarrollo justo para la realización del proyecto, lo que puede dar como resultado que no se cumpla el plazo
- Problemas de incompatibilidad entre un TSA y la libreria de manejo de PDFs itext5
- Problemas de incompatibilidad con lectores de DNIe y Android
- El proyecto puede no ser lo suficientemente grande para considerarse un TFG
