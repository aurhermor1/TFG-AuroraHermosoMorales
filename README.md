Este repositorio contiene los experimentos desarrollados del Trabajo Fin de Grado titulado:

**“Técnicas de Machine Learning y Deep Learning para anotación de células en datos de single-cell RNA-seq”**

El objetivo principal del trabajo consiste en estudiar y evaluar distintos modelos de aprendizaje automático aplicados al problema de la anotación automática de tipos celulares a partir de datos de secuenciación de ARN de célula única (scRNA-seq).

Los experimentos incluyen técnicas clásicas de Machine Learning, modelos basados en Deep Learning y distintas estrategias de procesamiento y análisis de datos transcriptómicos de célula única.






---
El trabajo consta de dos experimentos:

# Experimento 1 — Mouse Cell Atlas (MCA)

El primer experimento se centra en la evaluación de distintos modelos de clasificación celular utilizando datos del Mouse Cell Atlas (MCA), concretamente muestras de tejido cerebral de ratón.

El objetivo principal es comparar distintos modelos de anotación celular bajo un flujo de procesamiento homogéneo utilizando el framework DANCE.

## Conjunto de datos

- Mouse Cell Atlas (MCA)
- Tejido: Mouse Brain

## Modelos evaluados

- SVM
- ACTINN
- CellTypist
- SingleCellNet





# Experimento 2 — Glioblastoma (SCP393)


El segundo experimento se centra en el análisis transcriptómico de muestras de glioblastoma utilizando datos públicos de secuenciación scRNA-seq.

El objetivo de este experimento es estudiar la heterogeneidad celular del glioblastoma y evaluar distintos modelos de clasificación celular sobre datos reales de tumores cerebrales.

Además del entrenamiento de modelos, el experimento incluye un flujo completo de exploración, control de calidad, procesamiento y visualización de datos mediante Scanpy y estructuras AnnData.


## Conjunto de datos

Los datos utilizados en este experimento fueron obtenidos del portal público:

https://singlecell.broadinstitute.org/single_cell/study/SCP393/single-cell-rna-seq-of-adult-and-pediatric-glioblastoma?tab=scatter

Correspondiente al repositorio:

- Broad Institute Single Cell Portal
- Dataset: SCP393


## Subconjuntos utilizados

### Smart-seq2 (SS2)
Archivos principales utilizados:
- IDHwtGBM.processed.SS2.logTPM.txt
- IDHwt.GBM.Metadata.SS2.txt

### 10X Genomics
Archivos principales:
- matrices .mtx de expresión,
- genes.tsv,
- barcodes/cells.tsv.


## Modelos evaluados
- SVM (LinearSVC)
- Random Forest
- ACTINN
- CellTypist
- PySingleCellNet




---
# Configuración del entorno
Los experimentos fueron desarrollados principalmente en Google Colab utilizando:

- Python 3.11
- Scanpy 1.10.1
- AnnData 0.10.8
- PyTorch 2.2.2
- scikit-learn 1.5.1
- numpy 



---

# Ejecución
Se recomienda reiniciar el entorno tras determinadas instalaciones de librerías para evitar conflictos de dependencias.




