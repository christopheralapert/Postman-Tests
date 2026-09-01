# Postmani ülesanne 3 – uue õpilase loomine

Loodud õpilane:

- Nimi: `Katrin Kask`
- Vanus: `20`
- Eriala (`major`): `Computer Science`
- Serveri määratud ID selles kontrollkäivituses: `4`

POST `/students` tagastas `201 Created` ja loodud õpilase JSON-objekti. Seejärel
tehtud eraldi GET `/students` tagastas `200 OK`; vastuse massiivist leiti sama
ID, nime, vanuse ja erialaga õpilane. Seega ei põhine kinnitus ainult POST-i
vastusel.

Collection salvestab POST-vastuse ID muutujasse `createdStudentId` ja kasutab
seda eraldi GET-kontrollpäringus.

Kasutaja peab Postmani GUI-s tegema POST requesti ja response'i ning GET
kontrollpäringu ja response'i screenshotid.
