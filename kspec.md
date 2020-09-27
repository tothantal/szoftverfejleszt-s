
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

## 4. Igényelt üzleti folyamatok
* A felhasználó tudjon:
  * az adatbázisból foglalásokat lekérni,
  * szabad szobákat keresni, 
  * szobákat foglalni
  * szobafoglalásokat lemondani
  * megnézni aznapra vonatkozó eseményeket (távozás, érkezés).
  * árakat kiszámolni
 
 
 | függvény | input | output |  transzformáció | megkötések |
|---|---|---|---|---|
| foglalt_leker |  |  | A függvény kiírja a foglalt szobák szobaszámát |  |
| szabad_leker  |  |  | A függvény kiírja a szabad szobák szobaszámát |  |
|  foglal | szobaszam, foglalo_ID |  | A függvény megpróbál lefoglalni egy szobát. | A választott szoba nem lehet foglalt |
| lead | szobaszam, foglalo_ID |  | A függvény megpróbál leadni egy foglalást. | A választott szoba nem lehet szabad, A választott szoba foglaló_ID-je meg kell egyezzen a paraméterben megadott foglalo_ID-vel |
| esemenyek | nap |  | A függvény kiírja az aznapra vonatkozó eseményket | |
| ar_kiszamol | szobaszam | ar | A függvény visszatéríti a választott szoba árát. | |
  

## 5. A rendszerre vonatkozó szabályok
* A rendszer C++ nyelven íródjon, átlátható, későbbiekben bővítésre alkalmas módon. 
* Használjon egy jól kialakított adatbázis modellt, amely naprakészen frissül és nem szolgáltat hibás adatokat. 
* Qt keretrendszerrel könnyen használható, átlátható és igényes GUI felülettel rendelkezzen. 

