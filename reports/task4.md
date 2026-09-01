# Postmani ülesanne 4 – õpilase muutmine

Muudetud õpilane oli Ülesandes 3 loodud Katrin Kask, kelle kontrollkäivituse ID
oli `4`.

Muudeti kaks välja:

- `age`: `20` → `21`
- `major`: `Computer Science` → `Mathematics`

PUT `/students/4` tagastas `200 OK` ja uuendatud objekti. Järgnev eraldi GET
`/students/4` tagastas samuti `200 OK` ning vastuses olid vanus 21 ja eriala
Mathematics. See kinnitas, et mõlemad muudatused säilisid serveri mälus.

Collection kasutab fikseeritud ID asemel Ülesande 3 muutujat
`createdStudentId`.

Kasutaja peab Postmani GUI-s tegema PUT requesti ja response'i ning GET
kontrollpäringu ja response'i screenshotid.
