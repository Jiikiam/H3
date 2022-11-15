# h3 GIT

a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.

-

b) Offline. Tee paikallinen offline-varasto git:llä. Varaston nimessä tulee olla sana "cat" (kissa). Aiemmin tehty varasto ei siis kelpaa. Aseta itsellesi sähköpostiosoite ja nimi. Näytä varastollasi muutosten teko ja niiden katsominen lokista.cd

Luodaan kansio kotihakemistoon ja laitetaan se toimimaan.

- mkdir cat
- git init cat

Määritetään meidän github käyttäjän tiedot, koska github vaatii sitä ensimmäisellä kerralla.
  
- git config --global user.name "user_name"
  
- git config --global user.email "email"

Luodaan varastoon tiedosto test.txt ja tallennetaan sinne jotain.

- cd cat
- nano test.txt

Ajetaan muutokset läpi

- git add test.txt
- git commit -m "test"

Nyt tiedosto test.txt on tallettu gittiin. Käydään tekemässä muutoksia kansioon.

- nano test.txt

Tehdään uusii commit ja katsotaan onko tiedostossa tehty muutosksia

- git commit -m "test1"

![Alt text](/h3/h3b.5.png)

- git log 

![Alt text](/h3/h3b.5.png)

Tietysti halutaan nähdä mitä muutoksia on tehty.

- git log --patch

![Alt text](/h3/h3b.4.png)

c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

Käydään poistamassa kaikki test.txt teidoston sisältö.

- nano test.txt
- cat text.txt, tiedosto on tyhjä
- git add .
- git status
- git reset --hard
- cat test.txt

![Alt text](/h3/h3c.2.png)

Nähdään että tiedosto on palautunut vanhaan tilaan ja sisältää kaikki sinne lisätyt osat.



