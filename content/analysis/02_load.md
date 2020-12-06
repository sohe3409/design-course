---
Title: Page Speed
Description: Analysis report 2
Template: analysis
---
Laddningstid
=======================
<div class="report">
    <div class="selection">
      <p class="intro">Denna undersökning kollar på tre olika hemsidor för att testa hur snabbt de laddas och för att se om det finns någon förbättringspotential för att minska laddningstiden och öka användbarheten.</p>
      <h2>Urval</h2>
      <p>När jag valde vilka tre hemsidor jag skulle undersöka tänkte jag på vilken typ av hemsida jag skulle vilja få information snabbt ifrån. Jag kom att tänka på hur jag tidigare under dagen försökt hitta nyheter om en viss händelse, så jag gjorde samma sökning igen och blev intresserad av vilka nyhetssajter som kom högst upp för de var inte nödvändigtvis de hemsidor jag hade förväntat mig. Detta gav mig idén att undersöka tre hemsidor som bland annat eller till största del innehåller nyhetsrapportering: Sveriges Radio som är en public servicesida som fokuserar på ljud, Expressen som från början är en papperstidning, vars hemsida har väldigt mycket bilder och olika typer av media som kan påverka laddningstiden, samt VICE, en internationell hemsida med gratis nyhetsrapportering och ofta lite mer annorlunda nyheter, och som riktar sig mot en yngre läsargrupp genom digitala medier. Jag valde att endast granska startsidan av varje hemsida, det första man ser och upplever när man går in på sidan.</p>
    </div>
        <hr style="width:100%">
    <div class="method">
      <h2>Metod</h2>
      <p>Både för mobila enheter och desktop samlade jag in följande data från undersökningens mätningar: laddningstid, antal resurser som ska laddas, sidans totala storlek, prestationspoäng, tid tills första innehållsrenderingen, tid tills största uppritningen av innehåll, tid till interaktivitet, summan av alla tidsperioder mellan FCP och tid till interaktivt tillstånd, samt kumulativ layoutförskjutning.</p> <p>Jag använde mig av två verktyg för att göra mina mätningar. Först mätte jag laddningstid, antal resurser samt hemsidans totala storlek med hjälp av firefox devtools under fliken networks. Jag laddade om sidan flera gånger med ctrl + shift + r eller ”forced reload” för att inte ladda sidan via cache och dokumenterade sedan snittet i ett Excel-ark. Resten av datan samlade jag in med hjälp av Googles verktyg PageSpeed Insights. Jag fokuserade främst på labdatan som baseras på en simulerad belastning av en sida på en enda enhet och en fast uppsättning nätverksförhållanden, och dokumenterade även det i samma Excell-ark.</p>
    </div>
        <hr style="width:100%">
    <div class="analysis">
      <h2>Analys</h2>
      <p>Sveriges radios hemsida fick den bästa prestationspoängen av de tre hemsidorna med 39/100 för mobila enheter och 82/100 för desktop. Hemsidan skulle förbättra sin laddningstid främst genom att ta bort JavaScript som inte används, både för desktop och mobila enheter. Genom att göra så förväntas tidsbesparingen bli en halv sekund för desktop, alltså cirka 21% av laddningstiden och 1.05 sekunder för mobila enheter, detta är cirka 38% av laddningstiden enligt mina mätningar. Laddningstiden hade också blivit betydligt bättre för hemsidan på mobila enheter genom att ta bort oanvänd CSS samt resurser som blockerar renderingen, och genom att undvika att skicka äldre JavaScript till moderna webbläsare. Det Sveriges Radio verkligen skulle behöva göra är att rensa upp och uppdatera sin hemsida för mobila enheter, då det skulle minska laddningstiden med mer än 60% om jag utgår ifrån snittet av mina mätningar. Jag antar att SR kanske har satsat mer på att ha en snabb app, då många lyssnar på poddar och radio genom just appar som är skapta för det istället för genom respektive hemsidor.</p>
      <p>Expressens hemsida fick helt okej prestationspoäng med 39/100 för mobila enheter och 70/100 för desktop. Denna hemsida har också stor möjlighet att förminska sin laddningstid genom att ta bort JavaScript som inte används, framförallt för mobila enheter. Det hade minskat laddningstiden med 37% enligt mina mätningar. Och det finns även här en tidsbesparing att göra genom att undvika att skicka äldre JavaScript till moderna webbläsare. För desktop går det att minska laddningstiden genom att skjuta upp inläsningen av bilder som inte visas tills dess att de viktiga resurserna har blivit inlästa och tiden till interaktivt tillstånd minskar. Detta kommer även göra användarupplevelsen bättre. För att förbättra mobildataförbrukningen och inläsningstiden är det viktigt att skicka bilder i rätt storlek. Expressens hemsida är fylld av bilder och ibland är de inte i rätt bildformat och storlek, så detta är därför något de skulle kunna jobba med för att få en snabbare hemsida.</p>

      <p>VICE var hemsidan med sämst prestationspoäng med 8/100 för mobila enheter och 37/100 för desktop. Detta beror nog delvis på att laddningstiden är nästan tre gånger så lång som hos de andra två hemsidorna. Innan hemsidan är fullständigt interaktiv tar det i snitt cirka 22 sekunder för mobila enheter och cirka 5 sekunder för desktop, vilket är dubbelt så mycket som för de andra två sidorna. Detta beror antagligen på att VICE hemsida är betydligt större. Även på denna hemsida finns det störst potential för tidsbesparing genom att ta bort JavaScript som inte används. På mobila enheter hade det gått 2.85 sekunder snabbare och 0.5 sekunder snabbare på desktop. Precis som på Expressens hemsida kan man även minska laddningstiden genom att undvika att skicka äldre JavaScript till moderna webbläsare. Utöver det bör textresurser skickas komprimerade så att färre byte skickas via nätverket. Bilderna bör även hållas i rätt storlek. Bildformat som JPEG 2000, JPEG XR och WebP ger ofta bättre komprimering än PNG eller JPEG. Det gör att nedladdningen går snabbare och ger minskad dataförbrukning.</p>
      <p>Vanligaste förbättringsåtgärden för de tre hemsidorna är att ta bort JavaScript som inte används, speciellt för mobila enheter. Där finns det mycket tid att vinna. Att undvika att skicka äldre JavaScript till moderna webbläsare är också något alla tre bör göra. Genom att använda JavaScript-paket kan man även använda en strategi för skriptimplementering, som även stödjer äldre webbläsare, där registrering av funktioner med eller utan moduler används för att minska mängden kod som skickas till moderna webbläsare. Ett annat sätt att minska laddningstiden på hade varit att använda modernare bildformat som JPEG 2000, JPEG XR och WebP som ofta ger bättre komprimering än PNG eller JPEG.</p>
    </div>
        <hr style="width:100%">
    <div class="other">

      <p>När jag själv har testat dessa tre hemsidor på min laptop och mobil har jag inte märkt jättestor skillnad mellan de tre, förutom att VICE kändes lite segare. När det kommer till olika laddningstid är jag som många andra att jag inte riktigt har tålamod när en sida laddar långsamt. Jag tror nog att min gräns, innan jag kryssar sidan, går vid ungefär fem sekunder, men jag hinner bli irriterad efter tre. Så om jag utgår från det klarade Expressen och Sveriges Radio sig bäst. När hemsidorna väl hade laddat upplevde jag att Expressens hemsida var minst trevlig. Den kändes långsammare än vad den var på grund av de enorma annonserna, och de många bilderna och videorna i flera olika storlekar, som behöver ladda när man skrollar. Trots att VICE hemsida låter en vänta tycker jag att layouten och innehållet får det att kännas mer okej. De använder skärmens storlek på ett bättre sätt än Expressen, viket gör att den känns lättare att använda och behagligare för ögat. Sveriges Radios hemsida känns rätt snabb och lätt att använda, vilket är skönt och får en att vilja stanna på hemsidan. Däremot tycker jag att den är rätt tråkig färgmässigt, det händer inte så mycket med layouten, så det finns definitivt plus och minus. Men jag väljer ändå Sveriges Radio som vinnare i undersökningen när jag utgår från min egen upplevelse.</p>
      <p>Av: Sofia Herelius</p>
    </div>
</div>


<div class="result">
<a href="https://docs.google.com/spreadsheets/d/12pmtGvvx3OwpVI7uyk0be4s0UTppL5j7T5e2SlWtE6Q/edit?usp=sharing" target="_blank"><p class="r-link">Klicka här för att se datan från mätningarna!</p></a>

<a href="https://sverigesradio.se/"><h2>Sveriges Radio:</h2></a>
<div class="mini">
    <img class="page-img load sr" src="../assets/img/sr.png">
    <h1 class="centered">Vinnaren!</h1>
</div>
<div class="result-txt">
    <p>Hemsidan skulle förbättra sin laddningstid främst genom att ta bort JavaScript som inte används, både för desktop och mobila enheter. Genom att göra så förväntas tidsbesparingen bli en halv sekund för desktop, alltså cirka 20% av laddningstiden, och 1.05 sekunder för mobila enheter, vilket är cirka 38% av laddningstiden enligt mina mätningar.</p>
</div>

<a href="https://www.expressen.se/"><h2>Expressen:</h2></a>
<div class="mini">
    <img class="page-img load" src="../assets/img/expressen.png">
    <h1 class="centered">2</h1>
</div>


<div class="result-txt">
    <p>Expressens hemsida har stor möjlighet att förminska sin laddningstid genom att ta bort JavaScript som inte används. Det finns även här en tidsbesparing att göra genom att undvika att skicka äldre JavaScript till moderna webbläsare. För desktop går det att minska laddningstiden genom att skjuta upp inläsningen av bilder som inte visas tills dess att de viktiga resurserna har blivit inlästa och tiden till interaktivt tillstånd minskar.</p>
</div>

<a href="https://www.vice.com/en"><h2>VICE:</h2></a>
<div class="mini">
    <img class="page-img load" src="../assets/img/vice.png">
    <h1 class="centered">3</h1>
</div>

<div class="result-txt">
    <p>VICE hemsida har störst potential för tidsbesparing genom att ta bort JavaScript som inte används, men också genom att undvika att skicka äldre JavaScript till moderna webbläsare. Utöver det bör textresurser skickas komprimerade så att färre byte skickas via nätverket och bilderna bör också hållas i rätt storlek. </p>
</div>
<div class="winner-txt">
      <p>Jag utgår från mätningarnas data och utser Sveriges Radios hemsida till vinnaren i denna undersökning. Prestationspoängen var bäst och desktop-versionen är den enda av hemsidorna som klarade granskningen i diagnosrapporten om huvudvärden på webben, där man granskar webbsidors prestanda utifrån faktisk användning. Därefter kommer Expressen och sist VICE.<p>
</div>
</div>
