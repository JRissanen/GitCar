# GitCar
Car repository for Configuration Management Systems exercise

# h3 Git

__b) Offline. Tee paikallinen offline-varasto git:llä. Varaston nimessä tulee olla sana "cat" (kissa). Aiemmin tehty varasto ei siis kelpaa. Aseta itsellesi sähköpostiosoite ja nimi. Näytä varastollasi muutosten teko ja niiden katsominen lokista.__ 

Aloitin tekemällä kansion komennolla: `git init GitCat`. </br>
Sitten siirryin uuteen kansioon ja tein nano-tekstieditorilla README.md-tiedoston: `nano README.md`. </br>
Käytin komentoa: `git add .` lisätäkseni tekemäni muutokset ja komentoa: `git commit` tallentaakseni ne. </br>

Sähköpostin ja nimen sain lisättyä komennoilla: `git config --global user.email "<sähköposti>"` ja `git config --global user.name "<oma nimi>"`. </br>
Tarkistin vielä sähköpostin ja nimen komennolla: `git config --global --list`.

Tein vielä lisää muutoksia README.md-tiedostoon nanolla. </br>
Lopuksi tarkistin muutokset komennolla: `git log --patch`.

![Screenshot 2022-11-15 152411](https://user-images.githubusercontent.com/116954333/201936382-ad2be891-cfb3-4039-951a-c254f2a9779a.png)


__c) Doh! Tee tyhmä muutos gittiin, älä tee commit:tia. Tuhoa huonot muutokset ‘git reset --hard’. Huomaa, että tässä toiminnossa ei ole peruutusnappia.__
