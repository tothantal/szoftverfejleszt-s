
# Hotel szoba foglalási rendszer követelményspecifikációja

## 1. Jelenlegi helyzet
A hotel nem régiben nyitott meg, a kevés vendég miatt pedig egy füzetben vezetjük fel, hogy mely szobák foglaltak, hány fővel és milyen szolgáltatást kértek mellé. Ebből a füzetből olvassuk ki azt, hogy aznap milyen vendégek várhatóak, illetve kik fognak távozni. A pénzügyeket, és hogy aktuálisan mely szobák foglaltak vagy szabadok, szintén külön füzetekben írjuk. 

Olyan adatokat írunk fel, mint név, telefonszám, e-mail cím, mettől meddig való tartózkodás, hány fő, hányszori étkezés egy nap, szobaszám és árak. 


## 2. Vágyálom rendszer
A hotel egy megnyert pályázatnak hála jobb marketingeseket tudott fogadni, a fennmaradó összeget pedig egy komplett rendszer kialakítására fordítja. A rendszer feladata legyen, hogy egy adatbázist használva számon tartsa az eddigi foglalásokat, illetve hogy mely szobák szabadok még. Legyen olyan menüpont is, ami felsorolja, hogy aznap mely szobákból távoznak, és melyekbe érkeznek vendégek. 

---
* Az alkalmazás legyen könnyen értelmezhető és használható.
* Adatbázissal lehessen nyomon követni, hogy az egyes időintervallumokban milyen szobák szabadok még. 
* Azonnal visszajelzést biztosítson a dolgozónak a sikeres vagy sikertelen foglalásról.
* Le lehessen követni, hogy aznap mely szobákból távoznak és melyekbe jönnek vendégek. 


## 3. Jelenlegi üzleti folyamatok
* Foglalások felírása
* Foglalások lemondása
* Árak kiszámolása


## 4. Igényelt üzleti folyamatok
* A felhasználó tudjon:
  * az adatbázisból foglalásokat lekérni,
  * szabad szobákat keresni, 
  * megnézni aznapra vonatkozó eseményeket (távozás, érkezés).


## 5. A rendszerre vonatkozó szabályok
* A rendszer C++ nyelven íródjon, átlátható, későbbiekben bővítésre alkalmas módon. 
* Használjon egy jól kialakított adatbázis modellt, amely naprakészen frissül és nem szolgáltat hibás adatokat. 
* Qt keretrendszerrel könnyen használható, átlátható és igényes GUI felülettel rendelkezzen. 


## 6. Követelménylista
| Modul | ID | Név |  V. | Megjegyzés |
|---|---|---|---|---|
|  | K1 | Foglalás | 1.0 | A felhasználó tudjon foglalásokat leadni adott szobákra a megfelelő adatokkal. Ha a választott szoba foglalt, a foglalás sikertelen, és ezt jelezze is. Ha a szoba szabad, és minden adatot helyesen töltött ki, akkor a foglalás elfogadását mutassa, és helyezze el az adatbázisban. |
|   | K2 | Szabad szobák | 1.0 | Még foglalás előtt a felhasználó tudja megnézni, hogy mely szobák azok, amik az adott időintervallumban még szabadok. |
|   | K3 | Mai események | 1.0 | Le lehessen kérni, hogy milyen események fognak aznap történni. A távozásokat és az érkezéseket egyaránt nyomon lehessen követni, és kipipálni, ha már megtörtént. |
