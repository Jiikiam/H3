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

Luodaan varastoon tiedosto test.txt ja tallennetaan se tyhjänä.

- cd cat
- nano test.txt

Ajetaan muutokset läpi

- git add test.txt
- git commit -m "test"

Nyt tiedosto test.txt on tallettu gittiin. Käydään tekemässä muutoksia kansioon.

- nano test.txt

![Alt text](/h3/h3b.1.png)


![Alt text](/h3/h3b.2.png)

c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.




