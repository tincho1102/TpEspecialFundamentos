
# Análisis de Enfermedad Renal Crónica (CKD) y Variables Clínicas

Este repositorio contiene el desarrollo del análisis exploratorio y multivariado sobre el conjunto de datos de la Encuesta Nacional de Salud y Nutrición de EE. UU. (NHANES 2021-2023). El objetivo principal es identificar factores clínicos, corporales y demográficos asociados a la presencia de Enfermedad Renal Crónica (CKD) mediante técnicas de estadística y aprendizaje supervisado/no supervisado.

---

## Requisitos Previos

Asegúrate de contar con lo siguiente instalado en tu sistema:

* **Python 3.10** o superior.
* **Git** (para clonar el repositorio).
* **Jupyter Notebook**

---

## Instrucciones para la Instalación y Ejecución

Sigue estos pasos para reconstruir el entorno de desarrollo y ejecutar el código localmente:

### 1. Clonar el repositorio
Abre una terminal y clona el proyecto en tu máquina local:

```bash
git clone https://github.com/tincho1102/TpEspecialFundamentos.git
cd TpEspecialFundamentos

```

### 2. Crear y activar un entorno virtual

Para evitar conflictos de dependencias con otras librerías de Python, se recomienda crear un entorno virtual limpio:

* **En Linux / macOS:**
```bash
python3 -m venv venv
source venv/bin/activate

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

##  Estructura del Repositorio

```text
├── CKD_NHANES_2021_2023.csv   # Archivo de datos con variables clínicas y demográficas
├── analisis.ipynb             # Notebook única de Jupyter con el desarrollo del proyecto
├── README.md                  # Guía de instrucciones para ejecución local
├── requirements.txt           # Librerías de Python necesarias para reconstruir el entorno
└── Informe-TPEspecial.pdf     # Informe escrito con hallazgos y conclusiones principales

