---
title: Automatisk simulering
layout: default
parent: Simuleringer
nav_order: 3
---

# Automatisk simulering # 

På denne side foretages den automatiserede simulering der, på baggrund af det faktiske kørselsmønster, vil foreslå de mest optimale flådesammensætninger. Formålet er at tilfredsstille kørselsbehovet, men med en grønnere og/eller mere økonomisk bæredygtig flådesammensætning. Optimeringsalgoritmen vil forsøge at finde frem til løsninger og præsentere de op til fem bedste løsninger ud af potentielt flere tusinde forskellige kombinationer.

I denne vejledning kan du læse om de to faner i simuleringsværktøjet: 
+ Optimeringsopsætning
+ Resultater

## Optimeringsopsætning ##
Meget af opsætningen i den automatiske simulering er det samme som i __manuel simulering link__, hvorfor kun de opsætninger, der adskiller sig, gennemgås her.

![automatisk simulering -  opsætning - red str.png](..\assets\automatisk simulering -  opsætning - red str.png)

__Antal i optimering__: Algoritmen i målsimulering vil ikke skifte biler med gyldig leasingaftale ud, medmindre de er i overkapacitet. Du kan manuelt vælge/frigive specifikke køretøjer, som gerne må skiftes ud med andre alternativer, og på den måde give algoritmen mere råderum.  

__Optimeringsindstillinger__: 
+ Vægtning mellem omkostning og co2e udledning: Du kan i den automatiske simulering styre, hvad algoritmen skal prioritere: Her kan du styre hvad algoritmerne skal prioritere: Mest mulig CO2-reduktion (10), størst mulig økonomisk besparelse (0) eller 50/50 mellem de to parametre.
+ Testkøretøjer: Her kan du tilføje test-køretøjer, som algoritmen skal tage med i analysen. Dette giver mest værdi, hvis du har frigivet køretøjer, som kan skiftes ud. 


## Resultater ##

Når simuleringen er slut, præsenteres op til fem forskellige forslag til en ændret flådesammensætning, med udgangspunkt i den faktiske kørsel og ud fra de indstillinger du har lavet. Du har for hvert forslag mulighed for at hente resultaterne ned i excel.

![automatisk simulering - resultat 2.png](..\assets\automatisk simulering - resultat 2.png)

Besparelse (DKK/år): Den samlede økonomiske besparelse for den højest rangerede løsning. 
Reduktion udledning (Ton Co2e/år): Den samlede årlige CO2e-besparelse for den højeste rangerede løsning. Tallet er beregnet vha. miljøstyrelsens TCO-værktøj, hvorfra det udvalgte køretøjs allokerede ture, er udgangspunkt for det enkelte køretøjs årlige CO2e. 
Årlig omkostning i kr.: Oversigt over totale omkostninger for den nuværende flåde samt de forslåede løsninger. Der vises de samlede omkostninger inkl. omkostninger til drivmiddel.
Årlig udledning ton CO2e: Oversigt over CO2e-udledningen for den nuværende flåde  og de foreslåede løsninger. Udledningen er summeret til et helt år, uanset valg af dataperiode i simuleringssetup. De allokerede ture til de forskellige køretøjer ligger til grund for udregningen.

### Scenarier for resultater ###

__Løsningerne indeholder færre køretøjer__: Algoritmen har regnet sig frem til at kørselsbehovet kan tilfredsstilles med færre køretøjer end der er i den nuværende delflåde. Sker dette scenarie i din optimering, er det et tegn på, at der i flåden har overkapacitet. Eller i hvert fald kan turene planlægges på en anden måde med færre tilgængelige køretøjer. Du kan gå til manuel simulering og forsøge at justere antallet af køretøjer en for en for at undersøge nærmere, hvornår du rammer punktet for underkapacitet på lokationen.

__Der er ingen ændringer__: Hvis simuleringen foreslår blot en enkelt løsning (eller få løsninger med en/flere cykler), som er en-til-en den samme som den nuværende flåde, er det et tegn på, at der mangler fleksibilitet i opsætningen. Det vil typisk skyldes, at kørselsbehovet lige netop kan tilfredsstilles af den mængde køretøjer, der er i den nuværende flåde. Derfor er den nuværende flådesammensætning umiddelbart den rette. Ønsker du stadig, for den pågældende lokation, at få forslået andre løsninger, kan du frigøre køretøjer fra simuleringen (se pkt. 4 ovenfor).

__Løsningen indeholder flere køretøjer__: I tilfælde hvor du har slået 'begræns km/år' til, kan du risikere, at simuleringsresultatet bliver dyrere og udleder mere co2.  Det skyldes, at den faktiske kørsel overstiger de angivne km på leasing-aftalerne. I en sådan situation vil algoritmen tilføje ekstra køretøjer, så kørselsbehovet dækkes uden at overskride de angivne km-værdier. Problemet kan løses ved at justere køretøjernes km-antal i konfigurationen.
