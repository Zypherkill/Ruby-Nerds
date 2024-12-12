Fråga 1: Skillnaden som vi sett från start är att Aizo har fler spärrar som vill att man själv ska tänka medans ChatGPT ger ut direkt svar på hur den applicerar metoderna på spelet.

Fråga 2: Båda Ai'sen förstår vad spelet innebär och har liknande kod men det är mer tydligt skrivet med ChatGPT. Den sist nämnande använder inventeringar och = tecken som påminner av vanlig kod till exempel.

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
