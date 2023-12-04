# records

Uppgiftens syfte är att hantera klasser och objekt.
Du ska simulera ett system med skivbolag och deras artister med musik. En simulering av att artisternas låtar spelas av användare och royalties tillfaller skivbolag och artister (beroende på antal spelningar/streams).

Systemet ska hantera artister, album, låtar, genrer, skivbolag, royalties och användare. Nedan följer detaljer för varje klass.
Varje klass nedan ska implementeras i en separat fil.



    Artist
    ======

    klassen ska representera en artist/band.
    attribut ska finnas för
    - id, name, genre, royaltyPercentage (andel i procent av royalty som tillfaller artisten för en stream) och recordLabel (vilket skivbolag artisten tillhör).
    - implementera en metod för att visa information om artisten. 
    - implementera metoder som kan förändra royaltyPercentage och returnera royaltyPercentage



    Genre
    ======
    
    klassen Genre representerar en genre för en musikstil.
    - attribut för id och name ska finnas.
    - implementera en metod för att visa information om genren.

    

    Album
    =====

    representerar ett album med låtar (Song-objekt)
    - attribut för klassen ska vara id, title, artist, genre, recordLabel (en artist ska tillhöra *en* RecordLabel) och songs (vilket ska vara en array med Song-objekt).
    - implementera en metod för att visa information om albumet, inklusive dess låtar (Song-objekten).
    - implementera en metod addSong, som lägger till en låt (ett Song-objekt) till albumet

    
    Song
    =====
    klassen Song ska representera en låt.
    - attributen ska vara id, title och playCount.
    - implementera en metod för att spela låten och öka playCount.
    - implementera en metod som returnerar värdet för playCount - getPlayCount
    - implementera en metod för att visa information om låten.


    Royalty
    =====
    Skapa en klass Royalty som hanterar beräkningen av royalties baserat på antalet spelningar och artistens procentsats.
    Klassen ska också kunna hantera beräkningen av royalties baserat på antalet spelningar och skivbolagets procentsats.
    - implementera en metod för att beräkna royalties. Metoden ska heta calculateRoyalties.


    RecordLabel
    =====
    klassen RecordLabel representerar ett skivbolag.
    - attributen ska vara id, name och royaltyPercentage (vilket är den procentandel av artistens intäkter skivbolaget tar).
    - implementera en metod för att visa information om skivbolaget.

    User
    ======
    denna klass representerar en användare som spelar låtar (Song) 
    - attributen som ska implementeras ska vara id, name, balance och playedSongs (en array för att hålla reda på vilka låtar användaren har spelat).
    Implementera en metod för att spela en låt och minska användarens saldo.
    Implementera en metod för att visa användarinformation.

    app.js
    =====
    Detta script ska vara "systemets"/din lösnings entry point.
    
    I detta script ska du skapa några genrer, skivbolag, artister, album och låtar.
    Skriv ut information om respektive objekt du skapar via dess metoder som ska visa information. 
    Skapa några användare (user objekt) som var och en spelar ett antal olika låtar.
    
    Låt användaren välja en genre och visa artister inom den genren.
    Låt användaren välja en artist, visa dess album och låtar och låt användaren spela låtarna.
    Simulera beräkning av royalties efter att användaren har spelat låtarna.

    Extra utmaning:
        Implementera möjligheten att lägga till nya genrer, skivbolag, artister, album och låtar i systemet.
        Implementera felhantering för ogiltiga inmatningar från användaren.

    Bedömning:

    Du kommer att bedömas på korrekt användning av klasser och objekt, implementation av royalties, användarinteraktion, genrehantering, skivbolasrelation och övergripande funktionalitet.

Kom ihåg att organisera koden i separata filer för varje klass och hålla den strukturerad. Lycka till med ditt utökade skivbolagssystem!
