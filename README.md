# Raportti: Debian Linuxin asennus virtuaalikoneeseen

**Kurssi:** Linux-palvelimet - ICI003AS2A-3016  
**Tekijä:** Heidi Immonen  
**Päivämäärä:** 18.1.2026  
**Paikka:** Kotilaboratorio, Windows 11 -kone

---

## x) Artikkelien tiivistelmät

### Install Debian on VirtualBox – Updated 2023
* Artikkeli opastaa Debianin asentamisen VirtualBox-virtuaalikoneeseen painottaen helppokäyttöisyyttä.
* Karvinen (2023) suosittelee asennuksen aloittamista **Live-tilasta**, sillä se on graafisesti selkeämpi ja helpompi aloittelijalle.
* Suorituskyvyn varmistamiseksi on tärkeää antaa koneelle riittävästi RAM-muistia ja levytilaa.

### Debian Live -levykuva
* Debian Live -ISO mahdollistaa järjestelmän kokeilemisen ilman asennusta suoraan RAM-muistista.
* Live-tilasta käynnistetty "Calamares"-asennusohjelma on usein varmatoimisempi kuin perinteinen tekstipohjainen asennin (Debian Project).

### Johanna 2025: Install Debian 13 Trixie
* Artikkelissa näytetään uuden Debian 13 "Trixie" -version asennusvaiheet.

---


## a) Asenna Linux virtuaalikoneeseen

### Ympäristö

* **Host OS:** Windows 11 64-bit
* **ISO-tiedosto:** debian-live-13.0.0-amd64-xfce.iso
* **Keskusmuisti (RAM):** 16 GB
* **Virtualisointiohjelmisto:** VirtualBox 7.1.x

### Virtuaalikoneen luonti
Loin uuden virtuaalikoneen seuraavin parametrein:
* **Nimi:** Debian13-Heidi
* **Tyyppi/Versio:** Linux / Debian (64-bit)
* **Muisti:** 4096 MB (4 GB)
* **Prosessorit:** 2 ydintä
* **Levytila:** 40 GB (VDI, dynaamisesti varattu)
* **Näytönohjain:** VMSVGA, 128 MB muistia

### Asennusprosessi
* **10:00** – Käynnistys: Liitin ISO-tiedoston virtuaaliseen CD-asemaan ja käynnistin koneen.
* **10:10** – Live Desktop: Valitsin käynnistysvalikosta *Live System*. Työpöytä latautui nopeasti. Testasin verkon toimivuuden.
* **10:20** – Asennus: Klikkasin työpöydältä "Install Debian" -kuvaketta.
* **10:35** – Konfigurointi: Valitsin kieleksi English (asennusohjelma) ja näppäimistöksi Finnish.
* **10:50** – Osiointi: Valitsin "Tyhjennä levy" (Erase disk). Ohjelma loi osiot automaattisesti.
* **11:00** – Käyttäjä: Luotiin käyttäjätunnus ja asetettiin salasana.
* **11:15** – Viimeistely: Asennus valmistui, poistin ISO-tiedoston ja käynnistin koneen uudelleen.

> **Huomio:** Asennus sujui ongelmitta. Huomasin, että 2 prosessoriydintä teki järjestelmästä huomattavasti nopeamman verrattuna oletusarvoiseen yhteen ytimeen.

Näyttökuva 2026-01-19 115133.png

### Lopputulos

* Debian käynnistyi onnistuneesti.
* XFCE-työpöytäympäristö toimi ilman ongelmia.


---

## k) Vapaaehtoinen bonus: suosikkiohjelmani Linuxilla

**Ohjelma:** GIMP (Image Manipulation Program)  
**Miksi tämä on suosikkini?** GIMP on ammattitason kuvankäsittelyohjelma, joka on täysin ilmainen. Se on kevyt ja sisältää valtavasti työkaluja muokkaamiseen.

**Toimenpiteen suorittaminen:**
1. **Asennus:** Avasin päätteen (Terminal). Päivitin paketit ja asensin ohjelman komennolla:
   ```bash
   sudo apt update
   sudo apt install gimp -y
    ```
Käyttö: Avasin ohjelman kirjoittamalla päätteeseen gimp.

Toimenpide: Otin kuvakaappauksen asennusraportistani, avasin sen GIMPissä, lisäsin siihen tekstikerroksen "Heidin Debian 13" ja tallensin kuvan.


---

## Lähteet

* Tero Karvinen – Linux-palvelimet: [https://terokarvinen.com/linux-palvelimet/](https://terokarvinen.com/linux-palvelimet/)
* Debian Project – [https://www.debian.org/](https://www.debian.org/)
* Install Debian on VirtualBox – Updated 2023
* Johanna 2025: Install Debian 13 Trixie with VirtualBox
