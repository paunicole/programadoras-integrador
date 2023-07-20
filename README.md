# ¿A dónde voy en las vacaciones de invierno? Gratis...

El proyecto tiene como objetivo desarrollar un programa que permita registrar y consultar eventos gratuitos que se llevarán a cabo en Argentina durante las vacaciones de invierno. Está dirigido a dos tipos de usuarios: aquellos que quieran registrar un evento con detalles como nombre, descripción, día, mes, hora, provincia y localidad; y aquellos que deseen consultar eventos en su municipio o en un rango de fechas.

## ⚡ Funcionalidades

- `Registro de un nuevo evento`: Los usuarios podrán ingresar los datos del evento y agregarlo a la base de datos en formato JSON.
- `Consulta de eventos por localidad`: Los usuarios podrán buscar eventos específicos en su localidad, obteniendo una lista de eventos que se llevarán a cabo allí.
- `Consulta de todos los eventos`: Se mostrará una lista completa de todos los eventos registrados en el archivo JSON.
- `Consulta de eventos entre dos fechas`: Los usuarios podrán seleccionar un rango de fechas y obtener una lista de eventos que se realizarán dentro de ese período.

## 🏢 Estructura JSON
Los registros de los eventos se guardarán en un archivo JSON, que servirá como base de datos para almacenar la información de los eventos. La estructura de un evento es la siguiente:

```json
{
    "nombre_evento": "Festival por aniversario del Club Atlético Libertad",
    "descripcion": "Evento familiar con músicos locales",
    "dia": 12,
    "mes": "julio",
    "hora": 15,
    "provincia": "Salta",
    "localidad": "Tartagal",
}
```

## 🗺 APIs
Se utilizarán las siguientes APIs externas para obtener la lista de provincias y localidades, facilitando las operaciones de registro y consulta en el programa:

- https://apis.datos.gob.ar/georef/api/provincias?campos=id,nombre

- https://apis.datos.gob.ar/georef/api/municipios?provincia=22&campos=id,nombre&max=100

## ⛏️ Módulos importados
- `requests`: Para realizar solicitudes a las APIs y obtener los datos de provincias y localidades.
- `json`: Para manejar la lectura y escritura de datos en formato JSON.

## ✒️ Autoras

| [<img src="https://avatars.githubusercontent.com/u/133787035?v=4" width=115><br><sub>Evangelina Dioli</sub>](https://github.com/EvangelinaDioli) |  [<img src="https://avatars.githubusercontent.com/u/129181094?v=4" width=115><br><sub>Nicole Cardozo Gómez</sub>](https://github.com/paunicole) |
| :---: | :---: |
