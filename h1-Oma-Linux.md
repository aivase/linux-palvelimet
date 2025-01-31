# x)
# Raportin kirjoittaminen
## Hyvä raportti on

- toistettava
- täsmällinen
- helppolukuinen
- viitattu lähteisiin
- aiheessa pysyvä

(Tero Karvinen 2006)

---

# What is free software?

## Neljä vapautta
1. Vapaus käyttää ohjelmaa mihin tahansa tarkoitukseen omien tarpeiden mukaan.
2. Vapaus tutkia ohjelman toimintaa ja muokata sitä sopimaan omiin tarkoituksiin. Tämä edellyttää, että pääset käsiksi ohjelman lähdekoodiin.
3. Vapaus jakaa muille kopioita ohjelmasta, jotta muutkin voivat hyötyä siitä.
4. Vapaus jakaa omia muokattuja versioitasi ohjelmasta, jotta myös yhteisö voi hyötyä tekemistäsi parannuksista.

(GNU 2024)

---

## Suoritettu tietokoneella, josta löytyy:
### Windows 11
### AMD Ryzen 5 3600 6-Core Processor 
### Nvidia GeForce RTX 4060
### Asennettu RAM 16 Gt

---
# a)
# Linuxin asentaminen virtuaalikoneeseen

- Latasin debian-live-12.9.0-amd64-xfce.iso -levykuvan osoitteesta:  
  https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/
- Avasin VirtualBoxin ja painoin New-kuvaketta, johon muokkasin asetukset:
  - Asetin nimeksi "Debian"
  - ISO Image: Valitsin lataamani debian-live-12.9.0-amd64-xfce.iso -levykuvan
  - Vaihdoin versioksi Debian (64bit)
  - Laitoin "Skip Unattended Install" päälle
  - Suljin asetukset painamalla Finish

  - Oikeaklikkasin juuri luotua virtuaalikonetta ja valitsin Settings
  - Asetuksissa valitsin Storage
  - Storagessa klikkasin Controller: IDE -alapuolelta Empty-kohtaa, jossa on CD-levyn kuva
  - Tämän jälkeen klikkasin Attributes-otsikon alla olevaa CD-levyn kuvaa, josta valitsin Choose/Create Virtual Optical Disk. Avautuneessa ikkunassa painoin Add-nappia ja valitsin debian-live-12.9.0-amd64-xfce.iso -levykuvan
  - Lopetin painamalla OK-nappia

  - Yritin käynnistää virtuaalikonetta tuplaklikkaamalla, mutta sain virheilmoituksen:  
    Not in a hypervisor partition (HVP=0) (VERR_NEM_NOT_AVAILABLE)  
    AMD-V is disabled in the BIOS (or by the host OS) (VERR_SVM_DISABLED)
    - Korjasin ongelman avaamalla BIOS/UEFI-asetukset ja vaihtamalla SVM Mode: Disabled --> Enabled
  - Käynnistin Live System -tilan
  - Avasin työpöydällä olevan Install Debian -tiedoston
  - Asetin asennusohjelmassa suomenkielisen näppäimistön ja valitsin Erase Disk -vaihtoehdon
  - Suoritin asennuksen ja uudelleenkäynnistin virtuaalikoneen

  - Avasin terminaalin ja suoritin siellä seuraavat komennot päivitysten ja palomuurin asentamiseksi:
    - sudo apt-get update
    - sudo apt-get -y dist-upgrade
    - sudo apt-get -y install ufw
    - sudo ufw enable

  - Asensin Guest Additions -lisäosat kirjoittamalla terminaaliin seuraavat komennot:
    - cd /media/*/VBox*
    - sudo bash VBoxLinuxAdditions.run

---

### Lähteet:
- https://www.gnu.org/philosophy/free-sw.html#four-freedoms
- https://terokarvinen.com/2006/raportin-kirjoittaminen-4/
- https://terokarvinen.com/2021/install-debian-on-virtualbox/
