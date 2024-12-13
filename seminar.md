Fråga 1: Skillnaden som vi sett från start är att Aizo har fler spärrar, han ställer frågor och vill att man själv ska tänka själv. Medans ChatGPT ger ut direkt svar på hur den applicerar metoderna på spelet och gav oss flera exempel på hur man skulle kunna koda upp spelet i python och java medans Aizo tog en annan approach med att gå vidare med att istället börja vägleda oss mot att skriva upp programmet.

Fråga 2: Vi behövde att förtydliga spelets regler för både Ai'sen för att de skulle förstå spelets regler och de har liknande kod men det är mer tydligt skrivet med ChatGPT. Den sist nämnande använder indenteringar och = tecken som påminner av vanlig kod till exempel.

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

Fråga 3: Båda misstolkade instruktionerna för spelet och behövde påmminas, Chatgpt gav kod som inte fungerade medans Aizo gav oss en korrekt kod som fungera men med ett resultat på 10,000 + slag innan spelet vart slutfört.

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

Fråga 4: Vi tror att om man är ordentlig med sina promptar så kommer bottarna att skriva ut bättre kod, vi misstänker att ChatGPT kommer att vara bättre i ett större projekt om man skulle låta den göra majoriteten av arbetet. Medans Aizo vill ha mer regulbunden input och frågor oss vad vi tror skulle våra bra, och ärd mer användar om man vill ha hjälp med mindre snuttar av koden.
Vi har också upptäckt att ChatGPT är bättre på att komma ihåg konversationer medans Aizo "glömmer bort" och behöver påminnas.

Fråga 5: Båda botterna förklarar väl vad de olika värdena betyder fast med annan olika ord och tonalitet. Aizo använder mer emojis för att vara lite rolig och uppmuntrar att man ska testa att justera värdena själv för att se vad som händer. ChatGPT gav oss även en egen html kod som exempel med en förklaring på hur box-shadow påverkar elementet.

Fråga 6:
När man jobbar i redan befinitliga projekt kanske den består av äldre versioner av kod som man måste förhålla sig till. ChatGPT är inmatad med den tidigare versionen av AWS SDK som är den andra versionen men det finns en version 3 av AWS SDK där promise inte längre behövs användas. Den tredje versionen är nyare och på de projekt som finns ute använder majoritet den andra versionen så den har fortfarande bra funktionalitet och det är lite onöndigt att skriva om koden och uppdatera till den tredje versionen.

Fråga 7:
Nybörjar versionen var mer kopplad till mer till vardagen för att man skulle kunna lättare sätta in sig i konceptet och det var även en kortare beskrivning på det hela. Vi fick även tips i slutet av svaret för att kunna hjälpa oss på traven så vi kan lättare lära oss om koncepten och den gav oss även exempel hur man använder det io programmering om man så ville veta.

Fråga 8:
En stor skillnad som vi såg är att koden är skriven på två helt olika sätt, den enklare versionen använde .map för att gå igenom strängen och kolla igenom alla positioner för att kolla igenom varje tecken medans den andra versionen kollade igenom med en loop istället. Vi tror även att den "svårare" versionen kan användas lättre till fler typer av scenarion än nybörjar versionen med .map.
