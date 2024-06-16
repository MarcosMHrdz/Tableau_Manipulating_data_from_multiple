![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Laboratorio | Tableau: manipulación de datos de múltiples fuentes

Para esta práctica de laboratorio, usaremos el conjunto de datos del Caso de Negocio de Análisis de Clientes. Este conjunto de datos se puede encontrar en la carpeta `files_for_lab`.

En esta práctica de laboratorio, veremos el archivo pdf, `files_for_lab/nz_water_water_resources.pdf`, pero veremos las otras dos tablas, es decir. `página 14 tabla 2` y `página 14 tabla 3`.

## Contexto


Como se analizó durante la última lección, estas son otras dos formas en las que Tableau lee los datos de la tabla de la página 14 en el archivo PDF.

  - `página 14 tabla 2` representa la mitad de la información
  - `página 14 tabla 3` representa la otra mitad de la información



### Instrucciones

1. Crea una unión entre las dos tablas.
2. Oculte la columna "Nombre de la tabla".
3. Limpiar los datos.

**Consejos**:

- Verá que la información de la _columna 1_ del archivo PDF se divide en dos columnas diferentes cuando los datos se importaron usando Tableau. Seleccione las dos columnas y luego use la opción "fusionar campos que no coinciden" para combinar esas dos columnas.
- Cambie el nombre de las columnas de forma adecuada (cambie el nombre de los encabezados a años, como se indica en el PDF)
- A diferencia del caso anterior, aquí mantendremos todas las fuentes excepto los totales (es decir, filtraremos el total y conservaremos el resto)
- Seleccione los datos y cree un pivote como se muestra a continuación
  ![Crear pivote](https://education-team-2020.s3-eu-west-1.amazonaws.com/data-analytics/6.1-create_pivot_tableau.png)
- Cambie el nombre de las columnas a "fuente", "año" y "millones de metros cúbicos".
- Como habrás notado, todavía habrá algunos valores nulos en la columna "millones de metros cúbicos". Elimina esos nulos.
- Convertir el tipo de columna de años al tipo Fecha.
- Convertir el tipo de columna `millones de metros cúbicos` a números enteros.
- Todavía habría algunos problemas con los nombres de las fuentes en la primera columna. Seleccione el menú desplegable de columnas y elija Alias.

  - Como se puede ver en el archivo PDF, "hidroelectricidad" debería ser "abstracción de hidroelectricidad"; y la generación debería ser "descarga procedente de la generación hidroeléctrica".
  - Adelante, cambia esos alias.
    ![Aliases_de_edición](https://education-team-2020.s3-eu-west-1.amazonaws.com/data-analytics/6.1-edit_aliases.png)
  - Cambiar dimensiones a medidas cuando sea necesario.
  - Ahora ve a la hoja, crea un gráfico y muestra las 4 principales fuentes de generación. La trama final debería verse así. Tenga en cuenta que aquí hemos utilizado un filtro en la hoja para eliminar la columna con descarga.

  ![Ejemplo de trama](https://education-team-2020.s3-eu-west-1.amazonaws.com/data-analytics/6.1-lab_final_plot.png)