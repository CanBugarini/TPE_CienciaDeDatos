# Análisis de datos – Proyecto de Ciencia de Datos

## Descripción del proyecto

Este repositorio contiene un análisis exploratorio y estadístico de datos de alojamientos de Airbnb, con el objetivo de estudiar la relación entre las características de los alojamientos y su precio por noche.

El proyecto incluye análisis exploratorio de datos (EDA), limpieza y preprocesamiento, tratamiento de valores atípicos, análisis de correlaciones y modelos estadísticos.

## Estructura del repositorio

El repositorio está organizado de la siguiente manera:

```text
proyecto-ciencia-de-datos/
│
├── entrega.ipynb              # Notebook con todos los análisis
├── requirements.txt           # Dependencias del proyecto
├── listings (1).csv.gz        # Dataset utilizado
└── README.md                  # Documentación e instrucciones
```

**Importante:** los archivos CSV deben encontrarse en el directorio raíz del proyecto para que las rutas utilizadas en la notebook funcionen correctamente.

## Requisitos previos

Antes de comenzar, es necesario tener instalado:

- Python 3.10 o superior.
- Git (opcional, para clonar el repositorio).
- pip (administrador de paquetes de Python).

Se puede verificar la instalación de Python ejecutando:

```bash
python --version
```

## Instalación y configuración

Para ejecutar el proyecto se recomienda crear un entorno virtual de Python. Esto permite instalar las dependencias necesarias de manera aislada, sin modificar las bibliotecas de Python del sistema.

### 1. Clonar el repositorio

Desde una terminal, ejecutar:

```bash
git clone URL_DEL_REPOSITORIO
```

Ingresar al directorio del proyecto:

```bash
cd proyecto-ciencia-de-datos
```

### 2. Crear el entorno virtual

Ejecutar el siguiente comando:

```bash
python -m venv .venv
```

Esto creará un entorno virtual llamado `.venv` dentro del directorio del proyecto.

### 3. Activar el entorno virtual

**Windows (PowerShell):**

```powershell
.\.venv\Scripts\Activate.ps1
```

**Linux / macOS:**

```bash
source .venv/bin/activate
```

Una vez activado, el nombre del entorno virtual debería aparecer al comienzo de la línea de comandos.

### 4. Instalar las dependencias

Con el entorno virtual activado, actualizar pip:

```bash
python -m pip install --upgrade pip
```

Luego, instalar todas las bibliotecas necesarias especificadas en `requirements.txt`:

```bash
pip install -r requirements.txt
```

Esto instalará automáticamente las versiones de las dependencias definidas para el proyecto.

### 5. Registrar el entorno como kernel de Jupyter

Para asegurarse de que Jupyter utilice el entorno virtual creado, ejecutar:

```bash
python -m ipykernel install --user --name=proyecto-ciencia-datos --display-name "Python (Proyecto Ciencia de Datos)"
```

De esta manera, el entorno estará disponible como kernel dentro de Jupyter.

## Ejecución del proyecto

Con el entorno virtual activado, iniciar Jupyter Notebook:

```bash
jupyter notebook
```

También se puede utilizar JupyterLab:

```bash
jupyter lab
```

Una vez iniciado:

1. Abrir el archivo `entrega.ipynb`.
2. Seleccionar el kernel **Python (Proyecto Ciencia de Datos)**.
3. Verificar que los archivos CSV estén ubicados en el directorio raíz.
4. Ejecutar las celdas en orden, desde la primera hasta la última.

## Consideraciones importantes

- Es necesario ejecutar las celdas en orden para garantizar que las variables y los DataFrames se encuentren correctamente definidos.
- No modificar los nombres de los archivos CSV sin actualizar las rutas correspondientes en la notebook.
- El archivo `requirements.txt` contiene las dependencias necesarias para reproducir los análisis.
- El dataset debe estar disponible localmente antes de ejecutar la notebook.

## Desactivar el entorno virtual

Una vez finalizado el trabajo, se puede desactivar el entorno virtual ejecutando:

```bash
deactivate
```

---

## Tecnologías utilizadas

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Statsmodels
- Wget

