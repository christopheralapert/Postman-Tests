# Postmani ülesanne 6 – ise leitud vigane päring

Valisin päringu `PUT /students/999`, mis proovib muuta olematu ID-ga õpilast.
Päring peab ebaõnnestuma, sest serveri andmetes ei ole õpilast ID-ga 999.
Päris API tagastas staatuse `404 Not Found`.
JSON-vastus `{"error":"Student not found"}` selgitab, et muudetavat õpilast ei
leitud.

Kasutaja peab Postmani GUI-s tegema vigase PUT requesti ja response'i
screenshoti ning lisama selle juurde ülaltoodud analüüsi.
