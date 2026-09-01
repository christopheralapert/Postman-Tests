# Postmani ülesanne 9 – valideerimine

API nõuab uue õpilase loomisel välju `name`, `age` ja `major`; testpäringust
jäeti `major` teadlikult välja. POST tagastas `400 Bad Request` ja veateate
`{"error":"Invalid data"}` ning järgnev GET kinnitas, et õpilast nimega
`Puudulik Test` ei loodud.

Kasutaja peab Postmani GUI-s tegema puuduliku request Body ja response'i
screenshoti ning lisama juurde ülaltoodud analüüsi.
