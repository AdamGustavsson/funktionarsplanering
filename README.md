# Funktionärsplanering

En enkel webbapp för att schemalägga funktionärer på matcher, cuper och arrangemang. Perfekt för idrottsföreningar och eventarrangörer.

**[Öppna appen →](https://adamgustavsson.github.io/funktionarsplanering/)**

![Status](https://img.shields.io/badge/status-aktiv-brightgreen)
![Licens](https://img.shields.io/badge/licens-MIT-blue)

---

## Funktioner

### 📅 Evenemang
- Skapa och hantera evenemang med namn, datum och plats
- Kopiera gamla evenemang med nytt datum (behåller passupplägg)
- Separata listor för kommande och avslutade evenemang

### ⏰ Pass & Roller
- Skapa pass med starttid, sluttid och roller
- **Bulk-generering:** Skapa en hel dags pass automatiskt (t.ex. 09:00-17:00, 1 timme per pass)
- Flexibla roller: kiosk, entré, sekretariat, parkering m.m.

### 👥 Medlemmar
- Spara kontaktuppgifter (namn, telefon, e-post)
- Enkel import/export för delning mellan enheter

### 🤖 Automatisk bemanning
- Fördela pass jämnt mellan valda medlemmar
- Prioriterar sammanhängande pass för samma person
- Förhandsgranskning innan tilldelning

### 📊 Schema & Översikt
- **Tidslinjevy:** Visuell överblick med färgkodade roller
- **Listvy:** Detaljerad lista per pass
- Utskriftsvänligt format (A4 liggande)

### 💬 Meddelanden
- Generera personliga meddelanden per funktionär
- Redigerbar meddelandemall som sparas
- Skicka via WhatsApp, SMS eller e-post med ett klick
- Inkluderar komplett schema med telefonnummer för passbyte

### 📤 Export & Import
- Exportera data som JSON (medlemmar, roller, evenemang, pass)
- Importera och slå ihop eller ersätt befintlig data
- Perfekt för att dela upplägg mellan enheter eller personer

---

## Kom igång

### Använda online
1. Öppna [appen](https://adamgustavsson.github.io/funktionarsplanering/)
2. Lägg till medlemmar och roller
3. Skapa ett evenemang och generera pass
4. Tilldela funktionärer och skicka meddelanden

### Installera som app på mobilen
**iPhone/iPad (Safari):**
1. Tryck på Dela-ikonen (□↑)
2. Välj "Lägg till på hemskärmen"
3. Tryck "Lägg till"

**Android (Chrome):**
1. Tryck på menyn (⋮)
2. Välj "Installera app" eller "Lägg till på startskärmen"

### Köra lokalt
Ingen installation krävs – öppna bara `index.html` i en webbläsare.

```bash
# Klona repot
git clone https://github.com/adamgustavsson/funktionarsplanering.git

# Öppna filen
open index.html
# eller
python -m http.server 8000  # och besök localhost:8000
```

---

## Teknisk information

### Arkitektur
- **100% klientsida** – ingen server eller backend
- **Självcontained HTML** – en enda fil med all CSS och JavaScript
- **localStorage** – all data sparas lokalt i webbläsaren

### Beroenden
- [Remix Icon](https://remixicon.com/) (CDN) – ikoner

### Datalagring
All data sparas i webbläsarens localStorage under nyckeln `funktionarsplanering`. Data stannar på enheten och skickas aldrig till någon server.

**Tänk på:**
- Data rensas om du rensar webbläsardata
- Använd export-funktionen för backup
- Varje enhet/webbläsare har sin egen data

---

## GDPR & Integritet

Appen hanterar personuppgifter (namn, telefon, e-post) lokalt på din enhet.

- ✅ Ingen data skickas till externa servrar
- ✅ Du har full kontroll över all data
- ⚠️ Säkerställ samtycke från personer vars uppgifter du sparar
- 🗑️ "Radera all data"-funktion finns i appen

---

## Bidra

Förbättringsförslag och buggrapporter är välkomna! Öppna ett [issue](https://github.com/adamgustavsson/funktionarsplanering/issues) eller skicka en pull request.

---

## Licens

MIT License – Använd fritt för privat och kommersiellt bruk.
