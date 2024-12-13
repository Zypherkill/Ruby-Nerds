<h1>AI Seminarium</h1>

<h2>Fråga 1:</h2>
Skillnaden som vi sett från start är att Aizo har fler spärrar, han ställer frågor och vill att man själv ska tänka själv. Medans ChatGPT ger ut direkt svar på hur den applicerar metoderna på spelet och gav oss flera exempel på hur man skulle kunna koda upp spelet i python och java medans Aizo tog en annan approach med att gå vidare med att istället börja vägleda oss mot att skriva upp programmet.

<h2>Fråga 2:</h2>
Vi behövde att förtydliga spelets regler för både Ai'sen för att de skulle förstå spelets regler och de har liknande kod men det är mer tydligt skrivet med ChatGPT. Den sist nämnande använder indenteringar och = tecken som påminner av vanlig kod till exempel.

```
funktion spelaStege():
    # Definiera startvärdet för sekvensen och antal kast
    mål = 1  # Första talet vi söker
    kast = 0  # Håll koll på antalet kast
    sekvens = []  # Håller koll på sekvensen vi får

    # Fortsätt tills vi får hela sekvensen 1, 2, 3, 4, 5, 6
    medan sekvens är inte lika med [1, 2, 3, 4, 5, 6]:
        kastaTärning()  # Kasta tärningen
        kast += 1  # Öka kastantalet

        om tärningens resultat är lika med mål:
            sekvens.add(mål)  # Lägg till mål i sekvensen
            mål += 1  # Gå vidare till nästa tal i sekvensen
        slutom

    # När sekvensen är klar, skriv ut antalet kast
    skriv ut "Antal kast: " + kast
    skriv ut "Sekvensen: " + sekvens
slutfunktion

funktion kastaTärning():
    # Generera ett slumptal mellan 1 och 6
    resultat = slumptal(1, 6)
    skriv ut "Tärningens resultat: " + resultat
    return resultat
slutfunktion
```

<h2>Fråga 3:</h2>
Båda misstolkade instruktionerna för spelet och behövde påmminas, Chatgpt gav kod som inte fungerade medans Aizo gav oss en korrekt kod som fungera men med ett resultat på 10,000 + slag innan spelet vart slutfört.

```
function rollDice() {
     return Math.floor(Math.random() * 6) + 1; }

 let targetSequence = [1, 2, 3, 4, 5, 6];
 let currentSequence = [];
 let attempts = 0;

 while (currentSequence.join('') !== targetSequence.join('')) {
     let roll = rollDice();
     console.log(`Du kastar: ${roll}`);
    
     if (roll === targetSequence[currentSequence.length]) {
         currentSequence.push(roll);
     } else {
         currentSequence = [];     }
    
     attempts++;
 }

 console.log(`Du fick rätt sekvens ${targetSequence.join(', ')} efter ${attempts} försök!`);
```

<h2>Fråga 4:</h2>
Vi tror att om man är ordentlig med sina promptar så kommer bottarna att skriva ut bättre kod, vi misstänker att ChatGPT kommer att vara bättre i ett större projekt om man skulle låta den göra majoriteten av arbetet. Medans Aizo vill ha mer regulbunden input och frågor oss vad vi tror skulle våra bra, och ärd mer användar om man vill ha hjälp med mindre snuttar av koden.
Vi har också upptäckt att ChatGPT är bättre på att komma ihåg konversationer medans Aizo "glömmer bort" och behöver påminnas.

<h2>Fråga 5:</h2>
Båda botterna förklarar väl vad de olika värdena betyder fast med annan olika ord och tonalitet. Aizo använder mer emojis för att vara lite rolig och uppmuntrar att man ska testa att justera värdena själv för att se vad som händer. ChatGPT gav oss även en egen html kod som exempel med en förklaring på hur box-shadow påverkar elementet.

<h2>Fråga 6:</h2>
När man jobbar i redan befinitliga projekt kanske den består av äldre versioner av kod som man måste förhålla sig till. ChatGPT är inmatad med den tidigare versionen av AWS SDK som är den andra versionen men det finns en version 3 av AWS SDK där promise inte längre behövs användas. Den tredje versionen är nyare och på de projekt som finns ute använder majoritet den andra versionen så den har fortfarande bra funktionalitet och det är lite onöndigt att skriva om koden och uppdatera till den tredje versionen.

<h2>Fråga 7:</h2>
Nybörjar versionen var mer kopplad till mer till vardagen för att man skulle kunna lättare sätta in sig i konceptet och det var även en kortare beskrivning på det hela. Vi fick även tips i slutet av svaret för att kunna hjälpa oss på traven så vi kan lättare lära oss om koncepten och den gav oss även exempel hur man använder det io programmering om man så ville veta.

<h2>Fråga 8:</h2>
En stor skillnad som vi såg är att koden är skriven på två helt olika sätt, den enklare versionen använde .map för att gå igenom strängen och kolla igenom alla positioner för att kolla igenom varje tecken medans den andra versionen kollade igenom med en loop istället. Vi tror även att den "svårare" versionen kan användas lättre till fler typer av scenarion än nybörjar versionen med .map.

<h2>Fråga 9:</h2>
Vi ser det som okej att avnända ai som ett litet bollplank och fråga om förklaringar på begrepp och funktioner eller ge ett exempel, vi ser Aizo som en extra handledare som finns tillgänglig när som helst. Vi tycker det inte är okej att använda ai till att skapa hela program, webbsidor till oss eller störra delar av kod som vi sen inte kan förklara/förstå och bara klistra in det.

<h2>Fråga 10:</h2>
En anledning är att man inte lär sig att koda om man bara kopierar och klistrar in, vi tycker att man inte ska göra sig för bekväm med att använda ai. Det kan vara så att ai'en inte har hela bilden på det problem vi vill lösa, för oss som studenter inte ska bygga för dåliga vanor med ai så vi i framtiden råkar läcka ut känslig information från ett företag.

<h2>Fråga 11:</h2>
Vi anser att man inte ska bli för bekväm med copilot som gör att det blir svårare att identifiera fel och som också gör det svårarare att förklara den kod man har skrivit, en styrka som vi ser är att få fler exempel på lösningar som inte kanske kommit på på egen hand. Det går betydligt snabbare att skriva koden förutsatt att man förstår det så man kan fokusera istället på att lösa problem.

<h2>Fråga 12:</h2>
Att efter en egen uppgift har lämnats in att gå tillbaka och använda github copilot för att få förslag på refaktuering och andra lösningar. Att man kan använda det för att snabba till processen av din kodning så vi inte behöver skriva knapp för knapp för att få fram resultat vi vill. Men vi ser att även vi som studenter ska vara försiktiga med att använda co-pilot och istället lära oss själva och ta hjälp av Aizo.

<h2>Fråga 13:</h2>
Det med att snabba på processen och ge andra förslag på lösningar och även göra så man kommenterar mer för att hjälpa andra som ska pyssla med koden eller bara för sig själv och att upptäcka nya paket och tekniker.

<h2>Fråga 14:</h2>
Vi tror att den mänskliga faktorn kommer alltid att vara en del av utvecklandet, vi matar ai'en med prompts för att kunna generera något typ av resultat. Vi ser det som ett verktyg för att bredda våra kunskaper och kunna arbeta med fler frågor an bara kod.

<h2>Fråga 15:</h2>
Att man till exempel tar för givet att ai'n skriver rätt och även som en säkerhetsfråga där man ger ut känslig eller viktigt information från det företag som man befinner sig på. Det kan även i dagsläget skrämma iväg kunder om man förlitar sig för mycket på ai med till exempel ai skriver text på en produkt sida.

<h2>Fråga 16:</h2>
<h3>Deep ai</h3>


