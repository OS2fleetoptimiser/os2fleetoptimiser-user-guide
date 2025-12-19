# Ofte stillede spørgsmål

*1. Hvad forstås ved en **rundtur**?*

En rundtur starter fra et køretøj forlader sin hjemmelokation og slutter, når køretøjet er retur på hjemmelokationen igen. Hvis man har sat vagtlag på som filter eller parameter, vil dette samle alle kørsler inden for det valgte tidsrum til én rundtur.

*2. Hvad betyder **rundturspræcision** - og hvilken betydning har det, hvis den er lav?* 

FleetOptimiser anvender allokeringsalgoritmer til at aggregere GPS-data. Det betyder, at alle GPS-logs behandles og forsøges at kobles på en rundtur. Hvis præcisionen er lav, betyder det, at der er kørsel, som ikke kan allokeres til en rundtur. Det kan bl.a. være gældende, hvis et køretøj parkerer langt fra de parkeringspunkter, der er registreret i konfigurationen. Det kan have en betydning i simuleringer, hvis den er lav, fordi køretøjer så låses i unødvendigt lang tid - køretøjet frigives først, når det registreres, at det er tilbage på sin hjemmelokation. Hvis man har vagtlag på, betyder det ingenting. Såfremt man ønsker at forbedre rundturspræcisionen bør man kigge på parkeringspunkterne, og evt. tilføje nogle flere i området, hvor der også parkeres. 

*3. Kan jeg simulere på **flere lokationer** samtidig?*

Ja, det kan du. Du skal blot vælge flere lokationer i "simuleringsindstillinger". Så vil værktøjet behandle lokationerne som én, og køretøjerne kan altså deles på tværs. 

*4. Hvordan **deaktiverer** jeg køretøjer, vi ikke længere bruger?*

Det gør du i "konfiguration - køretøjer". Her trykker på det grønne stik. Det er vigtigt at deaktivere køretøjet og ikke slette det, hvis du forstsat gerne vil kunne simulere på historisk data.  

*5. Hvordan bruges data fra **flådestyringssystemet**?*

Data fra flådestyringssystemet overføres en gang i døgnet til FleetOptimiser. GPS-logs er her den primære datakilde. Derudover overfører forskellige flådestyringssystemer også forskellige typer metadata på køretøjerne. Jo flere metadata, der overføres automatisk, jo færre systemer skal du vedligeholde data i. 
