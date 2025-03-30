# Scraping de Noticias - La Vanguardia  
## Extracción automatizada de artículos con Selenium  

Este proyecto realiza web scraping en la página principal de La Vanguardia para obtener información clave de las noticias, como el título, la fecha de publicación, el autor, la imagen destacada y el epígrafe. Se ha implementado en Python utilizando la biblioteca Selenium para navegar y extraer los datos de manera automatizada.  

## Autores  
Sergio Frutos Serrano y Inés Ripoll González

---

## Estructura del Proyecto  

```
/lavanguardia_scraper
│── README.md                 # Documentación del proyecto y guía de uso
│── requirements.txt          # Lista de dependencias necesarias
│── /source
│   └── lavanguardia_scraper.py  # Código Python que ejecuta el scraping
│── /dataset
│   └── lavanguardia_dataset.csv  # Archivo CSV con los datos extraídos
```  

---

## Requisitos Previos  

Antes de ejecutar el script, asegúrate de cumplir con los siguientes requisitos:  

### Instalar Dependencias  

Ejecuta el siguiente comando para instalar las librerías necesarias:  

```bash
pip install -r requirements.txt
```  

### Descargar ChromeDriver  

Selenium requiere ChromeDriver para interactuar con la web. Descárgalo desde:  
🔗 [https://sites.google.com/chromium.org/driver/](https://sites.google.com/chromium.org/driver/)  

Ubica el ejecutable en un directorio accesible desde tu sistema:  
- **Linux/Mac:** `/usr/bin/chromedriver`  
- **Windows:** La carpeta donde tengas Chrome instalado  

---

## Ejecución del Script  

Para iniciar el proceso de scraping, navega hasta la carpeta donde está el código y ejecuta:  

```bash
python source/lavanguardia_scraper.py
```  

El script realizará lo siguiente:  
✔ Accederá a la página principal de La Vanguardia.  
✔ Hará scroll para cargar más noticias.  
✔ Extraerá la información clave de los primeros 10 artículos.  
✔ Guardará los datos en un archivo CSV.  

---

## Datos Obtenidos  

El script genera un archivo llamado `lavanguardia_dataset.csv` dentro de la carpeta `/dataset/`. Este archivo contiene:  

- **Título** del artículo  
- **Enlace** a la noticia  
- **Fecha de publicación**  
- **Imagen destacada**  
- **Autor** del artículo  
- **Epígrafe** (subtítulo o frase destacada de la noticia)  

Puedes abrir este archivo en herramientas como Excel o Google Sheets para analizar los datos extraídos.  

---

## DOI de Zenodo del dataset generado:
https://doi.org/10.5281/zenodo.15109642


## Referencias y Recursos  

- Subirats, L., Calvo, M. (2019). _Web Scraping_. Editorial UOC.  
- Lawson, R. (2015). _Web Scraping with Python_. Packt Publishing Ltd.  
- Selenium Documentation: [https://www.selenium.dev/documentation/](https://www.selenium.dev/documentation/)  
