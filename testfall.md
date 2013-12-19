Testfall Vernoles GIS System
========

####UC1 Autentisera anv�ndaren och returnera informationen

####Huvudscenario
   1. **Byggingenj�ren** vill ha information fr�n databasen.
   2. **Systemet** ber om byggingenj�rens anv�ndaruppgifter.
   3. **Byggingenj�ren** anger anv�ndarnamn och l�senord.
   4. **Systemet** autentiserar byggingenj�ren.
   5a. **Byggingenj�ren** klickar p� tomten p� GIS kartan f�r att f� information om tomten.
   5b. **Byggingenj�ren** anger tomtens id nummer i en formul�ren f�r att f� information om tomten.
   6. **Systemet** kontollerar att byggingenj�ren har de r�ttigheterna som kr�vs f�r att f� tillg�ng till informationen.
   7. **Systemet** returnerar den beg�rda informationen.
	

####Testfall

####TF 1.1 Huvudscenario 1a - Autentisera som byggingenj�r och f� tillg�ng till informationen genom att klick p� kartan.
   1. G� till inloggningsportalen.
   2. Inloggningsformul�ren visas.
   3. Byggingenj�rens anv�ndarnamn och l�senord anges.
   4. Inloggningen lyckas.
   5. Klicka p� tomten p� kartan.
   6. Information ang�ende tomten returneras.

####TF 1.2 Huvudscenario 1b - Autentisera som byggingenj�r och f� tillg�ng till informationen genom att ange tomtens id nummer.
   1. G� till inloggningsportalen.
   2. Inloggningsformul�ren visas.
   3. Byggingenj�rens anv�ndarnamn och l�senord anges.
   4. Inloggningen lyckas.
   5. Ange tomtens id nummer i formul�rens s�k funktion.
   6. Information ang�ende tomten returneras.

####TF 1.3 Alternativt Scenario 4a - Misslyckad autentisiering
   1. G� till inloggningsportalen.
   2. Inloggningsformul�ren visas.
   3. Byggingenj�rens anv�ndarnamn och l�senord anges.
   4. Inloggningen misslyckas.
   5. Felmeddelande visas.
   6. Inloggningsformul�ren visas igen.
   
####TF 1.4 Alternativt Scenario 6a - Otillr�ckliga r�ttigheter
   1. G� till inloggningsportalen.
   2. Inloggningsformul�ren visas.
   3. Byggingenj�rens anv�ndarnamn och l�senord anges.
   4. Inloggningen lyckas.
   5. Klicka p� tomten p� kartan.
   6. Fel meddelande visas - anv�ndaren har inte de r�ttigheterna som kr�vs f�r att f� tillg�ng till informationen.
   7. Anv�ndaren uppmanas kontakta kommuningej�ren f�r att f� de n�dv�ndiga r�ttigheterna.

####TF 1.5 Alternativt Scenario 7a - Informationen finns inte
   1. G� till inloggningsportalen.
   2. Inloggningsformul�ren visas.
   3. Byggingenj�rens anv�ndarnamn och l�senord anges.
   4. Inloggningen lyckas.
   5. Klicka p� tomten p� kartan.
   6. Fel meddelande visas - Den beg�rda informationen finns inte.
   7. Anv�ndaren uppmanas kontakta kommuningej�ren f�r att f� tillg�ng till den beg�rda informationen.