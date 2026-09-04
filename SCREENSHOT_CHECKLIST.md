# Postmani GUI screenshotide kontrollnimekiri

Need GUI screenshotid tegi kasutaja käsitsi. Piltide sisu kontrolliti enne
repo `screenshots/` kausta kopeerimist; ühtegi pilti ei genereeritud.

## Ülesanne 1

- [x] [GET `/students` ja 200 response](screenshots/task1_get_all.png), kus on
  näha kolm õpilast ning väljad `id`, `name`, `age`, `major`.

## Ülesanne 2

- [x] [GET `/students/1` ja ühe õpilase response](screenshots/task2_get_one.png).

## Ülesanne 3

- [x] [POST `/students` ja 201 response](screenshots/task3_post.png).
- [x] [Loodud õpilase GET-kontroll ja response](screenshots/task3_get_check.png).

## Ülesanne 4

- [x] [PUT Body ja response kahe muudetud väljaga](screenshots/task4_put.png).
- [x] [GET-kontroll säilinud muudatustega](screenshots/task4_get_check.png).

## Ülesanne 5

- [x] [DELETE ja edukas response](screenshots/task5_delete.png).
- [x] [Kustutamise GET-kontroll ja 404 response](screenshots/task5_get_404.png).

## Ülesanne 6

- [x] [Vigane PUT `/students/999` ja 404 response](screenshots/task6_put_404.png).
- Screenshot või tekst 3–5-lauselise analüüsiga failist `reports/task6.md`.

## Ülesanne 7 – BLOCKED

- [x] [POST `/students/bulk` ja 404 `Cannot POST /students/bulk`](screenshots/task7_blocked.png).
- Tõend või tekst, et õpetaja `app.js` failis bulk-endpoint puudub.
- Ülesannet ei tohi näidata PASS-ina.

## Ülesanne 8

- [x] [DELETE `/students/999` ja 404 response](screenshots/task8_delete_404.png).
- Screenshot või tekst vastustega kolmele küsimusele failist
  `reports/task8.md`.

## Ülesanne 9

- [x] [Puudulik POST Body ja 400 `Invalid data` response](screenshots/task9_validation.png).
- Screenshot või tekst 2–3-lauselise analüüsiga failist `reports/task9.md`.

## Ülesanne 10

- [x] [Tests tab koos nõutud testikoodiga](screenshots/task10_test_code.png).
- [x] [Test Results PASS tulemus](screenshots/task10_pass.png).

## Ülesanne 11

- [x] [Postman Console `Keskmine vanus: 23` ja PASS tulemus](screenshots/task11_console.png).

## Ülesanne 12

- [x] [Ühe `Students API` collectioni ülevaade](screenshots/task12_collection.png).
- [x] [Collection Runner: 16 testi, 0 viga ja Ülesanne 7 eraldi 0/0](screenshots/task12_runner.png).
- Collection JSON peab jääma reposse faili
  `postman/Students_API.postman_collection.json`.
