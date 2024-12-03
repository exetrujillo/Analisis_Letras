# Letras de Canciones con LRC Lib API

Este proyecto permite obtener canciones y sus letras de un artista o banda específica, utilizando la API de [LRC Lib](https://lrclib.net/). El resultado se guarda en un archivo CSV y también se puede analizar directamente en R.

## Funcionalidades

1. Buscar canciones de un artista.
2. Obtener las letras de cada canción.
3. Consolidar los datos en un DataFrame de R.
4. Exportar los resultados a un archivo CSV.

## Requisitos

- **R (>= 4.0)**: Asegúrate de tener una versión reciente de R instalada.
- **Librerías de R**: Este proyecto utiliza las siguientes librerías, que pueden ser instaladas ejecutando el comando `install.packages()`:
  - `httr`
  - `jsonlite`
  - `dplyr`

## Configuración

1. **Clonar el repositorio o copiar el script**: Descarga el script principal en tu máquina.
2. **Configurar la API**: Modifica la variable `base_url` en el script si hay cambios en el endpoint base de la API. Si necesitas una clave API, asegúrate de incluirla en los encabezados de la solicitud (ver sección "Autenticación").

## Uso

1. **Cargar el script en R**: Abre el archivo del script en tu entorno de desarrollo (RStudio u otro).
2. **Ejecutar el script**:
   - Define el nombre del artista o banda modificando la variable `artista`.
   - Ejecuta el código para obtener y guardar los resultados.
3. **Resultados**:
   - Los resultados se muestran en consola y se guardan como un archivo CSV llamado `{nombre_del_artista}_letras.csv`.
