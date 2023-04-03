# Jupiter trojans

## Breve descripción 📖

El presente repositorio recoge una serie de archivos y códigos empleados para unir bases de datos de asteroides y analizar sus observaciones. Se cuenta con tres catálogos: Gaia DR2, Gaia DR3 y SVO MOC. 

La metodología seguida consiste en:

1. Arreglar y completar los catálogos de forma individual, preparándolos para ser unificados. Solo se utilizarán las observaciones de troyanos de Júpiter.
2. Unir los catálogos en función de los datos en común que se tengan.
3. Se crean subcatálogos con los asteroides de L4 y L5 por separado.
4. Se analizan los datos conjuntamente de los troyanos de Júpiter.


## Requisitos para ejecutar los códigos ⚙️

Algunos datos de Gaia DR3 y SDSS (entre ellos, los orginales) se encuentran disponibles para ser descargados [aquí](https://drive.google.com/drive/folders/1iRTPjhQL8YtAJDXacUd6ybkmz607drWK?usp=sharing). Se organizan en las correspondientes carpetas como se detalla acontinuación:

```
Datos_Gaia/ Gaia_DR3.csv
            Gaia_DR3_completed.csv
         
Datos_Sloan/ svomoc.csv
             SDSS_completed.csv
```             

Los paquetes de terceros de Python que deben tener instalados para la ejecución de los códigos son:

- [numpy](https://numpy.org/)
- [matplotlib](https://matplotlib.org/)
- [pandas](https://pandas.pydata.org/)
- [astropy](https://www.astropy.org/)
- [seaborn](https://seaborn.pydata.org/)
- [astroquery](https://astroquery.readthedocs.io/en/latest/)
- [pyedra](https://pyedra.readthedocs.io/en/latest/)


## Estructura del repositorio 📋  

Los códigos están explicados individualmente dentro de cada archivo.

Una breve descripción de cada uno:

`Gaia_DR2.ipynb`                      - Completa y arregla datos obtenidos de Gaia DR2
 
`Gaia_DR3.ipynb`                      - Completa y arregla datos obtenidos de Gaia DR3

`SDSS.ipynb`                          - Completa y arregla datos obtenidos del SVO MOC

`Merge_catalogs.ipynb`                - Une los distintos catálogos y crea los subcatálogos de asteroides de L4 y L5

`Analysis_Jupiter_trojans_Gaia.ipynb` - Analiza los datos de asteroides provenientes unicamente de Gaia DR2 y DR3

Por otro lado, los archivos con las observaciones se encuentran en las respectivas carpetas: aquellos documentos relativos a observaciones de Gaia están en la carpeta `\Datos_Gaia\`, los relativos a SDSS en `\Datos_Sloan\`, y los comunes en `\Datos\`.
