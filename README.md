# Servicio de grado de confianza de usuarios y comunidades

### para correr el proyecto:

    git clone https://github.com/lschirripa/service-02-calculador-confianza.git

### navegar al directorio src:

    cd src

### instalar la virtual enviromen en la cual correra nuestro proyecto de fast api

    python -m venv venv

### activar la venv (la siguiente linea de codigo pertenece a una terminal powershell)

    venv/scripts/activate

### una vez dentro de la venv, instalar las dependencias necesarias establecidas en el .txt para correr la aplicacion

    pip install -r requirements.txt

### para correr el proyecto

    uvicorn main:app --reload

Una vez levantado, se podra acceder al swagger de la api mediante http://127.0.0.1:8000.

## Como usar:

- La api solo provee un unico endpoint POST, en donde el INPUT sera una comunidad junto a sus usuarios e incidentes. La aplicacion necesitara algunos datos de los usuarios y de los incidentes para poder realizar los calculos correspondientes. El OUTPUT, sera la devolucion de cada usuario con su nuevo nivel de confianza, el nivel de confianza de la comunidad, y una recomendacion para cada user😉

- Para tener una idea de que tipo de variable espera cada campo del body para el input, bastara con abrir el endpoint y dentro del example value se podra visualizar. Lo mismo con la respuesta, debajo estan documentadas los ejemplos de respuesta tanto como para un codigo 200 o 422.

- Para mas detalle, debajo del endpoint se encuentran los Schemas, que nos van a servir para saber como se conforman nuestros objetos.

- De todas formas, dejamos aca un json de ejemplo para que puedan probar. Esta comunidad solo tendra 4 incidentes y 2 usuarios.





