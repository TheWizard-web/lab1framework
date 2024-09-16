# Laboratorul nr.1. Bazele HTTP

## Sarcini laborator

### Sarcina 1

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
  ![Cererea trimisa catre server : POST](/imagini/rasp4.jpg)

5. Răspundeți la următoarele întrebări:

  - Ce metodă HTTP a fost utilizată pentru a trimite cererea?
    - _Pentru a trimite cererea a fost utilizata metoda HTPP POST._
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

  