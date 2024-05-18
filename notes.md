
# Setup notes for keeping track of what happened (was installed)
## For the requirements.txt
 - opustools
 - requests


python3 -m venv venvDialectData
source venvDialectData/bin/activate

# Installed opustools and played around in the terminal
pip install opustools[all]

# Install opustools using pip
pip install opustools-pkg
# → Problematic compared to the command-line tool!

- [ ] Set download file to be located in "AllBlue"


# Manual Download
source venvDialectData/bin/activate
cd /media/AllBlue/ProjectData/Language
mkdir Bavarian
cd Bavarian

## Find all available language pairs for Bavarian-German
opus_get --list --source bar --target de
   1 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-de.xml.gz
   2 MB https://object.pouta.csc.fi/OPUS-WikiMatrix/v1/xml/bar-de.xml.gz
  26 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-de.xml.gz
  71 KB https://object.pouta.csc.fi/OPUS-XLEnt/v1.2/xml/bar-de.xml.gz

   2 MB Total size

## List all bar-de files in the whole OPUS:
opus_get --source bar --target de --list
    Same as above


## Find available target languages for Bavarian in Tatoeba:
opus_get --list --directory Tatoeba --source bar
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/ang-bar.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-bar.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-bar.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-bzt.xml.gz
   1 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-de.xml.gz
   1 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-en.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-eo.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-es.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-fo.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-fr.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-hu.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-ja.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-kab.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-ku.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-kzj.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-la.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-nn.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-ofs.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-pt.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-sjn.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-swg.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-tr.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-uk.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar-yi.xml.gz
  33 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/ang.zip
  26 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bar.zip
  26 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/bzt.zip
  59 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/de.zip
 147 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/en.zip
  45 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/eo.zip
  33 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/es.zip
  32 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/fo.zip
  48 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/fr.zip
  21 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/hu.zip
   8 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/ja.zip
  33 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/kab.zip
  86 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/ku.zip
 340 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/kzj.zip
   1 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/la.zip
  95 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/nn.zip
   8 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/ofs.zip
  23 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/pt.zip
  13 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/sjn.zip
 161 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/swg.zip
  38 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/tr.zip
   9 MB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/uk.zip
 763 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/yi.zip

 465 MB Total size


## List all files in Tatoeba that include Bavarian:
opus_get --directory Tatoeba --source bar --list
    Same as above


## Download Tatoeba corpus for bar-de:
opus_get --directory Tatoeba --source bar --target de



## Find available target languages for Bavarian in wikimedia:
opus_get --list --directory wikimedia --source bar
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/ar-bar.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/arz-bar.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-ca.xml.gz
  17 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-cs.xml.gz
  26 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-de.xml.gz
  13 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-en.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-es.xml.gz
   2 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-fr.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-gsw.xml.gz
   2 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-nds_nl.xml.gz
   0 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-simple.xml.gz
   1 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar-yi.xml.gz
 208 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/ar.zip
   5 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/arz.zip
   1 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/bar.zip
 211 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/ca.zip
  42 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/cs.zip
 117 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/de.zip
   3 GB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/en.zip
 617 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/es.zip
 438 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/fr.zip
 208 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/gsw.zip
 160 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/nds_nl.zip
   9 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/simple.zip
   1 MB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/yi.zip

   5 GB Total size


## Download corpus data for source: Bavarian:

opus_get --directory wikimedia --source bar --target cs -q
opus_get --directory wikimedia --source bar --target de -q
opus_get --directory wikimedia --source bar --target gsw -q
opus_get --directory wikimedia --source bar --target nds_nk -q
opus_get --directory wikimedia --source bar --target yi -q
# opus_get --directory wikimedia --source bar --target en -q → 3 GB
# opus_get --directory wikimedia --source bar --target es -q → 617 MB
# opus_get --directory wikimedia --source bar --target fr -q → 438 MB



mkdir Alemannic

- [!] ISO Codes according to wikipedia: 
 - qct (Colonia Tovar)
 - gsw (Swiss German and Alsatian)
 - swg (Swabian)
 - wae (Walser)

## List all files in opus
opus_get --source qct --target de --list
  0 KB Total size
opus_get --source gsw --target de --list
   1 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/de-gsw.xml.gz
  10 KB https://object.pouta.csc.fi/OPUS-wikimedia/v20230407/xml/de-gsw.xml.gz
  11 KB Total size

opus_get --directory Tatoeba --source gsw --target de
opus_get --directory wikimedia --source gsw --target de
opus_read --directory Tatoeba --source gsw --target de -m 50
opus_read --directory wikimedia --source gsw --target de -m 20

opus_get --source swg --target de --list
  17 KB https://object.pouta.csc.fi/OPUS-Tatoeba/v2023-04-12/xml/de-swg.xml.gz
  17 KB Total size

opus_get --directory Tatoeba --source swg --target de
opus_read --directory Tatoeba --source swg --target de -m 50

opus_get --source wae --target de --list
   9 KB https://object.pouta.csc.fi/OPUS-Ubuntu/v14.10/xml/de-wae.xml.gz
   9 KB Total size

opus_get --directory Ubuntu --source wae --target de
opus_read --directory Ubuntu --source wae --target de -m 50 → EMPTY on wae side


