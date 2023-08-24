# storage_of_the_alliance_JavaSpringBoot

Haaga-Helia AMK:n "Palvelinohjelmointi"-kurssin harjoitustyönä päätin tehdä
uuden version aiemmasta 'liittouman_varasto_JavaSwing'-sovelluksestani. Suurin
käytännön ero uuden ja vanhan version välillä on se, että vahassa versiossa
data tallennettin paikalliseen 'SQLite'-tietokantaan, kun taas uudessa versiossa
'AWS'-pilvipalvelussa sijaitsevaan 'MariaDB'-tietokantaan. Samoin myös itse
sovellus oli käynnissä 'AWS'-pilven 'elasticbeanstalk'-alustalla. Kotikäyttöä
varten muokkasin tästä uudesta versiostani kuitenkin vielä ns. 'economic'-version,
jossa yksi kotimme tietokoneista tomii palvelimena, ja myös sovelluksen käyttämä
'MariaDB'-tietokanta sijaitsee tällä samaisella palvelinkoneella. Tämä siksi,
että 'AWS'-pilven käyttö ei koskaan ole täysin ilmaista. Uusien versioiden etu
vanhaan alkuperäiseen verrattuna on se, että nyt kaikki kotimme koneet voivat
langattoman lähiverkkomme kautta olla vuorovaikutuksessa saman tietokannan kanssa,
ja myös sovelluksen käyttöliittymään tein muutamia asiakkaan (eli vaimon) toivomia
pieniä muutoksia. Uutta varastoinventaariota ei myöskään onneksi tarvittu, koska
suoritin pienimuotoisen migraation siirtämällä ohjelmallisesti vanhan 'SQLite'-
tietokantamme datan uuteen 'MariaDB'-tietokantaamme. 

---

As a part of the "Server Programming" course at Haaga-Helia University of Applied
Sciences, I decided to create a new version of my previous 'liittouman_varasto_JavaSwing'
application as the course project. The most significant practical difference between
the new and old versions is that in the previous version, data was stored in a local
'SQLite' database, whereas in the new version, it's stored in a 'MariaDB' database on
the 'AWS' cloud service. Additionally, the application itself was hosted on the 'AWS'
cloud using the 'elasticbeanstalk' platform. However, for home use, I further modified
this new version into what I call the 'economic' version. In this version, one of our
home computers acts as a server, and the 'MariaDB' database used by the application is
also located on this same server machine. I made this decision because using the 'AWS'
cloud service is never entirely free. One advantage of these new versions compared to
the original is that now all the computers in our home can interact with the same database
through our wireless local network. I also made a few minor changes to the application's
user interface based on some requests from the customer (my wife). Fortunately, there
was no need to perform a new inventory for the stock either, because I performed a small-
scale migration by programmatically transferring the data from our old 'SQLite' database
to the new 'MariaDB' database.
