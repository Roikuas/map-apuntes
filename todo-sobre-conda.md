# Mapa Mental de Comandos de Conda

## 1. Gestión de Entornos

- **Crear Entorno**

  - `conda create --name myenv`
  - `conda create -n myenv python=3.8`
  - `conda create --prefix ./myenv`
  - `conda create -p ./myenv python=3.8`

- **Activar Entorno**

  - `conda activate myenv`
  - `conda activate ./myenv`

- **Desactivar Entorno**

  - `conda deactivate`

- **Eliminar Entorno**

  - `conda remove --name myenv --all`
  - `conda env remove --name myenv`
  - `conda env remove -p ./myenv`

- **Listar Entornos**

  - `conda env list`
  - `conda info --envs`

- **Clonar Entorno**

  - `conda create --name newenv --clone oldenv`

- **Copiar Entorno**

  - `conda env export > environment.yml`
  - `conda env create -f environment.yml`

- **Cambiar Nombre de Entorno**
  - No hay un comando directo, pero se puede clonar y eliminar el entorno antiguo.

## 2. Gestión de Paquetes

- **Instalar Paquete**

  - `conda install package_name`
  - `conda install -n myenv package_name`

- **Instalar Paquete desde un Canal Específico**

  - `conda install -c conda-forge package_name`
  - `conda install -c channel_name package_name`

- **Instalar Paquete desde un Archivo YAML**

  - `conda env create -f environment.yml`

- **Actualizar Paquete**

  - `conda update package_name`
  - `conda update -n myenv package_name`

- **Actualizar Todos los Paquetes en un Entorno**

  - `conda update --all`

- **Eliminar Paquete**

  - `conda remove package_name`
  - `conda remove -n myenv package_name`

- **Listar Paquetes**

  - `conda list`
  - `conda list -n myenv`

- **Buscar Paquete**
  - `conda search package_name`

## 3. Gestión de Conda

- **Actualizar Conda**

  - `conda update conda`
  - `conda update conda -c conda-forge`

- **Información de Conda**

  - `conda info`
  - `conda info --envs`
  - `conda info --channels`

- **Configurar Conda**

  - `conda config --set key value`
  - `conda config --add channels channel_name`
  - `conda config --remove channels channel_name`
  - `conda config --get channels`

- **Listar Canales**

  - `conda config --get channels`

- **Limpiar Caché**
  - `conda clean --all`
  - `conda clean --packages`
  - `conda clean --tarballs`
  - `conda clean --index-cache`

## 4. Otros Comandos Útiles

- **Exportar Entorno**

  - `conda env export > environment.yml`
  - `conda env export --no-builds > environment.yml`

- **Importar Entorno**

  - `conda env create -f environment.yml`

- **Listar Paquetes Específicos de un Entorno**

  - `conda list -n myenv package_name`

- **Mostrar Dependencias de un Paquete**

  - `conda info package_name`

- **Verificar Integridad de Paquetes**
  - `conda verify package_name`

## 5. Comandos de Conda-Build

- **Crear un Paquete**

  - `conda build recipe_folder`

- **Convertir Paquete**

  - `conda convert package.bz2 -p all`

- **Subir Paquete**

  - `anaconda upload package.bz2`

- **Inspeccionar Paquete**
  - `conda inspect linkages package_name`
  - `conda inspect objects package_name`

## 6. Comandos de Conda-Env

- **Crear Entorno desde un Archivo YAML**

  - `conda env create -f environment.yml`

- **Exportar Entorno a un Archivo YAML**

  - `conda env export > environment.yml`

- **Listar Entornos**

  - `conda env list`

- **Eliminar Entorno**

  - `conda env remove -n myenv`
  - `conda env remove -p ./myenv`

- **Copiar Entorno**

  - `conda env export > environment.yml`
  - `conda env create -f environment.yml`

- **Actualizar Entorno desde un Archivo YAML**
  - `conda env update -f environment.yml`

## 7. Gestión de Canales

- **Agregar Canal**

  - `conda config --add channels channel_name`

- **Eliminar Canal**

  - `conda config --remove channels channel_name`

- **Listar Canales**

  - `conda config --get channels`

- **Priorizar Canal**
  - `conda config --add channels channel_name --append`

## 8. Gestión de Conda-Build

- **Crear Paquete**

  - `conda build recipe_folder`

- **Inspeccionar Paquete**

  - `conda inspect linkages package_name`
  - `conda inspect objects package_name`

- **Convertir Paquete**

  - `conda convert package.bz2 -p all`

- **Subir Paquete**
  - `anaconda upload package.bz2`

## 9. Otros Comandos Avanzados

- **Crear Entorno con Paquete Específico**

  - `conda create --name myenv package_name`

- **Forzar Instalación de una Versión Específica**

  - `conda install package_name=1.2.3`

- **Instalar Paquete desde un Archivo Local**

  - `conda install /path/to/package.tar.bz2`

- **Mostrar Dependencias de un Paquete**

  - `conda info package_name`

- **Verificar Integridad de Paquetes**
  - `conda verify package_name`
