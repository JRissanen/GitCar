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

Aloitin tekemällä GitCar-nimisen uuden repositoryn. Valistin "public" vaihtoehdon, sekä lisäsin README.md-tiedoston </br> ja GNU General Public License, version 3-lisenssin.

![Screenshot 2022-11-15 162928](https://user-images.githubusercontent.com/116954333/201944757-998acc8b-8981-4536-918b-4e0c20497dbe.png)



__e) Dolly. Kloonaa edellisessä kohdassa tehty varasto itsellesi, tee muutoksia, puske ne palvelimelle, ja näytä, että ne ilmestyvät weppiliittymään.__

Aloitin tekemällä uuden ssh-avaimen komennolla: `ssh-keygen`. </br>
Kun olin luonut avaimen, avasin sen micro-tekstieditorilla ja valitsin koko sisällön ja kopioin sen leikepöydälle, josta se oli helppo siirtää GitHubiin. </br>
Oli tärkeää muistaa valita oikea avain, eli ".pub" päätteinen, eli julkinen avain.</br>
GitHubissa menin siis oman profiilini asetuksiin, josta löytyy "SSH and GPG keys" välilehti, jossa SSH-avaimen voi lisätä. </br>
Nimesin avaimen repositoryn mukaan ja liitin aiemmin micro-tekstieditorilla kopioimani sisällön avimeksi ja painoin lopuksi "Add SSH key" nappia.

![Screenshot 2022-11-15 165145](https://user-images.githubusercontent.com/116954333/202200655-4bb8d7ad-4a62-4d29-8548-d15a21bad31f.png)

Seuraavaksi avasin GitHub repositoryni ja menin kohtaan "Code" ja siinä välilehdelle "SSH". </br>
Tekstikentässä näkyi oman repositoryni osoite, joten kopioin sen. </br>
Sitten kloonasin kyseisen repositoryn Ubuntu vieruaalikoneeni terminaalissa komennolla: `git clone <repositoryn osoite>` </br>

![Screenshot 2022-11-15 170034](https://user-images.githubusercontent.com/116954333/202199959-97b9c733-9c02-4e26-a233-af696a889439.png)

Tämän kappaleen tekstiä kirjoitin virtuaalikoneen terminaalista nano-tekstieditorilla. </br>
Käytin komentoa: `git add . && git commit ; git pull ; git push`, jotta sain muutokset tallennettua ja näkyviin.

![Screenshot 2022-11-16 163937](https://user-images.githubusercontent.com/116954333/202210910-53135f4b-db92-467c-98c1-3e93ea44f3a6.png)

Nyt kun tarkistin vielä repositoryyni tehdyt muutokset, siellä näkyi viimeisimpänä Ubuntu virtuaalikoneellani tekemäni muutokset ja tekijä oli virtuaalikoneella määrittämäni nimi eli "Julius Rissanen", eikä GitHub käyttäjänimeni "JRissanen".

<kbd>
  ![Screenshot 2022-11-16 164115](https://user-images.githubusercontent.com/116954333/202211550-aad3c3c1-6028-4102-8ad2-0ffb067b9f65.png)
</kbd>
