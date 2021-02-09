# Tiivistetty vaatimusmäärittely

* [SIJOITA TOIMEKSIANNON NIMI TÄHÄN] 
* Projektimäärittely/vaatimusmäärittelyn tiivistetty versio v 0.3 4.1.2021 (NarsuMan)

__Ohjeita ennen aloitusta :)__

**Olet editoimassa tiivistettyä vaatimusmäärittelyä, joka on normaalia OPF:n laajempaa [vaatimusmäärittelyä](vaatimusmaarittely-laaja.md) rajatumpi. Kannattaa tutustua ehdottomasti laajempaan vaatimusmäärittelyyn, koska se sisältää ohjeistuksen lisäksi videomateriaalia.**



## Johdanto

![](../assets/work-to-do.png)

Projektin tavoitteena on kehittää parempia ohjelmistoja niitä tarvitseville asiakkaille. Nykyaikana ohjelmistot ovat tärkeässä roolissa eri työpaikoilla ja yksityisyrityksissä, jossa tarvitaan tietotekniikkaa. Paremmat ohjelmistot mahdollistavat tehokkaamman työn ja sitä kautta paremman menestyksen yrityksille.



## Tavoitteet 

Tavoitteena rakentaa toimivat ohjelmistopaketit asiakkaille tarpeisiin. Eri käyttöön soveltuvat ja toimivat ohjelmistot ovat tavoitteena tehdä sekä ratkaista asiakkaiden ongelma räätälöidyllä ohjelmistopaketilla.

## Kohderyhmä

Kohderyhmiä ovat isot ja pienemmät yritykset, yksityisyrittäjät. Kaikki yritykset, jossa tarvitaan tietotekniikkaa arjessa ja erilaisia ohjelmistoja toiminnan ylläpitämiseksi ovat asiakkaita.

## Sidosryhmäkartta

![](../assets/work-to-do.png)

>Mietitään tarkemmin millaisia käyttäjä/sidosryhmiä liittyy suunniteltuun ratkaisuun/ohjelmistoon/palvelukokonaisuuteen? 
Näitä selkeyttääksemme kirjataan kaikki sidosryhmät sidosryhmäkartan muotoon. Nostetaan samalla esiin mikä on 
ko. sidosryhmän/edustajan palveluun liittyvä motivaatio. Kuvauksen voi laatia esim. piirtämällä, MindMap-muodossa tai soveltaen sopivaa UML-notaatiota.

> Voit tutustu nyt aiemmin mainittuun PlantUML-työkaluun ja kokeilla luoda sidosryhmäkartta käyttäen (http://plantuml.com/)
> Huomaa! PlantUML-lohkon määrittelyssä käytetään Gitlab-ympäristössä eri avainsanoja @startuml/@enduml- rivien sijaan  

```plantuml
@startmindmap
+ Projektin tuotos
++ Asiakas
+++ Yritykset
+++ yksityisyrittäjät
++ Kilpailevat valmistajat
+++ IT-toimijat
+++ Asiakkaan yhteystyökumppanit
-- Ohjelmistojen jälleenmyyjä
--- Ohjelmistojen oikeuksien myyjät
--- Nettisivustot 
-- Omat yhteistyökumppanit
--- Sijoittajat
@endmindmap
```

**Tarkennettut sidosryhmäprofiilit** 

![](../assets/work-to-do.png)

> Kuvataan tarkemmin sidosryhmäkartasssa esiteltyhä sidosryhmiä/profiileja. Tarvittaessa kuvataan tarkemmin valitut sidosryhmät ja tarkennetaan niitä, jos toimeksianto sitä edellyttää. Tähän sovelletaan alisivuja, joita tarpeen mukaan kopioidaan "pohjat"-kansiosta Katso esim. **Asiakas B**

| ID | Tyyppi | Nimi | Piirteet |  Motivaatio |
|:-:|:-:|:-:|:-:|:-:|
| SR-001 | Sidosryhmä/Profiili | Asiakas A | Isot yritykset| Tarvitsee paljon palvelua eritarkoituksiin  |
| SR-002 | Sidosryhmä/Profiili | [Asiakas B - Profiili 1 ](pohjat/pohja-profiilikuvaus.md) | yksityisyrittäjät| Yleinen asiakas, mutta tuotteen tilausmäärät pienemmät pienemmästä tarpeesta johtuen|
| SR-003 | Sidosryhmä/Profiili | Asiakas C | Yksittäiset asiakkaat | Pieni ja satunnainen tarve |
| SR-004 | Sidosryhmä/Profiili | yhteistyökumppanit | jälleenmyyjä| Mainostaa ja jälleenmyydä tuotetta |
| SR-005 | Sidosryhmä/Profiili | Sijoittajat |sijoittaja| Tukee ja sijoittaa tuotteeseen rahallisesti |

## Palveluun liittyviä asiakaspolkuja

> Mieti toimeksiantoa ja pohdi onko siitä tunnistettavissa ns. palvelupolkuja? 
> Asiaspolkukuvauksen avulla kuvataan tapahtuma sarjaa joka käydään jossain valitussa tilanteessa läpi palvelun käytön aikana. 
> Asiakas kohtaisia palvelupolkuja voi olla useita, mutta tärkeintä on tunnistaa alkuvaiheessa oleellisimmat. 
> Palvelupolkua kuvattaessa voi hyödyntää esim. Swim lane/BluePrint/tilakone-kuvausta tai muuta sopivaksi katsottua kuvausta.
> Tärkeää on kuitenkin kuvata polku ja käyttää sitä tarvittaessa selkeyttämään ymmärrystä tavoitellusta palvelusta. 
> Käy läpi tekemäsi kuvausta jonkun toisen henkilön kanssa yhdessä? Käy läpi polku ja kerro mitä sen aikana tapahtuu..

**asiakaspolku PlantUML-esimerkki tilakoneena**

> Kokeillaan luonnostella asiakaspolkua PlantUML-työkalun avulla. Kannattaa kokeilla ehdottomasti myös muita tapoja! 
> Sovella esim. PlantUML SDL/Swimlane kuvausta?

```plantuml

Step1: Palvelun kuvaus mainosnäytöllä 
Step2: Asiakas astuu ovesta sisään 
Step3: Palveluun tutustuminen sisätiloissa
Step4: Asiakas kysyy myyjää
Step5: Myyjä esittelee tuotteen
Step6: Asiakas pohdiskelee asiaa
Step7: Asiakas tekee sopimuksen
Step8: Asiakas ei ota tuotettava
Step9: Myyjä suosittelee lisäpalveluita
Step10: Jne
Step11: Asiakas poistuu paikalta

[*] --> Step1
Step1 --> Step2
Step2 --> Step3
Step3 --> Step6
Step3 --> Step4
Step4 --> Step5
Step5 --> Step6
Step6 --> Step7
Step6 --> Step8
Step8 --> Step11
Step7 --> Step9
Step9 --> Step10

```

### Käyttöliittymänäkymä/mockup 

![](../assets/work-to-do.png)

> Jos projektin tuloksena tuo sähköinen ratkaisu, on sen konkretisoimiseksi hyvä hyödyntää esimerkiksi MockUp-kuvaa.
Tähän kannattaa liittää tarvittaessa kuvausta kuvan/mockup-näkymän muodossa. Se helpottaa ymmärtämään tarvittaessa oleellisesti tavoiteltua ratkaisua. 

```plantuml
salt
{
  Just plain text
  [This is my button]
  ()  Unchecked radio
  (X) Checked radio
  []  Unchecked box
  [X] Checked box
  "Enter text here   "
  ^This is a droplist^
}
```


## Tärkeimmät toiminnallisuudet/ominaisuudet

![](../assets/work-to-do.png)

> Hahmotellaan tähän kohtaan ominaisuudet pelkästään ranskalaisilla viivoilla ja MindMap-kuvauksen avulla. Eli mitä tavoitellulla ratkaisulla/palvelulla mielestäsi on mahdollista tehdä? 
> Mieti tilannetta, kun joku kysyy sinulta mitä palvelulla voi tehdä? Saat aikaa vastata 15 sekuntia. Mitä vastaat ja mitkä toiminnot nostatat esiin ehdottomasti valtteina verrattuna muihin vastaaviin ratkaisuihin/palveluihin?
> Tässä kohtaa kannattaa tarkistaa mitä olivat asiakkaan esittämät toiveet palvelusta? Niistä voisi löytyä ehkä joitain tässä vaiheessa?


- Oleelliset toiminnot (Esimerkkejä) 
    - Asiakas_A voi lähettää postia toiselle henkilölle
    - Asiakas_A voi saada tietoa aiemmin tehdyistä valinnoista
    - Ylläpito-henkilö voi poistaa laskun Asiakaalta
    - Ylläpito-henkilö voi luoda uuden laskun Asiakkaalle 
    - Asiakas_A voi soittaa tuntemalleen kaverille
    - Asiakas_B voi jakaa kuvan
    - Asiakas_B kykenee tallettamaan tilanteen
    - Asiakas_B voi liittää Asiakkaan_A ryhmään uuden henkilön
    - etc..



```plantuml
@startmindmap
+ Tuote, eli tuotettava ratkaisu
++ Toiminnallisuus A
+++ Toiminto 1
+++ Toiminto 2
++ Toiminnallisuus B
+++ Toiminto 3
+++ Toiminto 4
-- Toiminnallisus C - Viestin suojaus
--- Toiminto 5 - Suojauksen valinta
--- Toiminto 6 - Suojauksen vaihto
-- Toiminnallisuus D - Viestintä
--- Toiminto 7 - Viestin lähetys
--- Toiminto 8 - Viestin kuittaus
@endmindmap
```



## Alustavat käyttäjätarinat

![](../assets/work-to-do.png)

> Ketterän kehityksen myötä on yleistynyt tapa kuvata asiakkaan tarpeita ns. käyttötarinoiden (User Story) muodossa. Kirjataan tähän ennalta tunnistetut käyttötarinat. 

| ID | Tyyppi | Kuvaus | Linkki |
|:-:|:-:|:-:|:-:|
| US-001 | Käyttäjätarina | Esim. Käyttäjänä haluan, että voin luoda raportin tekemistäni ostoista viimeisen kuukauden ajalta, koska se helpottaa oman talouteni hallintaa | #1 |
| US-002 | Käyttäjätarina | Esim. Käyttäjänä haluan, että voin poistaa historian tekemistäni ostoista viimeisen kuukauden ajalta, koska en halua muistella menneitä | #2 |

## Yleiset tekniset vaatimukset

> Teknisiä ratkaisuja määriteltäessa on hyvä tunnistaa tarvittavat teknologiat, laitteistot tai muut tarvittavat fyysiset ratkaisut. 
Ohjelmiostoratkaisuja määriteltäessä kannattaa erottaa puhtaasti tekniset/tuotannolliset vaatimukset ja kirjata ne vaatimusmäärittelyyn esimerkiksi teknisinä vaatimuksina. 

| ID | Tyyppi | Kuvaus | 
|:-:|:-:|:-:|
| HWREQ-0002 | Tekniset vaatimukset | Palvelun tärkeimpien palvelujen on oltava vähintään kahdennettu N+1 | |
| HWREQ-0003 | Tekniset vaatimukset | Palvelimen muistikapasiteeti >32GB  ||
| HWREQ-0005 | Tekniset vaatimukset | Palvelimen fyysinen sijainti on oltava EU-aluella| |
| HWREQ-0005 | ... | ... ||

# Toiminnalliset vaatimukset (Functional Requirements)

>Mitä toimintoja palveluun liittyy? Nämä kannattaa kirjata ensi ns. toiminnallisina vaatimuksina? Toiminnallisilla vaatimuksilla kuvataan ohjelmistolta/järjestelmältä vaadittuja toimintoja.
Toiminnalliset vaatimukset ovat helpoimmin tunnistettavia. Vältä useamman vaatimuksen kirjaamista samaan lauseeseen! Jokainen vaatimus erikseen.

| ID | Tyyppi | Kuvaus | Toiminnallisuus johon vaatimus vaikuttaa |								
|:-:|:-:|:-:|:-:|
| FUNCREQ-C0001 | Toiminnallinen vaatimus | Krjautumiseen voi käyttää Facebook-tunnuksia | [Toiminnallisuus X](pohjat/pohja-ominaisuus.md) |
| FUNCREQ-C0002 | Toiminnallinen vaatimus | Käyttöliittymää voidaan ohjata äänikomennoilla | [Toiminnallisuus Y](pohjat/pohja-ominaisuus.md) |
| FUNCREQ-C0003 | Toiminnallinen vaatimus | ... | ... |

# Laadulliset eli ei-toiminnalliset vaatimukset

>Mitä olivat ei-toiminnalliset vaatimukset? Voit esittää eri vaatimuksia erillisessä taulukossa tai viitata tässä [yhteen](pohjat/pohja-vaatimuslistalle.md) laajempaan taulukkoon.
[Ei-toiminnalliset vaatimukset](https://en.wikipedia.org/wiki/Non-functional_requirement) sisältää laajan joukko eri näkökulmia sähköiseen palveluun liittyen. Tärkeimmät kirjoittajan 
näkökulmasta ovat seuraavat: Suorituskyky, tietoturva ja saavutettavuus 

* Suorituskyky
* Tietoturva
* Saavutettavuus

## Suorituskykyyn liittyvät vaatimukset

![](../assets/work-to-do.png)

>Millaisia vaatimuksia palveluun kohdistuu suorituskyvyn näkökulmasta?

| ID | Tyyppi | Kuvaus |
|:-:|:-:|:-:|
| PERFREQ-0000 | Suorituskyky | Kirjautuminen on mahdollista yhtäaikaa 100 käyttäjällä (100 request/s) |					
| PERFREQ-0001 | Suorituskyky | Palvelun maksimi käyttäjä määrä on ? |
| PERFREQ-0002 | Suorituskyky | ... ||

## Tietoturvan vaatimukset

![](../assets/work-to-do.png)

>Millaisia vaatimuksia palveluun kohdistuu tietoturvan näkökulmasta?

| ID | Tyyppi | Kuvaus | Miten testataan? |
|:-:|:-:|:-:|:-:|
| SECURITY-REQ-0001 | Salasanassa on käytettävä vähintään MD5-tason salausta, koska [CONSTRAIN-000]() sitä edellyttää | [Testitapaus X]() |
| SECURITY-REQ-0002 | Jokainen tapahtuma palvelussa on kirjattava käyttölogiin, että niitä voidaan tarkastella myöhemmin | [Testitapaus Y]() |
| SECURITY-REQ-0003 | ... | ... |

## Saavutettavuuden vaatimukset

![](../assets/work-to-do.png)

>Mitä tarkoitetaan saavutettavuudella? Millaisia asioita/ohjeistuksia on otettava huomioon palvelua toteutettaessa?
Tutustu [saavutettavuusdirektiiviin](https://saavutettavuusdirektiivi.fi/saavutettavuus-verkkopalveluissa/) ja kirjaa  

| ID  | Luokka | Kuvaus | Miten testataan? |
|:-:|:-:|:-:|:-:|
| AVAILREQ-0000 | Saavutettavuus | | [Testit]() |	
| AVAILREQ-0001 | Saavutettavuus | | [Testit]() |
| AVAILREQ-0002 | Saavutettavuus | ... | ... |

### Toimeksiannon kannalta tärkeät oleelliset rajaukset

> Eri ohjelmistojena/palvelujen toteutusta ja käyttöä ohjaavat usein lait ja säädökset. Näiden edellyttämät vaatimukset voidaan kirjataan tarvittaessa vaatimusmäärittelyyn.
Rajausten vaikutus koskee usein palvelun jonkin osa-kokonaisuuden toteuttamista. Tästä syystä eri rajoitteet on tunnistettava ajoissa, koska vaikutus 
saataa olla varsin ratkaiseva pitemmällä tähtäimella. Esimerkkinä tästä on viime vuonna voimaan tullut [EU GDPR-säädös](https://en.wikipedia.org/wiki/General_Data_Protection_Regulation).
> Kannattaa tutkia esimerkiksi https://www.sfs.fi/aihealueet/terveydenhuolto/laakinnalliset_laitteet tai http://docs.jhs-suositukset.fi/jhs-suositukset/JHS190/JHS190.html

| ID | Tyyppi | kategoria | Vastuullinen |
|:-:|:-:|:-:|:-:|
| CONSTRAIN-000  | Rajaus | Palvelun kirjautumisprosessin on noudatettava JUHTA-hyväksyttyjä käytänteitä  | [Kirjautuminen ft1](pohjat/pohja-ominaisuus.md) |
| CONSTRAIN-001 | Rajaus | On huomioitava Standardi ZZZ osana palvelun tapahtuma login talletusta | [Log-palvelin](pohjat/pohja-ominaisuus.md)|
| CONSTRAIN-002 | Rajaus | ... | ... |

### Palvelun tuotantoympäristö

> Vaatimusmäärittelyn tukena sovelletaan erilaisia kuvauksia, joista esimerkkinä UML-kuvauskieleen liittyvä sijoittelu näkymä, eli "Deployment Diagram", kuvauksen avulla voi esittää miten palvelu on tarkoitus toteuttaa käytännössä. Missä sijaitsevat eri osat palvelusta ja miten eri osat on kytketty toisiinsa.

```plantuml
@startuml
actor User
node "Client_Host" as WIN10{
node "Browser"{
}
}

cloud "Network" as net{
queue "https"{
}
}

node "Uno Server / Ubuntu 20.04" as AWS{ 
node "Frontend_Container"{ 
}
node "Backend_Container" {
}
database "MariaDB_Container" {
}
node "Logger_Container" {
}

}
User -- Browser
Browser -- https
https -- Frontend_Container
Frontend_Container -- Backend_Container
Backend_Container -- MariaDB_Container
Logger_Container -- Frontend_Container
Logger_Container -- Backend_Container
Logger_Container -- MariaDB_Container

@enduml
```
## Palveluun liittyvät muut järjestelmät

Alla olevat kuvaukset ovat esimerkkejä UML-kuvauksen mahdollisuuksista, kannattaa tutustua tarkemmin laajempaan vaatimusmäärittely pohjaan,  koska siitä löytyy esimerkkejä.

> Järjestelmien välisiä yhteyksiä voidaan kuvata tarvittaessa esim. UML-kuvauksiin liittyvän sekvenssikaavion muodossa (Sequence Diagram). 

```plantuml
Client_Host --> Service_Frontend: Login Request
Service_Frontend --> Service_Backend : Logging request check
Service_Backend --> MariaDB : SQL Request for user account
MariaDB --> Service_Backend : Account and password 
Service_Backend --> Service_Frontend : Request Result pass
Service_Frontend --> Client_Host : Logged in

```
## Standardit ja lähteet

> Vaatimusmäärittelyyn kannattaa liittää mukaan kaikki tärkeät lähteet, joista on hyötyä tai merkitystä kokonaisuuden kannalta. Standardit ja ennalta jaetut ohjeistukset ovat hyödyllisiä lähteitä ja tarvittaessa tukevat esitettyjä vaatimuksia.

| ID | Nimi | Linkki | Kuvaus |  
|:-:|:-:|:-:|:-:|
| REF1 | JHS 165 ICT | [JHS Suositukset - vaatimusmäärittelylle](http://www.jhs-suositukset.fi/c/document_library/get_file?uuid=b8118ad7-8ee4-459a-a12b-f56655e4ab9d&groupId=14) | Vaatimusmäärittelyn suositus |
| REF2 | ISO 9241-11  | [Käytettävyys](https://fi.wikipedia.org/wiki/K%C3%A4ytett%C3%A4vyys)  | Usability | 
| REF3 |  EN 301 549 | [Saavutettavuus](https://fi.wikipedia.org/wiki/Saavutettavuus) | Availability |
| REF4 |  GDPR | [GDPR Asetus](https://europa.eu/youreurope/business/dealing-with-customers/data-protection/data-protection-gdpr/index_fi.htm) | General_Data_Protection_Regulation |
