# README

## Descripcion del proyecto

Este repositorio contiene un cuaderno Jupyter Notebook desarrollado para resolver el ejercicio de la Sesion 02 de la asignatura Bioinformatica en laboratorio. El objetivo principal es trabajar con ficheros FASTA utilizando la libreria Biopython para realizar operaciones basicas de analisis de secuencias.

El cuaderno permite:
- Leer un archivo FASTA con secuencias de ADN.
- Calcular el porcentaje de contenido GC para cada secuencia.
- Traducir cada secuencia de ADN a su correspondiente secuencia de aminoacidos.
- Guardar las secuencias proteicas generadas en un nuevo archivo FASTA.

## Requisitos

Para ejecutar correctamente este proyecto se necesita:

- Python 3.x instalado
- Libreria Biopython  
  Instalacion:  
  pip install biopython
- Jupyter Notebook, JupyterLab o VS Code con soporte para cuadernos
- Archivo de entrada gene.fna ubicado en el mismo directorio que el cuaderno

## Estructura del proyecto

El proyecto incluye:

- ejercicio_sesion02_biopython.ipynb  
  Cuaderno que contiene todo el flujo de trabajo solicitado.
- gene.fna  
  Archivo FASTA de entrada con las secuencias de ADN.
- proteinas_traducidas.fasta  
  Archivo generado automaticamente que contiene las secuencias de aminoacidos obtenidas mediante traduccion.

## Metodologia utilizada

El cuaderno implementa el siguiente procedimiento:

1. Importacion de Biopython y creacion de una funcion personalizada para calcular el contenido de GC.
2. Lectura del archivo FASTA utilizando SeqIO.parse de Biopython.
3. Calculo del contenido GC para cada secuencia del archivo y visualizacion del resultado.
4. Traduccion de cada secuencia de ADN a proteinas utilizando translate(to_stop=True).
5. Generacion de nuevos SeqRecord para almacenar las secuencias proteicas obtenidas.
6. Escritura del archivo de salida proteinas_traducidas.fasta manteniendo los identificadores y descripciones originales.
7. Automatizacion completa del proceso dentro del cuaderno Jupyter.

## Autores

Adrian Ojeda  
Raul Mendoza  

Estudiantes de la Universidad de Las Palmas de Gran Canaria (ULPGC)  
Asignatura: Bioinformatica
