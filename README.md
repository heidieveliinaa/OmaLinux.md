# OmaLinux.md
Homework reports for Linux course taught by Tero Karvinen
# h0 Kurssi ja tekijä

**Kurssi:** Linux-palvelimet
**Tekijä:** (oma nimi)
**Päivämäärä:** (pp.kk.vvvv)

---

# h1 Oma Linux

## x) Lue ja tiivistä

### Raportin kirjoittaminen

* Raportin tulee olla täsmällinen ja toistettava: toinen henkilö pystyy tekemään samat vaiheet samalla tavalla.
* Ympäristö (host OS, rauta, ohjelmistoversiot) on kuvattava selkeästi.
* Virhetilanteet ja niiden ratkaisut tulee dokumentoida huolellisesti.

### Install Debian on VirtualBox – Updated 2023

* Artikkeli opastaa Debianin asentamisen VirtualBox-virtuaalikoneeseen.
* Asennuksessa suositellaan käyttämään Live-tilaa, koska se on käyttäjäystävällisempi.
* Riittävä levytila ja RAM-muisti parantavat käyttökokemusta.

### Debian Live -levykuva

* Debian Live -ISO mahdollistaa järjestelmän kokeilemisen ennen asennusta.
* Live-tilasta tehty asennus tuottaa usein paremman lopputuloksen kuin perinteinen installer.

(Lähteet: Tero Karvinen 2023, Debian Project)

---

## a) Asenna Linux virtuaalikoneeseen

### Ympäristö

* **Host OS:** Windows 11 64-bit
* **Tietokone:** Kannettava, Intel i5 -prosessori, 16 GB RAM
* **VirtualBox:** versio 7.x
* **ISO-tiedosto:** debian-live-12.6.0-amd64-xfce.iso

### Virtuaalikoneen luonti

* Uusi virtuaalikone luotiin VirtualBoxissa.
* **Nimi:** Debian12
* **Tyyppi:** Linux
* **Versio:** Debian (64-bit)
* **Muisti:** 4096 MB
* **Prosessorit:** 2 ydintä
* **Levytila:** 40 GB (VDI, dynaamisesti allokoitu)

### Asennusprosessi

1. Virtuaalikone käynnistettiin ISO-tiedostosta.
2. Boot-valikosta valittiin **Live Desktop**.
3. Live-työpöydältä käynnistettiin asennusohjelma.
4. Valittiin kieli (suomi), näppäimistö (suomalainen) ja aikavyöhyke.
5. Levyosiointi tehtiin automaattisesti.
6. Luotiin käyttäjä ja salasana.
7. Asennus suoritettiin loppuun ja virtuaalikone käynnistettiin uudelleen.

### Lopputulos

* Debian käynnistyi onnistuneesti.
* XFCE-työpöytäympäristö toimi ilman ongelmia.

*(Lisää tähän ruutukaappaukset: VM-asetukset, asennusvaihe, valmis työpöytä)*

---

## k) Vapaaehtoinen bonus: suosikkiohjelmani Linuxilla

### Firefox-selain

* Firefox on valmiiksi asennettu Debianissa.
* Avasin selaimen ja kävin Debianin virallisilla verkkosivuilla.
* Selain toimi sujuvasti ja tukee päivittäistä käyttöä.

---

## Lähteet

* Tero Karvinen – Linux-palvelimet: [https://terokarvinen.com/linux-palvelimet/](https://terokarvinen.com/linux-palvelimet/)
* Debian Project – [https://www.debian.org/](https://www.debian.org/)
* Install Debian on VirtualBox – Updated 2023
* Johanna 2025: Install Debian 13 Trixie with VirtualBox
