# Postmani ülesanne 7 – bulk-lisamine

Staatus: **BLOCKED**

PDF nõuab endpointi `POST http://localhost:3000/students/bulk`, millele tuleb
saata vähemalt kahe õpilase JSON-massiiv. Kloonitud õpetaja API `app.js`
lähtekoodis seda endpointi ei ole.

Päris serverile saadeti korrektne kahe õpilase massiiv. Käsurea kontrolli
tulemus oli:

```text
STATUS 404
CONTENT_TYPE text/html; charset=utf-8
BODY Cannot POST /students/bulk
```

Õpetaja API-d ei muudetud ja bulk-endpointi omavoliliselt ei lisatud. Seetõttu
ei saa Ülesannet 7 praeguse õpetaja API versiooniga nõuetekohaselt lõpetada ega
PASS-iks märkida.
