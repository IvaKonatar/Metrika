U zadataku sam izracunala sledece metrike:
Sva tri fajla imaju ukupno 235 linija. 
Fajl kalkulator ima ciklomatsku i kognitivnu slozenost 11
Fajl start ima ciklomatsku i kongitivnu slozenost 2. 

Analizom fajla kalkulator dosla sam do sledecih zakljucaka:
Metoda ToString() u klasi Operations bi mogla biti preimenovana da bolje odražava njen zadatak, na primer, getOperationSymbols()
Trenutno se koristi opšti catch blok za hvatanje bilo kakvih izuzetaka pri parsiranju brojeva. Specifičniji tretman grešaka bi poboljšao razumevanje i otklanjanje problema.
Zatvaranje Scanner objekta unutar petlje može dovesti do problema ako se System.in koristi negde drugde. Bolje bi bilo zatvoriti Scanner van petlje ili koristiti try-with-resources za automatsko zatvaranje.


Analizom fajla start dosla sam do sledecih zakljucaka:
Resursi za skeniranje:Umesto petlje while, možemo kreirati jedan Scanner izvan petlje i koristiti ga unutar petlje.
Proveravanje stringa za izlaz: Možda bi bilo čitljivije koristiti equalsIgnoreCase() metodu kako bi se izbjeglo bilo kakvo slučajno razlikovanje u unosu.
Zatvaranje skenera: To bi se moglo postići pomoću try-with-resources konstrukta.
