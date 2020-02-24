oe-objecten-kalender-opl
Oefening om een datum van dag, maand en jaar te wijzigen.
# Kalender: werken met het date-object
## HTML aanvullen
Plaats id's waar je dit nodig acht. Gebruik de notatie die in de lessenreeks werd afgesproken. M.a.w. voeg een prefix toe die aantoont over welk soort DOM-element het gaat.
## Opstarten
Bij het opstarten :
1. worden alle DOM-elementen gekoppeld. Declareer hiervoor de nodige variabelen.
2. worden de elementen gekoppeld aan de overeenkomstige function (via EventListeners)
3. wordt in de variabele *datum* een dag opgeslagen
4. wordt function **GeefFeedBack()** uitgevoerd
### GeefFeedBack()
* In de resp. span-tags worden de dag, maand en jaar van de opgeslagen datum getoond
* In de onderste div wordt de datum voluit getoond 
## Datums wijzigen
We voegen de nodige functionaliteit toe om de datum te laten wijzigen.
Via een parameter geeft de gebruiker door of het om een verhoging of verlaging gaat.
De nieuwe datum wordt getoond via GeefFeedback, en wordt per deel ook aangepast in de span-elementen.
We gebruiken hierbij de onderstaande functies :

### WijzigJaar()
Bij de huidige datum wordt een jaar bijgeteld of ervan afgetrokken. 
### WijzigMaand()
Bij de huidige datum wordt een maand bijgeteld of ervan afgetrokken. 
> ### Opgelet
> Hou er rekening mee dat, bij een verhoging in december of een verlaging in januari, ook van jaar gewisseld moet worden.
### WijzigDag()
Bij de huidige datum wordt een dag bijgeteld of ervan afgetrokken.
> ### Opgelet
> * Niet alle maanden hebben evenveel dagen
> * Een verhoging op 31 december zorgt voor een verspringing naar 1 januari van het volgende jaar
> * Als de verhoging resulteert in een onbestaande datum, dan plaats je de datum op de eerste dag van de volgende maand
> * Als je op de 1ste dag van de maand verlaagt, zul je ervoor moeten zorgen dat je de laatste dag van de vorige maand als resultaat bekomt
