
# Análisis metagenómico de suelos del desierto de Atacama con QIIME 2

Este repositorio contiene el flujo de trabajo y los resultados principales del análisis de comunidades microbianas de suelos del desierto de Atacama basado en secuenciación del gen 16S rRNA y procesado con **QIIME 2**. Las lecturas crudas y el archivo de metadatos puede obtenerse desde: https://docs.qiime2.org/2024.10/tutorials/atacama-soils/

## Metodología general

El análisis incluyó los siguientes pasos:

* Importación y demultiplexado de lecturas pareadas.
* Filtrado y control de calidad de secuencias.
* Generación de tabla de OTUs y árbol filogenético.
* Rarefacción y análisis de diversidad alfa y beta.
* Evaluación de diferencias entre grupos mediante pruebas estadísticas.
* Análisis de abundancia diferencial con **ANCOM**.
* Comparación taxonómica de OTUs representativos mediante BLAST.

## Contenido del repositorio

```
Atacama_QIIME2/
│
├── README.md
├── qiime2_pipeline.txt
│
├── metadata/
│   └── sample-metadata.tsv
│
├── qiime_outputs/
│   ├── table.qza
│   ├── table.qzv
│   ├── rooted-tree.qza
│   └── core-metrics-results/
│
└── figures/
    ├── rarefaction_curve.png
    ├── pcoa_plot.png
    ├── faith_boxplot.png
    └── volcano_plot.png
```

### Archivos clave

* **qiime2_pipeline.txt** → contiene todos los comandos Bash utilizados en QIIME 2.
* **qiime_outputs/** → artefactos relevantes generados por QIIME 2.
* **figures/** → gráficas y visualizaciones resultados del análisis.

