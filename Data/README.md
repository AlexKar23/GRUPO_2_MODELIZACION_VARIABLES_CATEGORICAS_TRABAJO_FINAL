# Carpeta de Datos (`/data`)

🚨 **ATENCIÓN: Los archivos CSV originales no están subidos a este repositorio por restricciones de tamaño y buenas prácticas (están excluidos en el `.gitignore`).**

Para poder ejecutar los *notebooks* de este proyecto, es necesario descargar los datos originales del Instituto Nacional de Estadística (INE) y colocarlos en esta carpeta.

## 📥 Instrucciones de Descarga

1. Accede a la web del INE para la **Encuesta de Inserción Laboral de Universitarios (EILU 2019)**:
   [Enlace oficial de descarga del INE](https://www.ine.es/dyngs/INEbase/operacion.htm?c=Estadistica_C&cid=1254736176991&menu=resultados&idp=1254735976597#_tabs-1254736195339)
2. Descarga los siguientes archivos correspondientes a los **Egresados de Máster**:
   * `EILU_MAST_2019.csv` (Dataset principal con ~12.000 egresados y ~291 variables).
   * `dr_EILU_MAST_2019.xlsx` (Diccionario de variables para interpretar correctamente las codificaciones).
3. Coloca ambos archivos directamente en este directorio (`/data`).

Una vez descargados, los *notebooks* de la carpeta `/notebooks` podrán ejecutarse sin problema.