# records

Uppgiftens syfte är att hantera klasser och objekt.
Du ska simulera ett system med artister, skivbolag och album med låtar. 
En simulering av att artisternas låtar spelas av användare ska göras.
Syftet med uppgiften är att hantera klasser i separata filer samt relationer mellan klasser.

Systemet du ska implementera är alltså klasser för att hantera artister, album, låtar, genrer, skivbolag och användare. 
Notera att lösningen ska uppfylla krav på följande relationer mellan klasserna;
- skivbolag "har"/innehåller FLERA album 
- album "har"/innehåller FLERA låtar och EN artist.
- en artist "har" en genre
- ett album "har" en genre


Nedan följer detaljer för varje klass som du ska implementera.


**Ett krav är att varje klass nedan ska implementeras i en separat fil.
Du ska implementera klasserna enligt nedan krav.**




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
    - implementera en metod för att visa information om albumet, inklusive dess låtar (alla låtar som tillhör albumet, dvs Song-objekten, ska också visas/skrivas ut).
    - implementera en metod addSong, som lägger till en låt (ett Song-objekt) till albumet

    
    Song
    =====
    klassen Song ska representera en låt.
    - attributen ska vara id, title och playCount.
    - implementera en metod för att "spela" låten och öka playCount (playCount är alltså en räknar för antal spelningar/streams av låten).
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
    Detta script ska vara "systemets"/din lösnings entry point.
    
    I detta script ska du skapa några genrer, skivbolag, artister, album och låtar.
    Skriv ut information om respektive objekt du skapar via dess metoder som ska visa/skriva ut information. 
    Skapa några användare (user objekt) som var och en spelar ett antal olika låtar.
    
    Låt användaren välja en genre och visa artister inom den genren.
    Låt användaren välja en artist, visa dess album och låtar och låt användaren spela låtarna.
    Simulera beräkning av royalties efter att användaren har spelat låtarna.

    
**Frivilligt**
Följande är inget krav, men för dig som redan har kunskaper och vill göra extra kan implementera nedanstående:

- Implementera möjligheten att lägga till nya genrer, skivbolag, artister, album och låtar i systemet.        
- Implementera felhantering för ogiltiga inmatningar från användaren.
- Gör en webbapplikation med Express av din lösning. Gör sidor/routes för ett låtbibliotek och möjlighet att spela låtar.
- Använd Spotifys API (om du har konto) för att skapa låtar, album etc med data ifrån Spotify.


    Du kommer att bedömas på korrekt användning av klasser och objekt, implementation av royalties, användarinteraktion, genrehantering, skivbolasrelation och övergripande funktionalitet.

Kom ihåg att organisera koden i separata filer för varje klass och hålla den strukturerad. Lycka till med ditt utökade skivbolagssystem!
