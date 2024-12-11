# Proyecto de Graduación

Este repositorio contiene el código para el proyecto de graduación.

# Descripción

El proyecto consistió en el desarrollo de una aplicación móvil orientada a la gestión de residuos y la reducción de la huella de carbono, diseñada para educar y facilitar prácticas sostenibles entre los usuarios. La aplicación combina herramientas de concientización ambiental con funcionalidades prácticas, como el registro de desechos, su clasificación y el seguimiento del impacto ambiental individual.

Mi participación estuvo enfocada en garantizar la seguridad del proyecto desde su diseño y durante todo el desarrollo. Esto implicó seleccionar las tecnologías adecuadas para cumplir con los estándares de seguridad y asegurar que se siguieran buenas prácticas de codificación para prevenir posibles vulnerabilidades desde las etapas iniciales del desarrollo. Como parte de este esfuerzo, se utilizaron herramientas como SonarCloud, AppSweep y MobSF, que permitieron realizar análisis continuos para identificar y mitigar riesgos de seguridad.

La seguridad en el proyecto destaca por la aplicación de buenas prácticas desde las fases iniciales, lo que evita que las vulnerabilidades se conviertan en problemas costosos de solucionar en etapas posteriores. Este enfoque proactivo aseguró que la aplicación no solo ofreciera una experiencia funcional y atractiva para los usuarios, sino que también fuera robusta y resistente frente a posibles amenazas.

# Instrucciones de Instalación

## SonarCloud

1. Acceder a su pagina web https://sonarcloud.io/ lo ideal es acceder utilizando tu cuenta de github.
2. Crear una nueva organizacion el cual esto te permitira exportar tus proyectos de github a sonarcloud para sus analisis, en el cual se acepta el permiso que pide en enlazar github con sonarcloud. 
3. Seleccionar el proyecto que deseas exportar y darle en crear.
4. En las opciones para analisar el codigo escoger Githunb Actions y seguir los pasos detallados que menciona este. 
    - Ir a settings > Secrets > Actions
    - Crear un secret llamado SONAR_TOKEN
    - Agregar el valor dado por sonarcloud
    - Crear y agregar el build file (seleccionar segun la tecnologia utilizada)
5. Listo ya cualquier cambio que realices este sera analiado y mostrado en sonarcloud

## AppSweep

1. Acceder a su pagina web https://appsweep.guardsquare.com/ el cual seguir las instrucciones para crear tu cuenta
2. Generar en este caso el app o proyecto el cual se cargara al .apk correspondiente. 
3. Esperar a que este termine y se mostrara el resultado para ser consultado.

## MobSF

1. Acceder a su repositorio de github https://github.com/MobSF/Mobile-Security-Framework-MobSF y descargar el proyecto desde la parte de Releases.
2. Seguir los pasos de la documentacion dada si se desea correr en docker
3. En caso que se desea correr todo manualmente seguir

### Kali
1. Instalar git
```bash
sudo apt-get install git
```
2. Instalar python 3.8/3.9
```bash
sudo apt-get install python3.8
```
3. Instalar la ultima version de JDK
4. Instalar las dependencias requeridas
```bash
sudo apt install python3-dev python3-venv python3-pip build-essential libffi-dev libssl-dev libxml2-dev libxslt1-dev libjpeg62-turbo-dev zlib1g-dev wkhtmltopdf
```
5. Descargar MobSF
```bash
git clone https://github.com/MobSF/Mobile-Security-Framework-MobSF.git
```
6. Cambiar el directorio al MobSF
7. Preparar el ambiente
```bash
sudo ./setup.sh
```
8. Correr y levantar el MobSF
```bash
/run.sh 127.0.0.1:8000
```

### Windows
1. Instalar git en https://git-scm.com/downloads/win
2. Instalar python 3.8/3.9 https://www.python.org/downloads/
3. Instalar la ultima version de JDK
4. Instalar OpenSSL en https://slproweb.com/products/Win32OpenSSL.html
5. Instalar wkhtmltopdf en https://wkhtmltopdf.org/downloads.html
6. Clonar el repositorio 
```bash
git clone https://github.com/MobSF/Mobile-Security-Framework-MobSF.git
```
7. Cambiarse al directorio del MobSF
8. Prepara el ambiente
```bash
setup.bat
```
9. Correr y levantar el MobSF
```bash
run.bat 127.0.0.1:8000
```