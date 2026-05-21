# Chat en tiempo real

## Integrantes
proyecto desarrollado por los estudiantes 
  
   -Cordero

   -Pedro

## Informacion directa
- [instalacion Y configuracion](#Instalacion)
- [Configuracion2 Con el Firebase](#Configuracion2)
- [Uso](#uso)

## Instalacion Y configuracion local
comandos para probar este proyecto con firebase:

Crea un entorno virtual:
   - **python -m venv venv**

Activa el entorno virtual:
  - (linux) 
    
    **source venv/bin/activate**
    
  - (windows) 
    
    **venv\Scripts\activate**

Instala las dependencias requeridas:
   - **pip install -r requirements.txt**

inicia servidor Flask:
   > **python app.py**

## Configuracion2 Con el Firebase
ve a la web consolefirebase  y crea un proyecto
- En menu izquierdo> Databases & Storage> Create Database>next>next
- En menu izquierdo> settings> General> App web> (copia todo el const firebaseConfig = {cosas}) y sustituyelo por el que esta en el login.html

- En menu izquierdo> settings> Service accounts> Python> Generate new private key  (sustituye este archivo credenciales.json por lo que tenga el nuevo que se descargo)

-copia el (databaseURL: "link") del firebaseconfig y pegalo en app.py (linea 11 aprox)
## Uso
