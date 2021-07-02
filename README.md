# Cellulaire Automata
Verschillende soorten CA modelleren.
## Omschrijving
Dit project behandelt een-dimensionale CA en twee-dimensionale CA. Je kan met dit project een-dimensionale CA modelleren met een generieke regelset. Zo kan je bijvoorbeeld rule 30 toepassen. Daarnaast kan je ook Conway's Game Of Life uitvoeren. 

## Handleiding
Als we een een-dimensionale CA willen gebruiken moeten we eerst een object maken. Dat kan op de volgende manier:
```python
object_een = een_dimensionaal({hoogte},{breedte}, {begin}, {lijst0}, lijst{1})
```
Hierbij is de hoogte de hoogte van het rooster dat gemaakt wordt. De breedte de breedte van het rooster. Verder is begin de beginsituatie die je zelf kan instellen. 
Tenslotte zijn lijst0 en lijst1 de lijst van combinaties getallen die respectievelijk cellen naar 0 of 1 sturen.

We kunnen ook een twee-dimensionale CA gebruiken dan moet natuurlijk wel weer eerst een object worden gemaakt. Dan kan als volgt:
```python
object_twee = twee_dimensionaal({hoogte}, {breedte}, {aantal_updates})
```
Hierbij is de hoogte en breedte hetzelfde als in het geval van een_dimensionaal. Hier hebben we echter niet de begin, lijst0 en lijst1 paramteres,omdat we enkel willekeurige roosters bekijken en de regelset al vast ligt, namelijk de regelset van Conway's Game Of Life. Verder is er wel een nieuwe parameter namelijk aantal_updates. Deze parameter bepaalt het aantal evoluties dat plaats gaat vinden. In het geval van een_dimensionaal staat niet namelijk al vast door de groote van het rooster, echter in het geval van twee_dimensionaal moet er eindsignaal worden gegeven.

Nu we de objecten hebben gemaakt kunnen we ze gaan modelleren. We kunnen de een_dimensionale CA modelleren als volgt:
```python
object_een.grafisch()
```
Dit zal een plot geven van het eindresultaat van de CA. Daarnaast kunnen we ook de twee_dimensionale CA gaan modelleren als volgt:
```python
print(object_twee)
```
Dit zal de roosters printen die ontstaan na de evolutie. Het zal aantal_updates evoluties prnten.
