
# Conda Environments Install 🌐🔧🐍

## Fuente: 📚

[Anaconda Documentation](https://docs.anaconda.com/)
```
https://docs.anaconda.com/
```

## Pasos a seguir para la instalación

### 1. Descargar e instalar Miniconda

- Descarga el script de instalación de Miniconda para macOS ARM64:
```bash
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
```

- Ejecuta el script de instalación:
```bash
bash Miniconda3-latest-MacOSX-arm64.sh
```

> **TIP:** Durante la instalación, sigue las instrucciones en pantalla. Se te pedirá que aceptes el acuerdo de licencia y elijas la ubicación de instalación. Es recomendable instalar Miniconda en la ubicación predeterminada.

### 2. Configurar el entorno

- Recarga tu perfil de shell para aplicar los cambios de Miniconda:
```bash
source ~/.bash_profile
```

- Verifica la instalación de `conda`:
```bash
which conda
```

> **NOTE:** Si el comando anterior devuelve la ruta a `conda`, significa que la instalación se ha realizado correctamente. Si no es así, asegúrate de que Miniconda se haya añadido correctamente a tu `PATH`.

### 3. Crear un entorno Conda

- Crea un nuevo entorno con Python 3.10:
```bash
conda create --name prjct_assortments python=3.10
```

> **IMPORTANT:** Elegir un nombre descriptivo para tu entorno te ayudará a recordar su propósito. Aquí hemos usado `prjct_assortments`.

### 4. Activar el entorno

- Activa el entorno recién creado:
```bash
conda activate prjct_assortments
```

> **TIP:** Una vez que el entorno está activo, cualquier paquete que instales usando `pip` o `conda` se instalará solo en este entorno, manteniendo tu instalación base de Python limpia.

### 5. Instalar pyodbc

- Instala `pyodbc` usando `pip`:
```bash
pip install pyodbc
```

> **NOTE:** `pyodbc` es una biblioteca que permite a Python conectarse a bases de datos ODBC. Asegúrate de que cualquier controlador ODBC necesario esté instalado y configurado correctamente.

> **WARNING:** Recuerda siempre activar tu entorno antes de trabajar en tu proyecto para asegurarte de que estás utilizando las dependencias correctas.

---

Con esta guía, deberías poder configurar tu entorno Conda de manera efectiva en macOS. Si encuentras algún problema, revisa la [documentación de Anaconda](https://docs.anaconda.com/) para obtener más ayuda.
