# Análisis de Enfermedad Renal Crónica (CKD) y Variables Clínicas

Este repositorio contiene el desarrollo del análisis exploratorio y multivariado sobre el conjunto de datos de la Encuesta Nacional de Salud y Nutrición de EE. UU. (NHANES 2021-2023). El objetivo principal es identificar factores clínicos, metabólicos y demográficos asociados a la presencia de Enfermedad Renal Crónica (CKD) mediante técnicas de estadística inferencial y aprendizaje supervisado/no supervisado.

---

## Instrucciones de Instalación y Ejecución

Sigue estos pasos para reconstruir el entorno de desarrollo y ejecutar el código localmente:

### 1. Clonar el repositorio
Abre una terminal y clona el proyecto en tu máquina local:

```bash
git clone https://github.com/tincho1102/TpEspecialFundamentos.git
cd TpEspecialFundamentos

```

### 2. Crear y activar un entorno virtual (Recomendado)

Para evitar conflictos de dependencias con otras librerías de Python, se recomienda crear un entorno virtual limpio:

* **En Linux / macOS:**
```bash
source env/bin/activate

```


* **En Windows (CMD):**
```cmd
python -m venv venv
venv\Scripts\activate

```


* **En Windows (PowerShell):**
```powershell
python -m venv venv
.\venv\Scripts\activate

```



### 3. Instalar las dependencias

Con el entorno virtual activo, instala todas las librerías necesarias especificadas en el archivo `requirements.txt`:

```bash
pip install -r requirements.txt

```

### 4. Vincular el entorno virtual a Jupyter (Crear el Kernel)

Registra el entorno virtual para poder seleccionarlo dentro de Jupyter:

```bash
python -m ipykernel install --user --name=env_ckd --display-name="Python (CKD Analysis)"

```

### 5. Ejecutar la Notebook

Inicia Jupyter Notebook o JupyterLab:

```bash
jupyter notebook

```

1. Abre el archivo de la notebook principal (`analisis.ipynb`).
2. En el menú superior de Jupyter, asegúrate de seleccionar el Kernel **`Python (CKD Analysis)`** (en *Kernel > Change Kernel*).
3. Ejecuta las celdas de forma secuencial (*Cell > Run All* o `Shift + Enter`).

---

## 📁 Estructura del Repositorio

```text
├── dataset.csv            # Archivo de datos con variables clínicas y demográficas
├── analisis.ipynb         # Notebook única de Jupyter con el desarrollo del proyecto
├── README.md              # Guía de instrucciones para ejecución local
├── requirements.txt       # Librerías de Python necesarias para reconstruir el entorno
└── Informe_CKD.pdf        # Informe escrito con hallazgos y conclusiones principales

```

---

## 📊 Resumen de Técnicas Utilizadas

* **Estadística Descriptiva e Inferencial:** Gráficos bivariados, tests de normalidad (Shapiro-Wilk) y pruebas no paramétricas (U de Mann-Whitney).
* **Regresión Logística Múltiple:** Evaluación del impacto conjunto de variables cuantitativas y categóricas (*Dummy Encoding*) sobre la probabilidad de diagnóstico de CKD.
* **Análisis de Componentes Principales (PCA):** Reducción de dimensionalidad, evaluación de varianza explicada acumulada (*Elbow Plot*) y análisis de vectores (*Biplot*) para identificar agrupaciones biológicas en datos clínicos.

```

---

### Recomendaciones finales antes de hacer el `push`:
1. **Nombre de los archivos:** Revisa que los nombres de los archivos en tu repositorio coincidan exactamente con los que puse en la estructura (`dataset.csv`, `analisis.ipynb`, etc.) o edítalos en el Markdown si se llaman de otra forma.
2. **Link del repo:** Recuerda reemplazar `[https://github.com/tu-usuario/tu-repositorio.git](https://github.com/tu-usuario/tu-repositorio.git)` por la URL real de tu repositorio.

```
