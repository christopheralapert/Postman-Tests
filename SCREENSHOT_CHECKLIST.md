# Postmani GUI screenshotide kontrollnimekiri

Codex ei ole neid GUI screenshote teinud. Kasutaja peab Postmanis käsitsi
tegema järgmised pildid.

## Ülesanne 1

- GET `/students` request koos 200 response'iga.
- Vastus või eraldi tekst, kust on näha õpilaste arv ja väljad `id`, `name`,
  `age`, `major`.

## Ülesanne 2

- GET `/students/1` request koos ühe õpilase response'iga.

## Ülesanne 3

- POST `/students` request Body ja 201 response.
- Loodud õpilase GET-kontrollpäring ja response.

## Ülesanne 4

- PUT request Body ja response, kus on näha vähemalt kaks muudetud välja.
- Sama õpilase GET-kontrollpäring ja säilinud muudatustega response.

## Ülesanne 5

- DELETE request ja edukas response.
- Kustutamise GET-kontroll ning 404 response.

## Ülesanne 6

- Vigane PUT `/students/999` request ja 404 response.
- Screenshot või tekst 3–5-lauselise analüüsiga failist `reports/task6.md`.

## Ülesanne 7 – BLOCKED

- Tõend päringust `POST /students/bulk`, mille response on 404
  `Cannot POST /students/bulk`.
- Tõend või tekst, et õpetaja `app.js` failis bulk-endpoint puudub.
- Ülesannet ei tohi näidata PASS-ina.

## Ülesanne 8

- DELETE `/students/999` request ja 404 response.
- Screenshot või tekst vastustega kolmele küsimusele failist
  `reports/task8.md`.

## Ülesanne 9

- POST `/students` puudulik Body, kus `major` puudub.
- 400 `Invalid data` response.
- Screenshot või tekst 2–3-lauselise analüüsiga failist `reports/task9.md`.

## Ülesanne 10

- GET kõik õpilased requesti Tests tab koos testiga
  `Vastuses on vähemalt üks õpilane`.
- Sama testi PASS tulemus Postmani Test Results vaates.

## Ülesanne 11

- GET kõik õpilased Tests tab koos keskmise vanuse skriptiga.
- Postman Console log, kus on näha `Keskmine vanus: 23`.
- Testi `Keskmine vanus arvutatud` PASS tulemus.

## Ülesanne 12

- Collectioni ülevaade Postmanis, kus kõik võimalikud requestid on ühe
  `Students API` collectioni all.
- Collection Runneri tulemus, kus võimalikud testid on PASS ja Ülesanne 7 on
  eraldi BLOCKED, mitte PASS.
- Collection JSON peab jääma reposse faili
  `postman/Students_API.postman_collection.json`.
