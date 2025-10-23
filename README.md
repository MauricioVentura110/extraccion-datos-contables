# extraccion-datos-contables
Extracción automatizada de campos particulares de archivos XML para registro contable.

## Descripción

Este proyecto personal extrae **cuatro datos (campos) relevantes** de archivos XML:
- Nombre del cliente  
- Número de folio  
- Nombre del archivo  
- Letra  

Estos datos se utilizan en un proceso contable particular para anexarlos a registros de **ventas**, **cobros** y **descuentos**.  
Con ellos, el programa genera automáticamente una **carpeta con los archivos XML filtrados (renombrados con los campos)**, facilitando su revisión a partir de cualquiera de los datos extraídos.

Además, el programa crea **dos archivos Excel**:
1. XML que **no tienen folio**.  
2. XML que **no cumplen las condiciones** del programa y deben revisarse manualmente.

---

## Tecnologías utilizadas

* **Lenguaje:** Python 3.11.5  
* **Librerías:**
  * `os`
  * `glob`
  * `xml.etree.ElementTree`
  * `pandas` (2.0.3)
  * `shutil`
  * `zipfile`

---

## Ejecución

Este proyecto está implementado en un **Jupyter Notebook** (`.ipynb`).

Para ejecutarlo:

1. Instala las dependencias necesarias en caso de no tenerlas:
   ```bash
   pip install pandas
