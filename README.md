# h3 GIT

# a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.

Tämä tehtävä on tehty markdownilla repositoryyn H3. Tiedostoa README.md on muokattu webbiliittymässä ja tarvittavat kuvat on ladattu H3/h3.

# b) Offline. Tee paikallinen offline-varasto git:llä. Varaston nimessä tulee olla sana "cat" (kissa). Aiemmin tehty varasto ei siis kelpaa. Aseta itsellesi sähköpostiosoite ja nimi. Näytä varastollasi muutosten teko ja niiden katsominen lokista.cd

Luodaan kansio kotihakemistoon ja laitetaan se toimimaan.

``` 
mkdir cat
```
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
- git log 

![Alt text](/h3/h3b.5.png)

Tietysti halutaan nähdä mitä muutoksia on tehty.

- git log --patch

![Alt text](/h3/h3b.4.png)

# c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.

Käydään poistamassa kaikki test.txt teidoston sisältö.

- nano test.txt
- cat text.txt, tiedosto on tyhjä
- git add .
- git status
- git reset --hard
- cat test.txt

![Alt text](/h3/h3c.2.png)

Nähdään että tiedosto on palautunut vanhaan tilaan ja sisältää kaikki sinne lisätyt osat.

# d) Online. Tee uusi varasto GitHubiin (tai Gitlabiin tai mihin vain vastaavaan palveluun). Varaston nimessä ja lyhyessä kuvauksessa tulee olla sana "car" (auto). Aiemmin tehty varasto ei kelpaa. (Muista tehdä varastoon tiedostoja luomisvaiheessa, suosittelen tekemään README.md ja vapaista lisensseistä itse tykkään GPLv3 eli GNU General Public License, version 3)

Käydään ensiksi tekemässä uusi repository https://github.com/Jiikiam/car nimeltä car

![Alt text](/h3/h3d.1.png)

Seuraavaksi tehdään uusi kansio ubuntu serveriin samalla nimellä "car" ja luodaan kansioon README tiedosto.

- git init car
- cd car
- nano README

Kommitataan muutokset. Lisätään githubin url osoite mihin halutaan car kansio ladata. Pushataan ne github repositoryyn.

- git add README
- git commit -m "jotain"
- git git remote add origin https://github.com/username/car.git
- git push -u origin master

Vaatii github käyttäjän ja salasanan. Salasanana toimii nykyään personal access token, joka pitää käydä luomassa. https://www.youtube.com/watch?v=Ff66TqiaIto&ab_channel=RahulWagh

![Alt text](/h3/h3d.2.png)

![Alt text](/h3/h3d.3.png)

Nyt muutokset ovat kaikille näkyvissä.

# e) Dolly. Kloonaa edellisessä kohdassa tehty varasto itsellesi, tee muutoksia, puske ne palvelimelle, ja näytä, että ne ilmestyvät weppiliittymään.

Poistetaan ensin palvelimelle puskettu kansio ubuntulta

- rm -r /home/username/car

Cloonataan kansio githubista

- git clone https://github.com/username/car.git

![Alt text](/h3/h3e1.png)

Muutetaan kansiossa jotain

- nano car/README.md

Pushataan sanmoin kuin kohdassa d), tarkistetaan muuttuiko.

![Alt text](/h3/h3e2.png)

Muutokset menit läpi ja näkyväy githubissa.








