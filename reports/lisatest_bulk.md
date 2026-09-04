# Lisatest – POST /students/bulk API piirang

Staatus: **API EI TOETA ENDPOINTI**

Seda lisatesti ei nõua õpetaja lõplik PDF. Vabatahtlik kontroll saadab
endpointile `POST http://localhost:3000/students/bulk` vähemalt kahe õpilase
JSON-massiivi. Kloonitud õpetaja API `app.js` lähtekoodis seda endpointi ei ole.

Päris serverile saadeti korrektne kahe õpilase massiiv. Käsurea kontrolli
tulemus oli:

```text
STATUS 404
CONTENT_TYPE text/html; charset=utf-8
BODY Cannot POST /students/bulk
```

Õpetaja API-d ei muudetud ja bulk-endpointi omavoliliselt ei lisatud. 404 on
selle vabatahtliku lisatesti dokumenteeritud API piirang ega mõjuta lõpliku
PDF-i kohustuslike ülesannete staatust.
