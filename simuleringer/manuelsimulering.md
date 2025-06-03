# Manuel simulering #

I _manuel simulering_ kan du manuelt tilføje og fjerne køretøjer i simuleringerne. Udgangspunktet for simuleringen er de køretøjer, som er på lokationen/-erne i forvejen. I dette simuleringsværktøj kan du f.eks. undersøge om der er overkapacitet ved at fjerne et eller flere køretøjer, se hvor stor en del af turene der kan køres på cykel ud fra en række parametre du selv kan indstille, eller teste nye bilmodeller, som I overvejer at anskaffe ift. bl.a. rækkevidde, ladetid, CO2-udledning og økonomi.

## Simuleringsopsætning ##
Hvis ikke du laver ændringer og blot klikker på _start simulering_, vil du få et overblik over de ture, der bliver kørt i dag med den nuværende sammensætning, og algoritmen vil tildele de længste ture til de grønneste og mest økonomiske køretøjer for at reducere omkostninger og co2-udledning.

![simuleringsopsætning - forside - reduceret str](https://github.com/user-attachments/assets/4a2846ee-bc48-4194-ba84-ace92226fc18)

I kolonnen _antal i simulering_, kan du prøve at fjerne et eller flere køretøjer fra delflåden. Klik herefter igen på simulér for at få simuleringsresultatet på baggrund af den nye simulerede flådesammensætning.

### Simuleringsindstillinger ###

Før du starter din simulering, kan du lave om i indstillingerne, som påvirker resultatet af simuleringen.

![simuleringsindstillinger - reduceret str](https://github.com/user-attachments/assets/1e86f3ad-49ea-40a4-b9e2-5daf819721d1)

__Optimal tildeling__: Hvis du aktiverer _optimal tildeling_, aktiveres en intelligent algoritme. Algoritmen er optimeret til at håndtere enkelt-dags-ture, og den anbefales derfor ikke, hvis man har lange rundture, der strækker sig over flere dage. 

__Begræns km/år__: Hvis du aktiverer _begræns km/år_, vil simuleringen tage højde for at kilometertallet pr. år ikke overstiger det tilladte, for køretøjer med et max antal km/år på leasingaftalen. Du kan indtaste oplysninger om max km/år under fanebladet konfiguration.

__Vagtlag__: Her kan du indstille vagtlag for simuleringerne, hvor en bil "låses" til hele det tidsrum, du vælger, således at simuleringerne i højere grad afspejler virkeligheden hvor medarbejderne ikke nødvendigvis kan bytte bil hver gang bilen er på hjemlokationen i løbet af en vagt.

__Generelt__: Her kan du ændre på de generelle stillinger for simuleringer, som f.eks. co2-udledning ved kørsel i hhv. el- og fossilkøretøjer, drivmiddel priser, tid til køretøjsskift og maksimalt tilladte ukørte ture. Du kan vælge at gemme for den enkelte simulering eller at glemme gobalt, dvs. dine ændringer gør sig også gældende i fremtidige simuleringer og for andre brugere i din organisation. 

__Cykel__: Hvis du vil simulere med cykler, kan du indstille en række parametre for disse, bl.a. maksimal rutelængde, gennemsnitshastighed, samt indstille hvilke tidsrum ruter må tildeles til cykler, f.eks. hvis cykler kun må tildeles til ruter i dagtimerne.

__Testkøretøjer__: Her kan du tilføje testkøretøjer til simuleringen, hvis du vil prøve at simulere med cykler eller andre bilmodeller end dem der er på lokationen i forvejen. Du kan tilføje køretøjerne direkte her, eller gøre det i konfigurationen i venstre side. 


  

## Resultater ##
På resultatsiden vises resultaterne af din simulering, herunder både potentielle gevinster og visualiseringer af ændringer. Udover oversigten med de forskellige visualiseringer, er det også her muligt at dykke ned i simuleringerne ved både at se køretøjsdetaljer og allokerede køretøjer til ruter på hhv. nuværende og simulerede flåde. 

_Eksemplet på et resultat nedenfor er baseret på en lokation med seks køretøjer, heraf fire fossile og to el-drevne._

![manuel simulering resultat red str](https://github.com/user-attachments/assets/73512023-cdb0-403a-bfb5-ef337fbd6a93)

__Rundture uden køretøj__: Viser hvor mange, hvis nogen, af rundturene i den valgte periode, der ikke ville kunne være blevet kørt, hvis man implementere de tiltag, man har lavet i indstillingerne. I eksemplet har man fjernet to ud af seks køretøjer, og det betyder, at én rundtur ud af de 78 i perioden ikke ville kunne være blevet kørt. 

__Årlig besparelse__: Den økonomiske betydning af både ændringer i antal og sammensætning køretøjer samt om-allokering af kørsel til de mest drifts-økonomiske køretøjer. Ofte vil det være en gevinst, men i sjældne tilfælde vil resultatet blive negativt. Vær her OBS på:
+ Løsningen antager, at rundture uden køretøj køres i medarbejdernes egne biler. Disse rundture vil derfor være en omkostning der pågøres i kilometerpenge pr. kørt km. Indstillinger for lav og høj takst fastsættes i _simuleringsindstillinger_ under _generelt_.
+ Hvis du har slået "begræns km" til i _simuleringsindstillinger_ og samtidig har fjernet en masse biler, kan det resultere i en negativ effekt, fordi de nuværende km i leasingaftalerne derfor ikke længere dækker det simulerede forbrug. Det samme antal km bliver lagt over på færre køretøjer, og det vil derfor være en mulig effekt. Km på leasingaftale kan indstilles i __konfiguration af køretøjer link__.

__Årlig co2-reduktion__: Her sammenlignes den faktiske kørsels udledning mod den simulerede kørsels. Reduktionen dækker kun over scope 1 reduktioner, dvs. reduktioner i drivmiddelforbrug. 

__Ikke kørte rundture pr. dag__: Her kan man se hvornår ikke kørte rundture ligger. Flere detaljer kan findes under fanerne _køretøjsdetaljer_ og _ruter_. 

__Nuværende turfordeling på køretøjstype__: Her kan man se, hvordan turene fordeler sig i den faktiske kørsel. I eksemplet ses det, at størstedelen af turene er på kortere ture, og at der er en nogenlunde jævn fordeling mellem kørsel i fossile- og el-biler. 

__Simuleret turfordeling på køretøjstype__: I eksemplet kan man se, at algoritmen har flyttet mere kørsel over til de to el-biler, og samtidig kan man se, at rundturen uden køretøj er på en rute under 20 km. Såfremt man har tilføjet eksempelvis el-cykler i simuleringsindstillinger, vil det også fremgå af denne visualisering.  

Du kan til hver en tid hente både nuværende og simuleret data ned i excel ved at trykke på pilen øverst i menuen ved siden af _ruter_. 



