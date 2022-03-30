-- ENGLISH ---

MeteoServices - weewx extension that sends data to stations.meteo-services.com powered by MeteoServices / MR
Copyright 2015-2021 Dipl. Met. Frank Bandle (script base M. Wall)

Installation instructions:

0) Load the extension meteoservices-3.2.zip

1) run the installer:
# go to the directory with the "extension" to install:  EXTENSIONAME: meteoservices-3.2.zip

sudo wee_extension --install meteoservices-3.2

2) modify weewx.conf:   ( normally it will be done by the installer wee_extension )

You only have to enter a unique STATIONID from your registration at https://stations.meteo-services.com/login/

STATIONID will send to you by Mail / registered E-Mail address.
password is optional - set it to "1492254597"

This line you have to change with your given STATIONID

[StdRESTful]
    [[Meteoservices]]
        stationid = INSERT_STATIONID_HERE
        password  = INSERT_PASSWORD_HERE

3) restart weewx

sudo /etc/init.d/weewx stop
sudo /etc/init.d/weewx start

4) Done - your weatherdata should be displayed in 5 to 10 minutes at stations.meteo-services.com

Thank you
- MeteoServices -
Institute Weather- and Climatechangeanalytics


-- DEUTSCH ---

weather365 - weewx Erweiterung um Messdatatan an das stations-meteo-services.com powered by MeteoServices / MR zu senden
Das Script basiert auf einem Entwurf von M. Wall
Copyright: Dipl. Met. Frank Bandle 2015-2021

INSTALLATIONSANLEITUNG

0) Lade die EXTENSION meteoservices-3.2.zip herunter

1) INSTALLATION
# öffne ein TERMINAL Fenster und gehe in das Verzeichnis mit der EXTENSION: meteoservices-3.2.zip

sudo wee_extension --install meteoservices-3.2

2) ändere weewx.conf ( das macht im Normalfall die Installationsroutine wee_extension)

Sie müssen nur noch die passende STATIONID die sie nach Ihrer Registrierung auf https://stations.meteo-services.com/login/ bekommen eintragen

Eine eindeutige STATIONID wird per E-Mail an die registrierte E-Mail Adresse geschickt.
Das Passwort ist optional und wird auf "1492254597" gesetzt.

an diese Stelle in WEEWX kommt Ihre STATIONID

[StdRESTful]
    [[Meteoservices]]
        stationid = INSERT_STATIONID_HERE
        password  = INSERT_PASSWORD_HERE

3)  Neustart von weewx

sudo /etc/init.d/weewx stop
sudo /etc/init.d/weewx start


4) Fertig - Ihre WetterDaten sollten in ca 5 bis 10 Minuten auf stations.meteo-services.com sichtbar sein.

Vielen Dank 
- MeteoServices -
Institut Wetter- und Klimafolgenanalyse
