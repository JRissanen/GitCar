# GitCar
Car repository for Configuration Management Systems exercise

# h3 Git

__b) Offline. Tee paikallinen offline-varasto git:llä. Varaston nimessä tulee olla sana "cat" (kissa). Aiemmin tehty varasto ei siis kelpaa. Aseta itsellesi sähköpostiosoite ja nimi. Näytä varastollasi muutosten teko ja niiden katsominen lokista.__ 

Aloitin tekemällä kansion komennolla: `git init GitCat`. </br>
Sitten siirryin uuteen kansioon ja tein nano-tekstieditorilla README.md-tiedoston: `nano README.md`. </br>
Käytin komentoa: `git add .` lisätäkseni tekemäni muutokset ja komentoa: `git commit` tallentaakseni ne. </br>

Sähköpostin ja nimen sain lisättyä komennoilla: `git config --global user.email "<sähköposti>"` ja </br>
`git config --global user.name "<oma nimi>"`. 

Tarkistin vielä sähköpostin ja nimen komennolla: `git config --global --list`.

Tein vielä lisää muutoksia README.md-tiedostoon nanolla. </br>
Lopuksi tarkistin muutokset komennolla: `git log --patch`.

![Screenshot 2022-11-15 152411](https://user-images.githubusercontent.com/116954333/201936382-ad2be891-cfb3-4039-951a-c254f2a9779a.png)



__c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.__

Lisäsin README.md-tiedostoon tekstipätkän "###Doh! tyhmä muutos". </br>

![Screenshot 2022-11-15 153330](https://user-images.githubusercontent.com/116954333/201940895-6a362c2c-75c5-4a01-995d-a0353cf9ca1c.png)

Sitten käytin komentoa: `git add .` ja  yritin tarkistaa näkyisikö muutos komennolla: `git log --patch`, mutta ei näkynyt, koska en käyttänyt </br>
`git commit` komentoa.

![Screenshot 2022-11-15 153904](https://user-images.githubusercontent.com/116954333/201942850-9ffeeee9-4748-45dc-99d2-0843cad47764.png)

Käytin komentoa `git reset --hard` ja yritin taas tarkistaa näkyisikö muutos komennolla: `git log --patch`, mutta ei näkynyt.
Komento oli kuitenkin poistanut README.md-tiedostosta tekstipätkän "###Doh! tyhmä muutos".

![Screenshot 2022-11-15 153727](https://user-images.githubusercontent.com/116954333/201942927-96b24f1b-f620-4728-9fc6-525e9cceea75.png)



__d) Online. Tee uusi varasto GitHubiin (tai Gitlabiin tai mihin vain vastaavaan palveluun). Varaston nimessä ja lyhyessä kuvauksessa tulee olla sana "car" (auto). Aiemmin tehty varasto ei kelpaa. (Muista tehdä varastoon tiedostoja luomisvaiheessa, suosittelen tekemään README.md ja vapaista lisensseistä itse tykkään GPLv3 eli GNU General Public License, version 3)__

Aloitin tekemällä GitCar-nimisen uuden repositoryn.

![Screenshot 2022-11-15 154756](https://user-images.githubusercontent.com/116954333/201944236-25a8317f-21df-43f5-999a-bdf9cbe16b20.png)

























