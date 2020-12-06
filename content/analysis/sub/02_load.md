Analys av laddningstider
=======================

Målet är att mäta tre hemsidors laddningstider. Jag har valt att ta en lite närmare
titt på stora hemsidor som: Youtube, Reddit och WSJ.

<br/>

Urval
-----------------------

Jag har valt att studera Youtube, Reddit och WSJ eftersom de är alla väldigt stora hemsidor
med många användare och jag var intresserad över hur effektiva hemsidorna är.

<br/>

Metod
-----------------------

Jag använde mig av googles devtools PageSpeed Insights som mäter enligt Lighthouse Scoring.

<br/>

Resultat
-----------------------
![Image Title](%assets_url%/img/YOUTUBE-2.jpg) {.extrasmall}
![Image Title](%assets_url%/img/WSJ-1.jpg) {.extrasmall}
![Image Title](%assets_url%/img/REDDIT-1.jpg) {.extrasmall}

<br/>

Hemsidorna Reddit och Youtube fick båda en liknande poäng utvärdering (ca. 20-30)
Youtube hade där den bästa poängen med 32.
WSJ däremot presterade dåligt i alla tester (ca. 4-5).
Det som stog ut mest från WSJ och de andra två hemsidorna var att den hade extremt lång tid
tills sidan blev helt användbar TtI (Time to Interactive) vilket var på en tid mellan 42-45 sekunder.
WSJ hade även nästan dubbelt så hög TBT (Total Blocking Time) vilket kan kan bero på att sidan tog så lång
tid att ladda klart.
Youtube stog också ut med sitt värde av FCP (First Contentful Paint) där bara 6% av alla sidans inläsningar kunde
skrivas ut inom den första sekunden.
Medans Reddit hade 43% och WSJ hade 55%.
WSJ hade en väldigt snabb LCP (Largest Contentful Paint) på 1,9 sekunder vilket anses vara bra.
Och laddas in inom den första sekunden i 86% av inläsningarna.
WSJ stog även ut bland de andra genom att ha hela ~15 sekunders uppskattad tidsbesparing genom att ta bort
JavaScript som inte användes.

<br/>

Analys
-----------------------

Jag anser att Youtubes FCP är dålig pga att sidan innehåller videor och därför lär det vara svårt att göra en inläsning
som är snabbare än en sekund. Över lag så presterar Youtube väldigt bra, och många av tiderna är bättre eller snabbare än
de tider som Reddit har. WSJ har även de en väldigt snabb sida, men verkar falla pga. dess javascript som verkar göra
att sidan inte är helt interaktiv under flera sekunder.
Jag gissar att det kan bero på att de laddar in flera "pop-ups" med videor eller liknande vilket ser ut att ta väldigt lång tid
för hemsidan att ladda in. Utan dessa Javascript så hade hemsidan antagligen presterat lika bra eller bättre än Youtube och Reddit.

<br/>

Referenser
-----------------------

https://docs.google.com/spreadsheets/d/1l8lpMKbUnkjQrepzW1gDB0KV3kW3EHY_wwXlmet7lOg/edit?usp=sharing
https://web.dev/first-contentful-paint/?utm_source=lighthouse&utm_medium=unknown

Övrigt
-----------------------

Filip Antonsson
