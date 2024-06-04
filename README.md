[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7317125.svg)](https://doi.org/10.5281/zenodo.7317125)

# Desvelando el Pulso de Colombia: Extracción de Datos y Análisis de Noticias con Scrapy

![map accident](https://github.com/jhontd03/eltiemposcraper/blob/master/img/daily_news.png "daily_news")

## [Contenido](#Contenido)

- [Introducción](#Introduccón)
- [Instalación](#Instalación)
- [Requisitos](#Requisitos)
- [Uso](#Uso)
- [Estructura del repositorio](#Estructura-del-repositorio)
- [Resultados](#Resultados)
- [Autor](#Autor)

## Introducción

El presente proyecto es una aplicación de la técnica de webscraping, para la obtención de noticias en el diario [El Tiempo](https://www.eltiempo.com/).

Su desarrollo se enmarca en la práctica 1 de la asignatura Tipología y ciclo de vida de datos del [Mater Universitario en Ciencia de Datos](https://estudios.uoc.edu/es/masters-universitarios/data-science/presentacion) de la Universitat Oberta de Catalunya.

## Instalación

## Requisitos

Para la ejecución del programa es necesario instalar la version de python 3.8.x y para usuarios de windows, un emulador de la terminal de comandos similar al bash de linux 

Instale [python](https://www.python.org/downloads/) y [cmder](https://cmder.app/)

## Uso

Clone el presente repositorio cree un entorno virtual, instale las librerias y ejecute el código Python directamente.

```
git clone https://github.com/jhontd03/eltiemposcraper.git
cd eltiemposcraper
python -m venv venv
venv\Scripts\activate
python -m pip install --upgrade pip
pip install scrapy
cd eltiemposcraper
scrapy crawl news
```

## Estructura del repositorio

El árbol de directorios del repositorio es el siguiente:
```
.
│   .gitignore
│   LICENSE
│   Memoria.pdf
│   README.md
│   scrapy.cfg
│   tree.txt
│   
├───dataset
│       news_eltiempo_11-11-2022.json
│       
├───eltiemposcraper
│   │   items.py
│   │   middlewares.py
│   │   pipelines.py
│   │   settings.py
│   │   __init__.py
│   │   
│   └───spiders
│           news.py
│           __init__.py
│           
└───img
        daily_news.png

```

## Resultados

Se obtuvo un archivo json que contiene 234 noticias correspondientes al 11 de noviembre de 2022, en las categorias: economía, política, justicia, unidad investigativa y opinión, cada noticia contiene el título, epígrafe y el cuerpo.

[Ver dataset obtenido](https://github.com/jhontd03/eltiemposcraper/tree/master/dataset)

## Autor

Jhon Jairo Realpe

jrealpe0@uoc.edu
