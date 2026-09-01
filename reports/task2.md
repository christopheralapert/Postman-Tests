# Postmani ülesanne 2 – ühe õpilase leidmine

- Päring: `GET http://localhost:3000/students/1`
- HTTP staatus: `200 OK`
- Vastus: üks JSON-objekt, mitte massiiv
- Kontrollitud ID: `1`
- Kontrollitud nimi: `Alice`

Vastus sisaldas õpilase välju `id`, `name`, `age` ja `major`. Collectioni test
kontrollib nii staatust, objekti kuju kui ka ID ja nime vastavust päringule.

Kasutaja peab Postmani GUI-s tegema ühe õpilase requesti ja response'i
screenshoti.
