# Raportin kirjoittaminen
## Hyvä raportti on

- toistettava
- täsmällinen
- helppolukuinen
- viitattu lähteisiin
- aiheessa pysyvä

(Tero Karvinen 2006)

# What is free software?

## Neljä vapautta
1. Vapaus käyttää ohjelmaa mihin tahansa tarkoitukseen omien tarpeiden mukaan.
2. Vapaus tutkia ohjelman toimintaa ja muokata sitä sopimaan omiin tarkoituksiin. Tämä edellyttää, että pääset käsiksi ohjelman lähdekoodiin.
3. Vapaus jakaa muille kopioita ohjelmasta, jotta muutkin voivat hyötyä siitä.
4. Vapaus jakaa omia muokattuja versioitasi ohjelmasta, jotta myös yhteisö voi hyötyä tekemistäsi parannuksista.

(GNU 2024)

# Linuxin asentaminen virtuaalikoneeseen
## Käyttöjärjestelmäni on Windows 11
- Latasin "debian-live-12.9.0-amd64-xfce.iso" levykuvan osoitteesta: https://cdimage.debian.org/debian-cd/current-live/amd64/iso-hybrid/.
- Virtualboxissa: 
  - new
  - asetin nimen
  - ISO image: debian-live-12.9.0-amd64-xfce.iso, jonka latasin
  - vaihdoin versioksi Debian (64bit)
  - asetin usernamen ja salasanan
  - lopetin finish napilla
    
  - klikkasin juuri luotua virtuaalikonetta ja valitsin asetukset
  - valitsin asetuksissa storage kohdan
  - storagessa painoin Controller: IDE alapuolelta Empty kohtaa jossa on CD-levyn kuva
  - tämän jälkeen klikkasin Attributes otsikon alla olevaa CD-levyn kuvaa, josta valitsin choose/create virtual optic disk, jonka sisässä painoin add nappulaa ja valitsin debian-live-12.9.0-amd64-xfce.iso levykuvan
  - lopetin painamalla ok nappia

  - yritin käynnistää virtuaalikonetta tuplaklikkaamalla ja sain virheilmoituksen "Not in a hypervisor partition (HVP=0) (VERR_NEM_NOT_AVAILABLE) AMD-V is disabled in the BIOS (or by the host OS)          (VERR_SVM_DISABLED"
  - 
### Lähteet:
https://www.gnu.org/philosophy/free-sw.html#four-freedoms

https://terokarvinen.com/2006/raportin-kirjoittaminen-4/
