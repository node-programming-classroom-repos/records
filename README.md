# Uppgift klasser och objekt - simulation av artister och skivbolag

## Syfte
Syftet med uppgiften är du ska hantera klasser, relationer mellan klasser samt objekt/instanser av klasser.
Kortfattat så ska du implementera grunden för ett system som simulerar artister, skivbolag, användare och album med låtar. 
Det finns inget medföljande jest-test - du ska implementera din lösning enligt instruktioner och krav i den här uppgiften.
Du kommer att bedömas enligt kraven nedan samt på korrekt användning av klasser och objekt och övergripande funktionalitet. Bedömningen kommer också att ta hänsyn till struktur i din kod, inklusive indentering, namngivning och övergripande struktur.

## Krav
Systemet du ska implementera är alltså klasser för att hantera artister, album, låtar, genrer, skivbolag och användare. En användare ska kunna spela låtar 
Notera att lösningen ska uppfylla krav på följande relationer mellan klasserna;
- skivbolag "har"/innehåller FLERA album. 
- album "har"/innehåller FLERA låtar och EN artist.
- en artist "har" en genre.
- ett album "har" en genre.
- respektive klass ska implementeras i en separat fil.
- skriv beskrivande, korta och koncisa kommentera varje fil; exmpelvis för varje metod i klasserna. Skriv kommentarer i app.js som gör det enkelt att följa flödet och vad som händer i det scriptet.


Implementera klasserna enligt nedan:


    Artist
    ======

    klassen ska representera en artist/band.
    attribut ska finnas för
    - id, name, genre och bio (biogragi/text om artisten/bandet).
    - implementera en metod för att visa/skriva ut information om artisten. 



    Genre
    ======
    
    klassen Genre representerar en genre för en musikstil.
    - attribut för id och name ska finnas.
    - implementera en metod som skriver ut/visar information om objektet

    

    Album
    =====

    representerar ett album med låtar (Song-objekt)
    - attribut för klassen ska vara id, title, artist, genre och songs (vilket ska vara en array med Song-objekt).
    - implementera en metod för att visa/skriva ut all information om albumet, inklusive genre och dess låtar (alla låtar som tillhör albumet, dvs Song-objekten, ska också visas/skrivas ut).
    - implementera en metod addSong, som lägger till en låt (ett Song-objekt) till albumet


    
    Song
    =====
    klassen Song ska representera en låt.
    - attributen ska vara id, title och playCount.
    - implementera en metod för att "spela" låten och öka playCount (playCount är alltså en räknare för antal spelningar/streams av låten).
    - implementera en metod som returnerar värdet för playCount
    - implementera en metod för att visa/skriva ut information om låten.



    RecordLabel
    =====
    klassen RecordLabel representerar ett skivbolag. Ett skivbolag äger rättigheter til album vilket ska representeras av ett attribut med Album-objekt.
    - attributen ska vara id, name, headOfficeAddress, albums (en array med Album-objekt)
    - implementera en metod för att visa/skriva ut information om skivbolaget.



    User
    ======
    denna klass representerar en användare som spelar låtar  
    - attributen som ska implementeras ska vara id, name och playedSongs (en array för att hålla reda på vilka låtar användaren har spelat).
    - implementera en metod för att spela en låt och håller reda på vilka låtar användaren har spelat.
    - implementera en metod för att visa/skriva ut användarinformation.
    - implementera en metod som kan visa information/skriva ut vilka titlarna på de låtar (Song) en användare har spelat/lyssnat på.



    app.js
    =====
    Detta script ska vara "systemets"/din lösnings entry point (main).
    Den ska kunna köras med kommandot $node app.js utan fel och innehålla följande;
    
    I scriptet ska du skapa några genrer, skivbolag, artister, album och låtar.
    Skriv ut information om respektive objekt du skapar via dess metoder som ska visa/skriva ut information. 
    Skapa några användare (user objekt) som var och en spelar ett antal olika låtar.
    
    

    
**Frivilligt**
Följande är inget krav, men för dig som redan har kunskaper och vill göra extra kan implementera nedanstående:

- Implementera möjligheten att lägga till nya genrer, skivbolag, artister, album och låtar i systemet.
- Vid körning av scriptet ska man kunna välja en genre och visa artister inom den genren.
- Vid körning av scriptet ska man kunnan välja en artist, visa dess album och låtar och låt användaren spela låtarna.        
- Implementera felhantering för ogiltiga inmatningar från användaren.
- Gör en webbapplikation med Express av din lösning. Gör 'sidor' och routes för ett låtbibliotek och möjlighet att spela låtar.
- Använd Spotifys API (om du har konto) för att skapa låtar, album etc med data ifrån Spotify.


