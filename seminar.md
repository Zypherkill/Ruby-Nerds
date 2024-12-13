Fråga 1: Skillnaden som vi sett från start är att Aizo har fler spärrar, han ställer frågor och vill att man själv ska tänka själv. Medans ChatGPT ger ut direkt svar på hur den applicerar metoderna på spelet och gav oss flera exempel på hur man skulle kunna koda upp spelet i python och java medans Aizo tog en annan approach med att gå vidare med att istället börja vägleda oss mot att skriva upp programmet.

Fråga 2: Båda Ai'sen förstår vad spelet innebär och har liknande kod men det är mer tydligt skrivet med ChatGPT. Den sist nämnande använder indenteringar och = tecken som påminner av vanlig kod till exempel.

```
START

spela = True
spela_till_slut = False

medan spela:
    Slå_tärning()  // Rullar tärningen för att få ett tal mellan 1 och 6
    visa_resultat()  // Visar resultatet av tärningsslaget

    om tärningsresultat är 1 eller 2:
        // Spelaren förlorar sin tur
        skriv_ut("Du förlorade din tur!")
        gå_tillbaks_nästa_tur()
    annars om tärningsresultat är 3 till 6:
        // Spelaren avancerar på stegen
        flytta_spelare(tärningsresultat)

        // Kontrollera om spelaren har nått slutet av stegen
        om spelaren_nått_slut():
            skriv_ut("Du har vunnit!")
            spela = False

    // Ny tur, om spelet inte är slut
    gå_tillbaks_nästa_tur()

SLUT
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
