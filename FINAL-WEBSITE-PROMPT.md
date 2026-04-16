# CLAUDE CODE — ULTIMATIVER WEBSITE-PROMPT
# bewusstseinsarchitektur.de · Julia Lauer
# Version FINAL

---

## AUFGABE

Erstelle eine vollständige, produktionsreife index.html für bewusstseinsarchitektur.de.
Baue von Grund auf neu — kein Recycling alter Dateien.
Ziel: die beste Single-Page-Website die du je gebaut hast.

---

## BRAND-IDENTITÄT

**Marke:** Bewusstseinsarchitektur · Julia Lauer
**URL:** bewusstseinsarchitektur.de
**Calendly:** https://calendly.com/zentrum-bewusstseinsarchitektur/30min

**Was sie tut:**
Julia Lauer ist Bewusstseinsarchitektin. Sie arbeitet 1:1 online mit hochleistenden Frauen
in Führung und Selbstständigkeit. Ihre Methode heißt Bewusstseinsarchitektur-Methode.
Sie arbeitet direkt im Unterbewusstsein — über das Zentrum, die übergeordnete innere
Instanz — ohne Hypnose, ohne Retraumatisierung, ohne Analysemarathon.

**Kernaussage:** Alles läuft. Aber es kostet.

**Zielklientin:**
Sara, 38. Selbständig. Familie. Trägt mentale und organisatorische Verantwortung für alles.
Funktioniert nach außen. Innerlich: Daueranspannung, Schlafprobleme, Körpersymptome.
Hat schon alles versucht. Sagt: "Ich bekomme es nicht weg."
Sie ist ROT-Typ: Leistung als Identität. Braucht Klarheit, nicht Heilungs-Sprech.

---

## FARB-SYSTEM (nicht verhandelbar)

```css
--bordeaux:    #2E0F14;   /* Primär · max. 2-3 Sektionen dunkel */
--terrakotta:  #B5603A;   /* Einziger Akzent · CTAs · Linien · Highlights */
--licht:       #FAF8F5;   /* Haupt-Hintergrund hell */
--weiss:       #FFFFFF;   /* Text auf Bordeaux */
--text-dunkel: #1A1A1A;   /* Fließtext auf hell */
--text-mittel: #4A4A4A;   /* Sekundärtext auf hell */
```

**Regeln:**
- Bordeaux: Hero, Quote-Sektion, finaler CTA, Footer
- Licht: alle anderen Sektionen
- Terrakotta: nur für Akzente, nie als Fläche
- Keine Verläufe. Kein Beige. Kein Grün. Kein Violett.
- Text auf Bordeaux: immer #FFFFFF, minimum font-weight 400 für kleine Texte

---

## TYPOGRAFIE

```
Google Fonts:
Cormorant Garamond: ital, wght 300+400
Jost: wght 300+400

Headlines / Display: Cormorant Garamond · Italic · 300
Fließtext: Jost · 300
Labels / Caps / kleine Texte: Jost · 400 · letter-spacing 0.2em
Buttons: Jost · 400

REGEL: Kein font-weight unter 300 für Fließtext, kein font-weight unter 400 für Texte unter 13px.
```

---

## BILDER

Alle Bilder liegen in: `C:\Users\sifu-\Desktop\CLAUDE_BEWUSSTSEINSARCHITEKTUR_2026`

**Zuweisung:**
- Hero (rechte Seite, Vollbild): `3H0A0008.jpeg` — Porträt, dunkel, direkt
- Problem-Sektion: `IMG_2795.JPEG` oder `IMG_2793.JPEG` — Kopf in Hand, erschöpft
- Über mich links: `Ballett_Julia.JPEG` — Schwarz-Weiß, Jung, dramatisch
- Über mich rechts unten: `IMG_7914.JPEG` — Blauer Pullover, ruhig, nachdenklich

---

## SEITENSTRUKTUR & TEXTE

### 00 · NAVIGATION (fixed)

Logo links: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic)
Links: Methode · Angebote · Über mich · FAQ
CTA rechts: `Klarheitsgespräch →` (Button, Terrakotta-Rand)

Verhalten: transparent auf Hero · weißer Hintergrund beim Scrollen

---

### 01 · HERO (Bordeaux · Vollbild · 100vh)

Layout: 2 Spalten — links Text, rechts Foto mit Bordeaux-Übergang

Label oben:
```
BEWUSSTSEINSARCHITEKTUR
```

Headline (Cormorant Garamond Italic, sehr groß):
```
Für Frauen,
die funktionieren —
und aufgehört haben zu spüren,
was es kostet.
```

Subtext:
```
Du trägst Verantwortung.
Du entscheidest.
Menschen verlassen sich auf dich.

Und lange funktioniert das auch.

Bis dein Körper irgendwann beginnt zu zeigen,
dass etwas unter der Oberfläche nicht mehr stimmt.

Nicht laut.
Eher leise.
Aber deutlich.
```

CTA Button:
```
Klarheitsgespräch anfragen →
```

Kleiner Text darunter:
```
0 € · 30 Minuten · Kein Verkaufsdruck
```

---

### 02 · PROOF BAR (Bordeaux · schmal)

3 Kennzahlen nebeneinander:
```
100+          |    3 Angebote    |    seit 2023
Klientinnen   |    ab 0 €        |    online, 1:1
```

---

### 03 · PROBLEM-SEKTION (Licht)

Layout: links Foto (3/4 Hochformat, mit Terrakotta-Rahmen-Offset), rechts Text

Headline:
```
Du hast schon vieles versucht.
Trotzdem ist es noch da.
```

Fließtext:
```
Meditation. Therapie. Urlaub. Bücher über Burnout.
Alles war hilfreich — für eine Weile.
Aber das Grundrauschen bleibt.
Die Anspannung. Das Nicht-abschalten-Können.

Du kommst nicht, weil du nicht mehr kannst.
Du kommst, weil du verstehst:
So will ich nicht weitermachen.
```

Liste (mit Terrakotta-Strich davor):
```
— Nachts wach, obwohl du erschöpft bist
— Körpersymptome ohne medizinischen Befund
— Das Gefühl, für alle da zu sein — außer für dich
— Leistung aus Zwang, nicht aus Kraft
— Du weißt, wie es laufen sollte. Trotzdem schaffst du es nicht.
— Noch nicht wach, schon auf der Hut
```

---

### 04 · REFRAMING (Bordeaux · zentriert)

Großes Zitat:
```
Vielleicht wurde dir irgendwann gesagt:
Du bist zu kontrollierend. Zu perfektionistisch. Zu viel.

Ich höre das anders.
```

Dann 5 Zeilen (Cormorant Italic, groß):
```
Kontrolle ist Organisationskraft.
Perfektionismus ist Qualitätswille.
Verantwortung ist Stärke.
Ausgleichen ist Fürsorge.
Harmonie halten — eine Kunst.
```

Darunter (Jost, klein):
```
Das sind keine Fehler. Das sind Kräfte.
Kräfte, die dich weit gebracht haben.

Das Problem ist nicht, wer du bist.
Sondern: Irgendwann dienen dir diese Kräfte nicht mehr.
Sie halten dein System rund um die Uhr unter Strom.
Und das kostet. Jeden Tag.
```

---

### 05 · METHODE (Licht)

Label: METHODE

Headline:
```
Ich arbeite nicht an deinen Symptomen.
Nicht an deinem Verhalten.
```

Einleitungstext:
```
Es bringt nichts, die Mitfahrer auszutauschen.
Wenn derselbe Fahrer am Steuer sitzt,
führt die Reise immer wieder an denselben Ort.

Darum arbeite ich direkt mit dem Fahrer.
```

Dann 3 Karten nebeneinander (Grid, Terrakotta-Linie unten beim Hover):

**Karte 1 — An der Wurzel**
```
Die Bewusstseinsarchitektur-Methode setzt dort an,
wo Muster tatsächlich entstehen.
Nicht im Denken. Nicht im Verhalten.
Sondern darunter. Im Unterbewusstsein.
```

**Karte 2 — Ohne Umweg**
```
Kein Analyse-Marathon.
Keine Ursachen-Odyssee.
Keine Retraumatisierung.

Wir gehen direkt dorthin,
wo diese Muster entstanden sind.
Und verändern sie dort.
```

**Karte 3 — Alles, was bleibt**
```
Alles, was du erlebt hast, hinterlässt Spuren.
Manche tief. Manche früh.
Wie Bernsteinstücke — eingefroren in dem Moment,
in dem sie entstanden sind.
Sie wirken weiter. Oft ohne, dass wir es merken.
```

Darunter breiter Text:
```
Die Ursache muss nicht bekannt sein.
Du musst nichts verstehen, bevor es sich verändert.
Das System weiß, wo es sitzt.
```

---

### 06 · WAS SICH VERÄNDERT (Licht · 2 Spalten)

Headline links:
```
Was sich verändert.
```

Kleiner Text links:
```
Vielleicht spürst du zuerst Müdigkeit.
Ein erstes Loslassen aus der dauernden Spannung heraus.

Dann wird es klarer.
Nicht dramatisch. Eher in kleinen Momenten.
```

4 Blöcke rechts (2x2 Grid):

**Körperlich**
```
Das Nervensystem beruhigt sich.
Die Symptome flachen ab.
Der Schlaf wird tiefer.
```

**Zwischenmenschlich**
```
Du nimmst deinen Partner wieder wahr.
Wählst bewusst, wann du Freunde treffen willst.
Kannst Grenzen setzen, ohne zu verletzen.
```

**Beruflich**
```
Du beendest ein großes Projekt.
Stehst vor dem Ergebnis.
Und sagst dir: Ja. Das habe ich gut gemacht.
```

**Innerlich**
```
Du reagierst nicht mehr automatisch.
Du atmest aus.
Und wählst.

Nicht weil du es dir antrainiert hast.
Sondern weil innen etwas anders geworden ist.
```

Großes Abschluss-Zitat darunter (Cormorant, zentriert):
```
Du weißt was du weißt.
Und das reicht.
```

---

### 07 · ANGEBOTE (Bordeaux)

Label: ANGEBOTE

Headline:
```
Wo möchtest du anfangen?
```

3 Karten nebeneinander. Mittlere (Deep Shift) hervorgehoben mit Terrakotta-Rand:

**Karte 1 — Klarheitsgespräch**
```
0 € · 30 Minuten

Du willst wissen, ob das hier das Richtige für dich ist.
Kein Pitch. Keine Agenda.
Wir schauen gemeinsam hin —
und du gehst mit einer klaren Einschätzung raus.

[Anfragen →]
```

**Karte 2 — Focus Shift (HERO · hervorgehoben)**
Tag: KERNANGEBOT
```
3.500 € · 12 Wochen · 6–8 Sessions · 1:1 online

Die tiefgreifendste Form der Zusammenarbeit.

Wir arbeiten nicht an Symptomen.
Wir ordnen dein System neu.

Meine Arbeit ist gut,
wenn du mich danach nicht mehr brauchst.
Nicht weil sie oberflächlich ist.
Sondern weil du lernst, dein eigenes System zu führen.
Ohne dauerhafte Begleitung.
Ohne Abhängigkeit.

[Klarheitsgespräch buchen →]
```

**Karte 3 — Focus Shift**
```
450 € · 2 Sessions · 1 Thema

Ein Thema. Zwei Sitzungen.
Ein gezielter Wendepunkt.

Für alle, die wissen, was sie bewegt —
und bereit sind, genau dort anzusetzen.

[Anfragen →]
```

---

### 08 · TESTIMONIALS (Licht)

Label: KLIENTINNENSTIMMEN

3 Zitate (große Cormorant Anführungszeichen, dann Text):

**Sarah L. · Unternehmerin**
```
„Ich habe funktioniert — aber innerlich war da ständig dieser Druck.
Nach unserer Arbeit war er weg. Einfach weg.
Und Dinge, die sich unmöglich angefühlt haben,
haben sich von allein gelöst."
```

**Elena C. · Projektleiterin**
```
„Ich habe nicht erwartet, dass sich mein Körper verändert.
Aber auch nicht, dass ich aufhöre,
mein Wohlbefinden von der Meinung anderer abhängig zu machen.
Beides ist passiert."
```

**Nadine H. · Ärztin**
```
„Die Schuldgefühle, die ich jahrelang mit mir getragen habe —
sie sind einfach nicht mehr da.
Ich weiß selbst nicht genau wie. Aber es ist so."
```

---

### 09 · ÜBER MICH (Licht · 2 Spalten)

Label: ÜBER MICH

Layout: links Ballett-Foto (Schwarz-Weiß, dramatisch) + kleines Foto unten rechts davon.
Rechts Text.

Headline:
```
Ich kenne dieses Muster.
Von innen.
```

Text:
```
Klassisches Ballett ab fünf Jahren.
Mit 13 München, Talentschmiede des Bayerischen Staatstheaters.
Leisten, funktionieren, psychosomatische Beschwerden —
über jede Grenze hinaus.

Mit 15 die Prüfung vor John Neumeier.
Der erkannte, was ich mir selbst vorher nicht eingestehen konnte.
Und stellte mir eine Frage:

Du kannst. Aber willst du das hier wirklich?

Danach: ALL-AACHT-Kampfkunst. Faszien. Atem. Somatik.
Jahrelange Körperarbeit mit Frauen.

Und immer wieder derselbe Punkt:
Symptome, die bleiben — egal wie präzise die Arbeit ist.
Weil ihre Ursachen woanders sitzen.

Das hat mich zur Yager Mind Matrix geführt.
Und zu der Erkenntnis,
dass Veränderung oft nicht dort passiert,
wo wir sie normalerweise suchen.

Daraus ist mein eigener Ansatz entstanden.
```

Kleines Zitat darunter (Terrakotta-Linie + Cormorant):
```
Yager ist der Ursprung.
Bewusstseinsarchitektur ist mein Weg.
```

---

### 10 · FAQ (Licht · Accordion)

Label: FRAGEN & ANTWORTEN

5 Fragen (öffnen/schließen per Klick):

**Für wen ist das gedacht?**
```
Für Frauen, die das Gefühl haben, mit dem Kopf allein nicht weiterzukommen.
Die innerlich an eine Grenze gestoßen sind und spüren,
dass da etwas ist, was sich verändern will.
Keine Vorkenntnisse nötig.
Nur die Bereitschaft, wirklich hinzuschauen.
```

**Wie läuft eine Sitzung ab?**
```
Jede Sitzung ist anders, weil jeder Mensch anders ist.
Wir starten dort, wo du gerade bist.
Was dich beschäftigt, was sich zeigt, was du mitbringst.
Von da aus arbeiten wir gemeinsam.
```

**Wie lange dauert der Prozess?**
```
Das lässt sich nicht pauschal sagen.
Manche spüren nach wenigen Sitzungen eine spürbare Veränderung,
andere brauchen mehr Zeit.
Wir schauen gemeinsam, was sinnvoll ist — ohne künstlichen Druck.
```

**Ich habe schon vieles versucht. Warum jetzt anders?**
```
Weil wir auf einer anderen Ebene arbeiten.
Nicht an dem, was du denkst oder weißt.
Sondern an dem, was sich festgehalten hat.
Manchmal braucht es einfach einen anderen Zugang.
```

**Ist das Therapie?**
```
Nein. Bewusstseinsarchitektur ist kein therapeutisches Verfahren
und ersetzt keine psychotherapeutische oder medizinische Behandlung.

Bei akuten psychischen oder körperlichen Erkrankungen
wende dich bitte an einen Arzt oder Therapeuten.
```

---

### 11 · FINALER CTA (Bordeaux · zentriert)

Label: BEREIT?

Headline:
```
Wenn du beim Lesen gemerkt hast,
dass irgendwo etwas in dir ruhig genickt hat —
dann können wir sprechen.
```

Text:
```
In einem Gespräch schauen wir gemeinsam,
ob diese Arbeit für dich passt.
```

Button:
```
Klarheitsgespräch anfragen →
```

Darunter 3 Garantien:
```
✓ Kostenlos   ✓ 30 Minuten   ✓ Kein Verkaufsdruck
```

---

### 12 · FOOTER (Bordeaux)

Links: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic)
Mitte: `© 2026`
Rechts: Impressum · Datenschutz

---

## DESIGN-PRINZIPIEN

**Typografie-Rhythmus:**
- Headlines: Cormorant Garamond Italic, groß, viel Luft
- Kurze Zeilen. Ein Gedanke pro Zeile wo möglich.
- Fließtext: Jost 300, 1rem, line-height 1.85
- Labels: Jost 400, 0.68rem, letter-spacing 0.22em, UPPERCASE

**Abstände:**
- Sektionen: padding-block clamp(5rem, 9vw, 9rem)
- Kein enger Textsatz — Luft ist Luxus

**Divider:**
- Terrakotta-Linie 48px, animiert beim Einblenden

**Animationen:**
- Scroll-Reveal: opacity 0 → 1, translateY 30px → 0, 0.8s ease
- Hero-Text: sequenzielles Einblenden mit Delay
- Buttons: Terrakotta füllt sich von links (scaleX)
- Custom Cursor: Terrakotta-Dot + Ring (nur Desktop)

**Buttons:**
- Outline: Terrakotta-Rand, Terrakotta-Text → füllt sich beim Hover
- Filled: Terrakotta-Hintergrund, weißer Text → Bordeaux beim Hover
- Light (auf Bordeaux): weißer Rand, weißer Text → füllt sich weiß

**Hover-States:**
- Methode-Karten: Terrakotta-Linie wächst von links
- FAQ: sanftes Öffnen/Schließen
- Magnetische Buttons (leichtes Folgen der Maus)

**Foto-Behandlung:**
- Hero: Bild füllt rechte Hälfte, Bordeaux-Verlauf nach links
- Problem: Bild 3:4, dekorativer Terrakotta-Rahmen versetzt
- Über mich: Ballett-Foto groß + kleines Foto darunter rechts

**Noise-Textur:**
- Bordeaux-Sektionen erhalten subtile SVG-Noise (opacity 0.03)

---

## TECHNISCHE ANFORDERUNGEN

- Eine einzige HTML-Datei (alles inline: CSS + JS)
- Responsive: Mobile-first, Breakpoints bei 860px und 640px
- Smooth Scroll
- Intersection Observer für alle Animationen
- FAQ Accordion (vanilla JS)
- Custom Cursor (nur bei pointer: fine)
- SEO: Title, Meta Description, OG-Tags, JSON-LD (Person + ProfessionalService)
- Accessibility: Skip-Link, Focus-Visible, ARIA-Labels, prefers-reduced-motion
- Performance: Google Fonts mit preconnect

**Meta-Daten:**
```
Title: Julia Lauer · Bewusstseinsarchitektur — für Frauen, die funktionieren
Description: Für Frauen, die funktionieren — und aufgehört haben zu spüren, was es kostet.
Die Bewusstseinsarchitektur-Methode arbeitet unterhalb des Denkens. 1:1 online.
```

**JSON-LD:**
```json
Person: Julia Lauer, Bewusstseinsarchitektin
Service: Bewusstseinsarchitektur, 1:1 online, DE
Offers: Klarheitsgespräch (0€), Focus Shift (450€), Deep Shift (3500€)
```

---

## QUALITÄTSANSPRUCH

Diese Website muss wirken wie:
- Editorial — nicht wie Coaching-Template
- Warm — nicht klinisch
- Präzise — nicht erklärig
- Würdevoll — nicht werbend

Sara landet hier und denkt: die meint mich.
Sie scrolt. Sie liest. Sie nickt.
Sie bucht.

Das ist das Ziel.

---

## AUSGABE

Komplette, sofort lauffähige index.html.
Alle Bilder werden per relativer Pfadangabe eingebunden
(sie liegen im selben Ordner wie die index.html).

Bildnamen exakt:
- 3H0A0008.jpeg
- IMG_2795.JPEG
- Ballett_Julia.JPEG
- IMG_7914.JPEG
