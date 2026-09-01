# Postmani ülesanne 8 – olematu õpilase kustutamine

Päring: `DELETE http://localhost:3000/students/999`

1. HTTP staatus oli `404 Not Found`.
2. API ei tagastanud õpilast, vaid JSON-veateate
   `{"error":"Student not found"}`.
3. Veateade tähendab, et serveri andmetes ei olnud ID-ga 999 õpilast, keda
   kustutada.

Collectioni test kontrollib nii 404 staatust kui täpset veateadet.

Kasutaja peab Postmani GUI-s tegema DELETE `/students/999` requesti ja
response'i screenshoti.
