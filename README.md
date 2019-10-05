oe-selectie-gokspel
# Gokspel

## Methode GeefStartSituatie
- In de variabele **teGokkenGetal** wordt een getal van 0 t.e.m. 9 opgeslagen
- In de console verschijnt te tekst 'teGokkenGetal = ' gevolgd door de inhoud van de variabele teGokkenGetal
- De cursor wordt in txtGetal geplaatst
- btnGok is uitgeschakeld
Deze methode wordt opgeroepen op het moment dat het programma opstart.
## Methode HeeftTekstMinimumLengte
Deze methode geeft een antwoord op de vraag of een bepaalde tekst een meegegeven minimum aan karakters heeft.
## Methode MarkeerTextBox
De opmaak van de doorgegeven textbox wordt gewijzigd afhankelijk van het feit of de input al dan niet geldig is.
- Geldige input
  - Randdikte = 1 px
  - Randkleur = grijs
  - Achtergrond = wit
- Ongeldige input
  - Randdikte = 2 px
  - Randkleur = rood
  - Achtergrond = lichtroos
## Gewijzigde input in txtGetal
Telkens als de input in txtGetal wijzigt, wordt de opmaak via **MarkeerTextBox** aangepast.
btnGok is enkel bruikbaar bij geldige input.
## Methode GeefFeedbackOpGok
De methode ontvangt een te gokken getal en een gok.
Op bais hiervan kan de volgende feedback gegeven worden:
- Hoger
- Lager
- U heeft het getal geraden
## Klik op btnGok
- Het gegokt getal wordt uitgelezen van txtGetal
- Er wordt feedback gegeven op basis van de return van GeefFeedbackOpGok. In dit statement wordt het aantal pogingen met 1 vermeerderd.
![feedback](/images/Raadspel.png)
- Als het getal geraden is wordt
  - txtGetal leegGemaakt en uitgeschakeld
  - btnGok uitgeschakeld
  - de cursor op btnNieuwSpel geplaatst
- Als het getal**niet** geraden is wordt
  - de cursor in txtGetal en de input ervan wordt gewist
## Klik op btnNieuwSpel
De methode GeefStartSituatie wordt uitgevoerd.
## Aanpassing methode GeefStartSituatie
Pas de methode **GeefStartSituatie** aan zodat de input van het vorige spel volledig verdwijnt en er een nieuwe spel gespeeld kan worden.
