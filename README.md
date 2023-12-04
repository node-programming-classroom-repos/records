# records

Uppgiften Skivbolagssystem med Artister, Album, Låtar, Genrer, Skivbolag, Royalties och Användare

Du ska skapa ett interaktivt skivbolagssystem i Node.js med klasser och objekt. Systemet ska hantera artister, album, låtar, genrer, skivbolag, royalties och användare. Nedan följer detaljer för varje del av systemet:

    Artistklassen (Artist):
        Skapa en klass Artist med egenskaper som id, name, genre, royaltyPercentage och recordLabel (vilket skivbolag artisten tillhör).
        Implementera en metod för att visa information om artisten.

    Genreklassen (Genre):
        Skapa en klass Genre med egenskaper som id och name.
        Implementera en metod för att visa information om genren.

    Albumklassen (Album):
        Skapa en klass Album med egenskaper som id, title, artist, genre, recordLabel och songs (en array av låtar).
        Implementera en metod för att visa information om albumet.

    Låtklassen (Song):
        Skapa en klass Song med egenskaper som id, title och playCount.
        Implementera en metod för att spela låten och öka playCount.
        Implementera en metod för att visa information om låten.

    Royaltyklassen (Royalty):
        Skapa en klass Royalty som hanterar beräkningen av royalties baserat på antalet spelningar och artistens procentsats.
        Implementera en metod för att beräkna royalties.

    Skivbolagsklassen (RecordLabel):
        Skapa en klass RecordLabel med egenskaper som id, name och royaltyPercentage (vilket är den andel av artistens intäkter skivbolaget tar).
        Implementera en metod för att visa information om skivbolaget.

    Användarklassen (User):
        Skapa en klass User med egenskaper som id, name, balance och playedSongs (en array för att hålla reda på vilka låtar användaren har spelat).
        Implementera en metod för att spela en låt och minska användarens saldo.
        Implementera en metod för att visa användarinformation.

    Huvudprogrammet (app.js):
        Skapa några genrer, skivbolag, artister, album och låtar.
        Låt användaren välja en genre och visa artister inom den genren.
        Låt användaren välja en artist, visa dess album och låtar och låt användaren spela låtarna.
        Simulera beräkning av royalties efter att användaren har spelat låtarna.

    Extra utmaning:
        Implementera möjligheten att lägga till nya genrer, skivbolag, artister, album och låtar i systemet.
        Implementera felhantering för ogiltiga inmatningar från användaren.

    Bedömning:

    Du kommer att bedömas på korrekt användning av klasser och objekt, implementation av royalties, användarinteraktion, genrehantering, skivbolasrelation och övergripande funktionalitet.

Kom ihåg att organisera koden i separata filer för varje klass och hålla den strukturerad. Lycka till med ditt utökade skivbolagssystem!
