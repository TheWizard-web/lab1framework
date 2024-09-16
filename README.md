# Laboratorul nr.1. Bazele HTTP

## Sarcini laborator

### Sarcina 1. Analiza cererilor HTTP

1. Accesați site-ul http://sandbox.usm.md/login.
  - Rezultat
![Accesare site](/imagini/rasp1.jpg)

2. Deschideți fila Network în instrumentele pentru dezvoltatori ale browserului.
  - Rezultat
  ![Fila Network](/imagini/rasp2.jpg)

3. Introduceți date incorecte pentru autentificare (de exemplu, username: student, password: studentpass).
  - Rezultat
  ![Autentificare date incorecte](/imagini/rasp3.jpg)

4. Analizați cererile care au fost trimise către server.
  - Rezultat
  ![Cererea trimisa catre server : POST(Creaza o noua resursa pe server.)](/imagini/rasp4.jpg)

5. Răspundeți la următoarele întrebări:

  - Ce metodă HTTP a fost utilizată pentru a trimite cererea?
    - _Pentru a trimite cererea a fost utilizata metoda HTTP POST._
  - Ce anteturi au fost trimise în cerere?
    - ![Request Headers](/imagini/rasp5.jpg)
  - Ce parametri au fost trimiși în cerere?
    - ![Parametri cerere](/imagini/rasp6.jpg)
  - Ce cod de stare a fost returnat de server?
    - _De server a fost returnat cod-ul de stare 401(Autentificarea utilizatorului este necesara)._
    - ![Cod de stare](/imagini/rasp7.jpg)
  - Ce anteturi au fost trimise în răspuns?
    -![Response Headers](/imagini/rasp8.jpg)

6. Repetați pașii 3-5, introducând date corecte pentru autentificare (username: admin, password: password).

  - Listing-ul sarcinei :

    - _Autentificarea cu date corecte._
    - _Analiza cererilor trimise catre server (cerere de tip POST)._
    - _Metoda HTTP utilizata pentru a trimite cererea (metoda POST)._
    - ![ScreenshotDescriptiv1](/imagini/photo1.jpg)
    - _Antenturi trimise in cerere._
    - ![ScreenshotDescriptiv2](/imagini/photo2.jpg)
    - _Parametri cerere._
    - ![ScreenshotDescriptiv3](/imagini/photo3.jpg)
    - _Cod de stare returnat de server (200 OK)._
    - _Antenturi trimise in raspuns._
    - ![ScreenshotDescriptiv4](/imagini/photo4.jpg)

### Sarcina 2. Crearea cererilor HTTP 

1. Scrieți o cerere de tip GET către server la adresa http://sandbox.com, indicând în antetul User-Agent numele și prenumele dvs.

2. Scrieți o cerere de tip POST către server la adresa http://sandbox.com/cars, indicând în corpul cererii următorii parametri:

   - `make: Toyota`
   - `model: Corolla`
   - `year: 2020`

3. Scrieți o cerere de tip PUT către server la adresa http://sandbox.com/cars/1, indicând în antetul User-Agent numele și prenumele dvs., în antetul Content-Type valoarea application/json, iar în corpul cererii următorii parametri: 
    
  - `json { "make": "Toyota", "model": "Corolla", "year": 2021 }`
   
4.  Scrieți unul dintre posibilele răspunsuri ale serverului la cererea anterioară. 

http POST /cars HTTP/1.1 Host: sandbox.com Content-Type: application/json User-Agent: John Doe model=Corolla&make=Toyota&year=2020 

Presupuneți situațiile în care serverul poate returna codurile de stare HTTP 200, 201, 400, 401, 403, 404, 500.

5. Scrieți o cerere de tip DELETE la alegerea dvs. și să explicați de ce, în acest caz, este potrivit să utilizați metoda DELETE.

### Sarcina 3. Sarcina Suplimentara. HTTP_Quest

1. Trimiteți o cerere de tip POST către server la adresa http://sandbox.usm.md/quest, indicând în antetul User-Agent numele și prenumele dvs. 

(De exemplu, User-Agent: John Doe). 

http POST /quest HTTP/1.1 Host: sandbox.usm.md User-Agent: John Doe curl: bash curl -X POST http://sandbox.usm.md/quest -H "User-Agent: John Doe"

2. Urmați instrucțiunile de pe server, îndeplinindu-le în ordine.

3. La finalul quest-ului, vi se va afișa un cuvânt secret, pe care va trebui să-l includeți în raport.

