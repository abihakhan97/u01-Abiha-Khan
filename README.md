<!-- Från skiss till kod -->

Jag började med att skapa de olika HTML-filerna och CSS-filen. Sedan länkade jag ihop sidorna i en provisorisk navigaton och länkade css filen till HTML-filerna, som jag har total fem stycken av.
Eftersom jag skulle börja med mobile first tänkte jag kolla på de olika sidorna i skissen, för att kunna se vilka delar var som viktiga på varje sida. Efter att ha kollat på Figma och skissens storlek för mobilesidan kunde jag lägga till att mobileversion skulle vara maximalt 600 px bred.
Sedan hittade jag en bild för att lägga till den på startsidan och började arbeta med stylingen. Jag valde att döpa den till home.html eftersom jag tyckte det var lättare att komma ihåg och gav på HTML-filerna mer enhetlig namn.

<!-- Semantik -->

På varje HTML-sida finns ett sidhuvud <header> med en egengjord logotyp (aks007), navigationen och en dropdown-meny med en knapp <button>. Jag ändrade länkarna till sociala medier från Pawans version för att länka till mina egna konton.
Jag använde <nav> för att samla navigationslänkar och markera dem som sidans navigationen. Det gör strukturen tydligare, även för skärmläsare. Med CSS kunde jag senare ändra navigationen från vertikallt till horisontell.
Sedan använde jag <div> för att gruppera olika delar, som ikonerna för sociala medier och styra deras placering med CSS. Jag valde <div> eftersom jag behövde en behållare för layouten utan nagån särskild semantisk betydelse.
Jag har lagt till en main-tag efter sidhuvudet på alla HTML-sidor för att hålla strukturen enhetlig. Main-taggen blev också tillagd för att definera huvudinnehåll på sidorna.
I slutet av varje HTML-sida finns en sidofot <footer> som centreras på samma sätt som i skissen, men jag har lagt till min egen touch i texten.

<!-- Layout -->

För att placera navigationslänkarna vertikalt använde jag Flexbox med flex-direction: column. Jag valde Flexbox eftersom länkarna skulle ligga under varandra i en riktning. Detta gjorde det enkelt att styra deras placering. Jag använde också padding för att skapa utrymme inuti elementen. Desutom använde jag Grid på projektsidan men tech stack-sidan för att placera projektkorten respektive teknikikonerna bredvid varandra.
Enligt instruktionerna började jag med mobillayouten och valde 600 px som brytpunkt med utgångspunkt i mobilskissen i Figma. Jag gjorde sidan responsiv genom att lägga till media queries för att anpassa layouten till desktopversionen. I skissen visades två projekt i mobilversionen och sex i desktopversionen, vilket jag föjlde i min layout. På större skärmar fanns det mer utrymme för projekten, samt att bilderna ändrades i desktopversionen. Dessutom ändrade jag navigationen från en vertikal till en horisontell layout och justerade färgerna och stylingen. Navigationen blev strukturerat främst med Flexbox i mobilläge och Grid i desktopläge.

<!-- Tillgänglighet -->

JJag har testat sidorna med utvecklarverktygen i Chrome och gjort en Lighthouse-analys som gav 100 av 100 poäng för tillgänglighet.
Jag testade också att navigera utan mus med Tab och Enter. Testet visade att jag kunde nå och aktivera alla länkar. Med :focus-visible i CSS gjorde jag fokusmarkeringen tydligare, så att det syntes vilken länk som hade fokus.
Jag har lagt till alt-texter på bilderna och logotyperna. De beskriver bildernas innehåll för personer som använder skärmläsare och kan även visas om bilderna inte laddas korrekt.
I dark mode blir ikonernas färger omvända för att synas bättre. Rubrikerna och texten blir vita för att vara lättare att läsa mot den mörka bakgrunden.
Det som kan förbättras är textfärgen i light mode. Vissa grå textdelar kan vara svåra att läsa, och en mörkare textfärg skulle kunna göra dem tydligare.

<!-- Användbarhet -->

I skissen känner jag igen principen om konsekvens, exempelvis genom att navigationen har samma utformning på alla sidor. Det skapar igenkänning och gör det lättare att navigare på vaje sida. Uppdelningen av texten i rubriker och stycken, gör sidorna välstrukturerade.
I skissen används närhetsprincipen genom att sammanhörande rubriker och bilder placeras nära varandra, vilket visar att de hör ihop.
En ändring jag skulle ha gjort är att lägga till en knapp för att visa fler projekt i mobilläge. Då skulle besökaren kunna ta del av alla projekt även på mobilen, utan att all information behöver visas direkt.

<!-- Styrkor och brister -->

En styrka är att jag följden skissen så bra som jag kunde och använde metoden för att testa tillgänglighet som vi lärde oss på lektionerna och workshopen. Det var enkelt att använda Tab och Enter för att navigera genom sidorna och man kunde tydligt ser vilken länk som hade fokus innan man aktiverade den.
Det jag kan förbättra är läsbarheten i light mode genom att välja mörkare textfärger för att öka kontrasten. Jag skulle vilja lägga till fler klickbara element på projektsidan, exempelvis möjligheten att öppna varje projekt, läsa en beskrivning och bläddra bland bilder och skärmdumpar från projektet. Detta skulle ge besökaren en tydligare bild av varje projekt. Genom att låta besökaren öppna projekten skulle jag kunna inkludera fler bilder och beskrivningar, samtididgt som projects.html visar mindre information från början.

<!-- AI-verktyg -->

Jag använde mig av ChatGPT när jag behövde förstå hur jag skulle använda vissa funktioner och för att felsöka när koden inte fungerade. För det mesta var det några punkter (.) eller semikolon (;) som saknades. Någon annan gång gjorde jag en felstavningen i CSS där HTML-taggen inte blev kopplad på grund av felstavningen. Sedan var jag osäker på hur man enklast skulle lägga till typsnitten som fanns med på Figma-skissen.
Jag försökte korskontrollera vissa svar som jag fick av ChatGPT med hjälp av W3Schools och Google-sökningar. Jag bad AI att förklara vad de olika funktionerna gör så att jag kunde testa på egen hand och lära mig bättre. Några förslag från ChatGPT var fel men jag kunde kolla upp det med Google eller W3Schools.
Jag lärde mig framför allt att man ska vara noggrann när man skriver klassnamn i CSS, att man inte kan glömma en punkt före klassnamnet och att man bör avsluta varje CSS-deklaration med ett semikolon.
