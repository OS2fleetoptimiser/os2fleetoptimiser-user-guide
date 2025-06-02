# Manuel simulering #

I _manuel simulering_ kan du manuelt tilføje og fjerne køretøjer i simuleringerne. Udgangspunktet for simuleringen er de køretøjer, som er på lokationen/-erne i forvejen. I dette simuleringsværktøj kan du f.eks. undersøge om der er overkapacitet ved at fjerne en eller flere køretøjer, se hvor stor en del af turene der kan køres på cykel ud fra en række parametre du selv kan indstille, eller teste nye bilmodeller, som I overvejer at anskaffe ift. bl.a. rækkevidde, ladetid, CO2-udledning og økonomi.

## Simuleringsopsætning ##
Hvis ikke du laver nogle ændringer, og blot klikker på _start simulering_, vil du få et overblik over de ture, der bliver kørt i dag med den nuværende sammensætning, og algoritmen vil tildele de længste ture til de grønneste og mest økonomiske køretøjer for at reducere omkostninger og co2-reduktioner. 

![simuleringsopsætning - forside - reduceret str](https://github.com/user-attachments/assets/4a2846ee-bc48-4194-ba84-ace92226fc18)

I kolonnen _antal i simulering_, kan du prøve at fjerne en eller flere biler fra delflåden. Klik herefter igen på simulér for at få simuleringsresultatet på baggrund af den nye simulerede flådesammensætning.

### Simuleringsindstillinger ###

Før du starter din simulering, kan du lave om i indstillingerne, som påvirker resultatet af simuleringen.

![simuleringsindstillinger - reduceret str](https://github.com/user-attachments/assets/1e86f3ad-49ea-40a4-b9e2-5daf819721d1)

__Optimal tildeling__: Hvis du aktiverer _optimal tildeling_, aktiveres en optimeringsalgoritme, der forsøger at planlægge allokeringen af køretøjer på den mest optimale måde. Dvs. en måde hvor der både spares på økonomi og CO2e udledning. Der laves så og sige en afvejning mellem udledning og omkostning, eksempelvis ved at allokere de køretøjerne med den laveste CO2-udledning og laveste omkostning til de længste ture. 

__Begræns km/år__: Hvis du aktiverer _begræns km/år_, vil simuleringen tage højde for at kilometertallet pr. år ikke overstiger det tilladte, for køretøjer med et max antal km/år på leasingaftalen. Du kan indtaste oplysninger om max km/år under fanebladet konfiguration.
Her kan du ændre værdierne der danner grundlaget for udregning af de samlede omkostninger samt CO2-udledningen.

__Vagtlag__: Her kan du indstille vagtlag for simuleringerne, hvor en bil "låses" til hele det tidsrum du vælger, således at simuleringerne i højere grad afspejler virkeligheden hvor medarbejderne ikke nødvendigvis kan bytte bil hver gang bilen er på hjemlokationen i løbet af en vagt.

__Generelt__: Her kan du ændre på de generelle stillinger for simuleringer, som f.eks. co2-udledning ved kørsel i hhv. el- og fossilkøretøjer, drivmiddel priser, tid til køretøjsskift og maksimalt tilladte ukørte ture. Du kan vælge at gemme for den enkelte simulering eller at glemme gobalt, dvs. dine ændringer gør sig også gældende i fremtidige simuleringer og for andre brugere i din organisation. 

__Cykel__: Hvis du vil simulere med cykler, kan du indstille en række parametre for disse, bl.a. maksimal rutelængde, gennemsnitshastighed, samt indstille hvilke tidsrum ruter må tildeles til cykler, f.eks. hvis cykler kun må tildeles til ruter i dagtimerne.

__Testkøretøjer__: Her kan du tilføje testkøretøjer til simuleringen, hvis du vil prøve at simulere med cykler eller andre bilmodeller end dem der er på lokationen i forvejen. Du kan tilføje køretøjerne direkte her, eller gøre det i konfigurationen i venstre side. 


## Resultater ##


