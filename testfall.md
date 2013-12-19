Testfall Vernoles GIS System
========

####UC1 Autentisera användaren och returnera informationen

####Huvudscenario
   1. **Byggingenjören** vill ha information från databasen.
   2. **Systemet** ber om byggingenjörens användaruppgifter.
   3. **Byggingenjören** anger användarnamn och lösenord.
   4. **Systemet** autentiserar byggingenjören.
   5a. **Byggingenjören** klickar på tomten på GIS kartan för att få information om tomten.
   5b. **Byggingenjören** anger tomtens id nummer i en formulären för att få information om tomten.
   6. **Systemet** kontollerar att byggingenjören har de rättigheterna som krävs för att få tillgång till informationen.
   7. **Systemet** returnerar den begärda informationen.
	

####Testfall

####TF 1.1 Huvudscenario 1a - Autentisera som byggingenjör och få tillgång till informationen genom att klick på kartan.
   1. Gå till inloggningsportalen.
   2. Inloggningsformulären visas.
   3. Byggingenjörens användarnamn och lösenord anges.
   4. Inloggningen lyckas.
   5. Klicka på tomten på kartan.
   6. Information angående tomten returneras.

####TF 1.2 Huvudscenario 1b - Autentisera som byggingenjör och få tillgång till informationen genom att ange tomtens id nummer.
   1. Gå till inloggningsportalen.
   2. Inloggningsformulären visas.
   3. Byggingenjörens användarnamn och lösenord anges.
   4. Inloggningen lyckas.
   5. Ange tomtens id nummer i formulärens sök funktion.
   6. Information angående tomten returneras.

####TF 1.3 Alternativt Scenario 4a - Misslyckad autentisiering
   1. Gå till inloggningsportalen.
   2. Inloggningsformulären visas.
   3. Byggingenjörens användarnamn och lösenord anges.
   4. Inloggningen misslyckas.
   5. Felmeddelande visas.
   6. Inloggningsformulären visas igen.
   
####TF 1.4 Alternativt Scenario 6a - Otillräckliga rättigheter
   1. Gå till inloggningsportalen.
   2. Inloggningsformulären visas.
   3. Byggingenjörens användarnamn och lösenord anges.
   4. Inloggningen lyckas.
   5. Klicka på tomten på kartan.
   6. Fel meddelande visas - användaren har inte de rättigheterna som krävs för att få tillgång till informationen.
   7. Användaren uppmanas kontakta kommuningejören för att få de nödvändiga rättigheterna.

####TF 1.5 Alternativt Scenario 7a - Informationen finns inte
   1. Gå till inloggningsportalen.
   2. Inloggningsformulären visas.
   3. Byggingenjörens användarnamn och lösenord anges.
   4. Inloggningen lyckas.
   5. Klicka på tomten på kartan.
   6. Fel meddelande visas - Den begärda informationen finns inte.
   7. Användaren uppmanas kontakta kommuningejören för att få tillgång till den begärda informationen.