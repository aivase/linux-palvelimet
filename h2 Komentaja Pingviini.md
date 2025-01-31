# x)
## Command Line Basics Revisited  
  
-pwd tulostaa nykyisen hakemiston  
-ls tulostaa luettelon työhakemiston tiedostoista  
-cd vaihtaa hakemistoa  
-cd .. vaihaa hakemistoa taaksepäin  
-mkdir asd luo uuden kansion nimellä asd

# a)
## Asenna micro-editori
### Asensin micro-editorin suorittamalla seuraavat komennot terminaalissa:  
  
    sudo apt-get update  
  
    sudo apt-get install micro  
# b)
## Asenna kolme itsellesi uutta komentoriviohjelmaa  
### 1. Neofetch
  
   Asensin neofetch komentoriviohjelman suorittamalla seuraavat komennot terminaalissa:  

      sudo apt-get update  
        
      sudo apt-get install neofetch  
        
Kun syöttää komennon neofetch terminaaliin saa näkyviin järjestelmän ja laitteiston tietoja.  

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/main/neofetch.png" alt="Neofetch Screenshot" width="500" height="500">


### 2. Htop
   Asensin htop komentoriviohjelman suorittamalla seuraavat komennot terminaalissa:  
     
      sudo apt-get update  
      
      sudo apt-get install htop  
        
Kun syöttää komennon htop terminaaliin avautuu näkymä, jossa voi seurata järjestelmän resurssien käyttöä reaaliajassa. Näkymän saa sujettua q näppäintä painamalla.

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/htop.png" alt="Htop screenshot" width="500">

### 3. Tree
Asensin tree komtoriviohjelman suorittamalla seuraavat komennot terminaalissa:
  
    sudo  apt-get update
    sudo apt-get install tree

Kun syöttää komennon tree terminaaliin avautuu visuaalinen kuvaus hakemistorakenteesta  
  
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/tree.png" alt="Tree screenshot" width="500">

# c) 

## FHS

/ Root directory on tietojärjestelmän ylin hakemisto, josta löytyy esimerkiksi bin, dev ja home.

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/main/root.png" alt="Root screenshot" width="800">

/home sisältää kaikkien käyttäjien kotihakemistot  
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/home.png" alt="Home screenshot" width="800">  

/home/eino on oma kotihakemistoni ja ainoa paikka johon käyttäjällä "eino" voi pysyvästi tallentaa tietoja. Sieltä löytyy esimerkiksi downloads, documents ja music.

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/home%20eino.png" alt="Home/eino screenshot" width="800">  

/etc sisältää kaikki järjestelmän laajuiset asetukset teksitiedostoissa
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/etc.png" alt="Home/eino screenshot" width="800">  

/media sisältää laitteeseen liitetyt välineet kuten USB-tikku. ls /media ei näytä tuloksia sillä en ole liittänyt mitään välinettä tietokoneeseeni.

/var/log sisältää järjestelmän lokit  
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/varlog.png" alt="Home/eino screenshot" width="800">  

# d) 
  
## The Friendly M.  
  
grep-komento etsii sanan "moi" kaikista hakemiston tiedostoista ja näyttää löytyneet rivit sekä tiedoston nimen.
  
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/grep1.png" alt="grep screenshot" width="800">  

# e)
  
## Pipe
Komennolla ps aux näytetään kaikki käynnissä olevat prosessit ja lisäämällä siihen | grep "bash" rajataan sen näyttämään vain ne joissa on "bash"

    ps aux | grep "bash"
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/grepbash.png" alt="grepbash screenshot" width="600">  

# f)
  
## Rauta
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/lshw.png" alt="lshw screenshot" width="500">

Listasta voidaan tulkita esimerkiksi, että järjestelmä on Virtualbox ja prosessori on AMD Ryzen 5 3600 6-Core

## Lähteet:  
https://terokarvinen.com/2020/command-line-basics-revisited/?fromSearch=command%20line%20basics%20revisited  
https://terokarvinen.com/linux-palvelimet/  








