# Postmani ülesanne 5 – õpilase kustutamine

Kustutati Ülesandes 3 loodud õpilane Katrin Kask, kelle ID oli selles
kontrollkäivituses `4`.

- DELETE `/students/4`: `200 OK`
- DELETE vastus: `{"message":"Student deleted"}`
- Järgnev GET `/students/4`: `404 Not Found`
- Kontroll-GET vastus: `{"error":"Student not found"}`

404 kontroll ja veateade kinnitasid, et õpilast ei olnud pärast kustutamist enam
API-s. Collection kasutab ID jaoks muutujat `createdStudentId`.

Kasutaja peab Postmani GUI-s tegema DELETE requesti ja response'i ning
kontrollpäringu ja response'i screenshotid.
