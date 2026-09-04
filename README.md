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
- Ülesanne 7: PASS – `DELETE /students/999` ja 404 analüüs.
- Ülesanne 8: PASS – puuduva `major` välja valideerimine.
- Ülesanne 10: PASS – vähemalt ühe õpilase Postmani test.
- Ülesanne 11: PASS – keskmise vanuse arvutus ja test.
- Ülesanne 12: PASS – üks collection, lokaalne Newman ja salvestatud väljund.

Vabatahtlik `POST /students/bulk` lisatest tagastab 404, sest õpetaja API seda
endpointi ei toeta. See ei ole lõpliku PDF-i Ülesanne 7 ega kohustusliku töö
blokeering. Lisatesti tulemus on failis `reports/lisatest_bulk.md` ja õpetaja
API-d ei ole muudetud.

## Kontrollitud Postmani screenshotid

Kasutaja käsitsi tehtud Postmani screenshotid kontrolliti visuaalselt ja
kopeeriti kausta `screenshots/`.

- Ülesanne 1: [GET kõik õpilased](screenshots/task1_get_all.png)
- Ülesanne 2: [GET üks õpilane](screenshots/task2_get_one.png)
- Ülesanne 3: [POST](screenshots/task3_post.png) ja [GET-kontroll](screenshots/task3_get_check.png)
- Ülesanne 4: [PUT](screenshots/task4_put.png) ja [GET-kontroll](screenshots/task4_get_check.png)
- Ülesanne 5: [DELETE](screenshots/task5_delete.png) ja [GET 404](screenshots/task5_get_404.png)
- Ülesanne 6: [PUT 404](screenshots/task6_put_404.png)
- Ülesanne 7: [DELETE 404](screenshots/task7_delete_404.png)
- Ülesanne 8: [valideerimine](screenshots/task8_validation.png)
- Ülesanne 10: [testikood](screenshots/task10_test_code.png) ja [PASS](screenshots/task10_pass.png)
- Ülesanne 11: [konsool](screenshots/task11_console.png)
- Lisatest: [bulk-endpointi 404](screenshots/lisatest_bulk_404.png)

Vana nummerdusega Ülesande 12 GUI-pildid säilitati ajalooliste tõenditena,
kuid neid ei esitata lõpliku nummerduse tõendina. Lõpliku tehnilise jooksu
tõend on `outputs/postman_newman_output.txt`.

Üksikasjalik kontroll on failis `SCREENSHOT_CHECKLIST.md`.
