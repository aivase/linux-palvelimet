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

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/main/neofetch.png" alt="Neofetch Screenshot" width="500">


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

<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/main/root.png" alt="Root screenshot" width="500">

/home sisältää kaikkien käyttäjien kotihakemistot  

/home/eino on oma kotihakemistoni ja ainoa paikka johon käyttäjällä "eino" voi pysyvästi tallentaa tietoja. Sieltä löytyy esimerkiksi downloads, documents ja music.

/etc sisältää kaikki järjestelmän laajuiset asetukset teksitiedostoissa

/media sisältää laitteeseen liitetyt välineet kuten USB-tikku. ls /media ei näytä tuloksia sillä en ole liittänyt mitään välinettä tietokoneeseeni.

/var/log sisältää järjestelmän lokit

  
# d) 
  
## The Friendly M.

# e)
  
## Pipe

# f)
  
## Rauta
<img src="https://raw.githubusercontent.com/aivase/linux-palvelimet/refs/heads/main/lshw.png" alt="lshw screenshot" width="500">





