# Postman-Tests

Projekti eesmärk on testida õpetaja Students API-t Postmani collectioni ja
Newmani abil. Õpetaja API repo:
`https://github.com/Sanksernebo/API-Postman`

## Õpetaja API käivitamine

Klooni või ava õpetaja API repo ning käivita seal:

```text
npm install
node server.js
```

Server peab töötama aadressil `http://localhost:3000`.

## Postmani collection

Impordi Postmani fail:

```text
postman/Students_API.postman_collection.json
```

Collection kasutab muutujat `baseUrl` väärtusega `http://localhost:3000`.
Loodud õpilase ID salvestatakse dünaamiliselt muutujasse `createdStudentId`,
mistõttu loomise, muutmise ja kustutamise ahel ei sõltu fikseeritud ID-st.

## Newmani käivitamine

Installi selle repo sõltuvused ja käivita collection:

```text
npm install
npm run test:api
```

Lõpliku kontrollkäivituse väljund asub failis
`outputs/postman_newman_output.txt`.

## Ülesannete olek

- Ülesanne 1: PASS – kõikide õpilaste GET.
- Ülesanne 2: PASS – ühe olemasoleva õpilase GET.
- Ülesanne 3: PASS – õpilase POST ja GET-kontroll.
- Ülesanne 4: PASS – kahe välja PUT ja GET-kontroll.
- Ülesanne 5: PASS – loodud õpilase DELETE ja 404 kontroll.
- Ülesanne 6: PASS – olematu õpilase PUT-vea kontroll.
- Ülesanne 7: **BLOCKED** – teacher API does not implement `POST /students/bulk`.
- Ülesanne 8: PASS – olematu õpilase DELETE-vea kontroll.
- Ülesanne 9: PASS – puuduva `major` välja valideerimine.
- Ülesanne 10: PASS – vähemalt ühe õpilase Postmani test.
- Ülesanne 11: PASS – keskmise vanuse arvutus ja test.
- Ülesanne 12: PASS – üks collection, lokaalne Newman ja salvestatud väljund.

Ülesande 7 blokeeringu tõendid asuvad failis `reports/task7.md`. Õpetaja API-d
ei ole muudetud ja bulk-requestile ei ole lisatud valet PASS-testi.

Postmani GUI-s käsitsi tehtavad screenshotid on loetletud failis
`SCREENSHOT_CHECKLIST.md`.
