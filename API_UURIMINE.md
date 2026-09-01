# Õpetaja API uurimine

Uuritud projekt: `https://github.com/Sanksernebo/API-Postman`

API käivitati käsuga `node server.js` ja päringud kontrolliti aadressil
`http://localhost:3000`. Andmed asuvad serveri mälus ning serveri taaskäivitamisel
taastuvad kolm algset õpilast.

## Kontrollitud endpointid

### `GET /students`

- Staatus: `200 OK`.
- Vastus: JSON-massiiv.
- Puhta serveri vastuses oli 3 õpilast.
- Õpilase väljad olid `id`, `name`, `age` ja `major`.

### `GET /students/:id`

- Olemasoleva ID `1` korral: `200 OK` ja ühe õpilase JSON-objekt.
- Olematu ID `999` korral: `404 Not Found` ja
  `{"error":"Student not found"}`.

### `POST /students`

- Request on JSON-objekt väljadega `name`, `age` ja `major`.
- Kõigi nõutud väljadega vastus: `201 Created` ning loodud õpilase objekt koos
  serveri määratud `id` väljaga.
- Välja `major` puudumisel: `400 Bad Request` ja
  `{"error":"Invalid data"}`.

### `PUT /students/:id`

- Request on muudetavate väljadega JSON-objekt.
- Olemasoleva ID korral: `200 OK` ning uuendatud õpilase JSON-objekt.
- Järgnev GET tagastas muudetud väärtused.
- Olematu ID korral määrab lähtekood vastuseks `404 Not Found` ja
  `{"error":"Student not found"}`.

### `DELETE /students/:id`

- Olemasoleva ID korral: `200 OK` ja
  `{"message":"Student deleted"}`.
- Kustutamise järel tagastas sama ID GET `404 Not Found`.
- Olematu ID `999` korral: `404 Not Found` ja
  `{"error":"Student not found"}`.

## Muud kontrollitud aadressid

- `GET /` tagastas `404 Not Found` ja HTML-teate `Cannot GET /`.
- `POST /students/bulk` tagastas `404 Not Found` ja HTML-teate
  `Cannot POST /students/bulk`. Kloonitud õpetaja `app.js` failis bulk-endpointi
  ei ole.
