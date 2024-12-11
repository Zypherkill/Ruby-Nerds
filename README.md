# Ruby-Nerds

<h1>Sammanfattning</h1>

<h2>Decomposition</h2>

Vi tolkade skissen som att kaffemenyn var huvudsidan. Genom navigationen (hamburgermenyn) kan användaren ta sig till fler delar av appen. Vi bedömde att orderhistoriken endast kunde visas i inloggat läge samt att användaren skickas till orderhistoriken när nedräkningen avslutas. Om användaren genomför en beställning i inloggat läge utgår vi från att kunduppgifter och betalningsinformation är förifyllda uppgifter.

<h2>Pattern recognition</h2>

Pattern recognition handlar om att hitta likheter mellan problem. Varje gång användaren genomför ett köp krävs information om betalning och leverans. För att förenkla för användaren finns alternativet att skapa ett konto. Där sparas dessa uppgifter och kan återanvändas vid varje ny order. 

Samma uppgifter finns också tillgängliga när användaren går in på “mina sidor” för att ändra uppgifter. Vissa av uppgifterna, till exempel mailadress, kan även användas för att skicka ut olika typer av meddelanden. Det kan röra sig om allt från att återställa ett lösenord till nyhetsbrev eller orderbekräftelser.

Även om skissen inte innehåller funktionen “glömt lösenord” utgår vi från att det är en funktion som kommer ingå i den slutliga produkten. Det är en vanlig del av digitala tjänster som många har behov av.

I menyn så finns en detaljerad beskrivning av innehållet i varje produkt för att hjälpa användaren att smidigt välja prefererad produkt eller undvika produkter som de  kan vara allergiska mot.

<h2>Abstraction</h2>

Abstraction är konsten att filtrera ut de stora dragen i en digital tjänst och skala bort allt oväsentligt. Den här tjänsten säljer kaffe, vilket innebär att det finns någon form av databas som hanterar produkterna. Vilken typ av produkter det rör sig om är ovidkommande. Däremot måste det gå att lägga till produkter och placera dem i kategorier av olika slag. 

Det ska även fungera att hämta information (produkter) och lägga till i olika listor. Det kan till exempel vara en lista som är en kunds order. Abstraction är alltså möjligheten att lägga till information och sedan hämta den. Pattern är en fördjupning. Exempel på patterns är att systemet kan använda köphistorik för att visa favoritprodukter eller för att visa hur mycket en kund har handlat för den senaste månaden.

Ett annat exempel är att inloggningen följer ett mönster. Användaren får feedback på om mailadress och lösenord är korrekt eller ej. En abstraction av samma fenomen är att systemet har möjlighet att skicka ut felmeddelanden.


<h2>Algoritm design</h2>

Algoritmer är steg- för steginstruktioner för en process. Vi har valt att beskriva en order från att användaren lägger en produkt i varukorgen till avslutad order. Processen kopplas till tidigare steg. Till exempel kan användaren välja att gå vidare till varukorgen eller att fortsätta handla och alltså gå bakåt i processen. På samma vis kan användaren gå från orderhistoriken till att göra om samma köp ytterligare en gång. 
