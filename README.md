# QtUIharjoituksia
Työpöytäsovellusten luominen QT Designer -ohjelmalla ja Python-kielellä. Harjoituksessa luodaan seuraava käyttöliittymä, jonka avulla harjoitellaan tiedoston käsittelyä, kuvan muokkausta ja tulostamista. 

![image](https://user-images.githubusercontent.com/24242044/173568229-3306546c-1157-4d33-8bfe-a340ac0bbfc4.png)

Käyttöliittymässä on kentät opiskelijan nimen ja opiskelijanumeron syöttämistä varten. Näiden tietojen perusteella muodostetaan tulostettava opsikelijatarra, jossa opiskelijanumero on viivakoodina. Sovellukseen voidaan ladata opiskelijan kuva. Sen skaalausta voidaan muuttaa ja muuttaa kuvasta näkyvää aluetta liukusäätimien avulla. Ohjelman asetuksissa voidaan määritellä paikkamerkkikuva, jota käytetään. Sovelluksen mukana tulee 2 kuvaa: `placeholder.png` ja `placeholder2.jpg`.

Sovellus koostuu useammasta tiedostosta ja se hyödyntää QT5:n Python kirjastoja. Pääohjelma on `opiskelijatarra.py` ja sen käyttöliittymä on määritelty tiedostossa `opiskelijatarra.ui`. Sovellus tarvitsee toimiakseen joitakin Pythonin sisäänrakennettuja kirjastoja sekä erillisen modulin `code128Bcode.py`, jonka avulla muodostetaan viivakoodit. Viivakoodit käyttävät `Libre Code 128` viivakoodifonttia, joka on asennetava tietokoneeseen, jotta tarrat tulostuisivat halutulla tavalla.

Harjoituksessa luodaan jakelupaketti ja asennusohjelma sovellukselle. Jakelu luodaan `PyInstaller`-ohjelman avulla. Osa sovelluksen käyttämistä tiedostoista on määriteltävä `spec`-tiedostoon, jotta jakeluun saadaan kaikki sovelluksen tarvitsemat tiedostot. Sovelluksen käyttämät kirjastot, modulit ja muut tiedostot ilmenevät seuraavasta kaaviosta:


![Modulikaavio drawio](https://user-images.githubusercontent.com/24242044/173565805-f2753b71-478e-41c9-af56-f56eb65d0568.png)
