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

Fråga 4: Vi tror att om man är ordentlig med sina promptar så kommer bottarna att skriva ut bättre kod, vi misstänker att ChatGPT kommer att vara bättre i ett större projekt om man skulle låta den göra majoriteten av arbetet. Medans Aizo vill ha mer regulbunden input och frågor oss vad vi tror skulle våra bra om man vill ha hjälp med mindre snuttar av koden. 
