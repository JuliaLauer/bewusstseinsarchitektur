# CLAUDE CODE — FINALE INDEX.HTML v3
# bewusstseinsarchitektur.de · Julia Lauer
# Baue von Grund auf neu. Beste Version. Kein Kompromiss.

---

## MISSION

Erstelle die ultimative index.html für bewusstseinsarchitektur.de.
Ziel: Editorial. Dramatisch. Warm. Präzise.
Wie eine 10.000€-Agentur-Website — aber mit Seele.

---

## FARB-SYSTEM (absolut unveränderlich)

```css
--bordeaux:    #2E0F14;
--terrakotta:  #B5603A;
--licht:       #FAF8F5;
--weiss:       #FFFFFF;
--text-dunkel: #1A1A1A;
--text-mittel: #4A4A4A;
```

---

## KONTRAST-REGELN (nicht verhandelbar)

NIEMALS unter diesen Werten:
- Text auf Bordeaux: #FFFFFF — niemals rgba unter 0.9
- Text auf Licht: #1A1A1A (primär) / #4A4A4A (sekundär) — niemals rgba unter 0.8
- Labels/Caps auf Bordeaux: #FFFFFF oder var(--terrakotta) — niemals gedimmt
- Kleine Texte (unter 13px): font-weight 400 minimum
- Fließtext: font-weight 300 minimum
- Footer-Links: rgba(255,255,255,0.75) minimum
- Proof-Bar Labels: rgba(255,255,255,0.8) minimum
- Hero Subtext: rgba(255,255,255,0.92) minimum
- CTA-Garantien: rgba(255,255,255,0.75) minimum

VERBOTEN:
- rgba(255,255,255,0.3) oder niedriger für lesbaren Text
- rgba(255,255,255,0.4) oder niedriger für lesbaren Text
- rgba(26,26,26,0.4) oder niedriger für lesbaren Text
- font-weight 200 irgendwo

---

## TYPOGRAFIE

```
Google Fonts:
Cormorant Garamond: ital, wght 300+400
Jost: wght 300+400

Display/Headlines: Cormorant Garamond · Italic · 300
Body: Jost · 300
Labels/Caps/kleine Texte: Jost · 400 · letter-spacing 0.2em+
Buttons: Jost · 400
```

---

## BILDER (im gleichen Ordner)

- Hero rechts: `3H0A0008.jpeg`
- Problem: `IMG_2795.JPEG`
- Über mich groß: `Ballett_Julia.JPEG`
- Über mich klein: `IMG_7914.JPEG`

---

## WOW-EFFEKT: LAYOUT-PRINZIPIEN

Jede Sektion braucht eine eigene visuelle Identität.
Kein Template-Denken. Keine gleichförmigen Abstände.

**Hero:** Vollbild-Split. Bild dominiert rechts. Text linke Hälfte.
**Problem:** Asym. Grid. Bild groß links, Text fließt rechts daneben.
**Testimonial 1:** Maximale Stille. Riesiges Anführungszeichen. Ein Satz. Viel Luft.
**Reframing:** Bordeaux. Zentriert. Die 5 Reframe-Zeilen GROSS, dramatisch, einzeln.
**Methode:** Horizontales Masonry — nicht 3 gleiche Karten. Unterschiedliche Höhen.
**Testimonials 2+3:** Überlappendes Layout. Linke Karte höher als rechte.
**Was sich verändert:** Großes Zitat links, 2x2 Grid rechts. Asymmetrisch.
**Angebote:** Bordeaux. Mittlere Karte ragt nach oben heraus (transform: translateY(-2rem)).
**Über mich:** Ballett-Foto nimmt 55% ein. Text rechts. Kleines Foto darunter versetzt.
**FAQ:** 2 Spalten. Links 3 Fragen, rechts 3 Fragen.
**Final CTA:** Bordeaux. Großes Cormorant-Zitat zentriert. Viel Luft. Ein Button.

---

## SEITENSTRUKTUR & ALLE TEXTE

---

### NAV (fixed)

Logo: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic)
Links: Methode · Angebote · Über mich · FAQ
CTA: `Klarheitsgespräch →` (Terrakotta-Button)

Verhalten:
- Transparent auf Hero
- Bordeaux bei Scroll über Bordeaux-Sektionen
- rgba(250,248,245,0.96) backdrop-blur bei Scroll über hellen Sektionen
- Hamburger Mobile

---

### 01 · HERO (Bordeaux · 100svh)

Layout: links Text (55%), rechts Foto (45%) mit Bordeaux-Gradient nach links.
Noise-Textur auf Bordeaux. Foto: scale 1.06 → 1 beim Laden (zoom-out).

Label (animiert rein, Terrakotta):
```
BEWUSSTSEINSARCHITEKTUR
```

H1 (Cormorant Italic, sehr groß, weiß, Zeile für Zeile animiert):
```
Für Frauen,
die funktionieren —
und aufgehört haben zu spüren,
was es kostet.
```

Subtext (Jost 300, rgba(255,255,255,0.92)):
```
Du trägst Verantwortung.
Du entscheidest.
Menschen verlassen sich auf dich.

Und lange funktioniert das auch.

Bis dein Körper irgendwann beginnt zu zeigen,
dass etwas unter der Oberfläche nicht mehr stimmt.

Nicht laut. Eher leise. Aber deutlich.
```

Button (btn--filled, Terrakotta):
```
Klarheitsgespräch anfragen →
```

Darunter (Jost 400, rgba(255,255,255,0.75)):
```
0 € · 30 Minuten · Kein Verkaufsdruck
```

Scroll-Indicator unten links (animierte Linie + "Scroll").

---

### 02 · PROOF BAR (Bordeaux · schmal · kein section-padding)

3 Kennzahlen mit animierten Countern:

```
100+               |     1:1 online      |     seit 2023
Klientinnen        |     weltweit        |     Deep Shift
```

Zahlen: Cormorant Italic, #FFFFFF, groß.
Labels: Jost 400, rgba(255,255,255,0.8).
Trennlinie: 1px rgba(255,255,255,0.15).

---

### 03 · PROBLEM (Licht)

WOW-LAYOUT:
- Foto links nimmt volle Höhe ein (sticky beim Scrollen auf Desktop)
- Text scrollt rechts daneben
- Terrakotta-Rahmen: versetzt top-right 1.5rem außerhalb des Fotos

Label (Jost 400, Terrakotta):
```
FÜR WEN
```

H2 (Cormorant Italic, Bordeaux, groß):
```
Die meisten Frauen kommen nicht zu mir,
weil sie nicht mehr können.
```

Terrakotta-Divider (animiert).

Text (Jost 300, #1A1A1A, Zeilen einzeln — kurze Abstände zwischen Absätzen):
```
Sie kommen, weil sie merken:
So will ich nicht weitermachen.

Du hast alles gegeben.
Den Erwartungen entsprochen — vor allem deinen eigenen.

Eigentlich sollte sich das jetzt leicht anfühlen.

Aber da ist eher Leere.

Du hast dich reguliert.
Kontrolliert.
Gedimmt damit andere strahlen können.
Harmonisiert. Gehalten. Ausgehalten.
Und geleistet.

Und jetzt stehst du hier.
Und bekommst gesagt:

Entspann dich doch mal. Du musst mal was für dich tun.

Dein Modus ist der Normalzustand geworden.
Es gibt keinen Ausknopf mehr.

Morgens. Noch im Halbschlaf.
Und schon scannt dein System:
War gestern was? Was steht heute an?

Noch nicht wach, schon auf der Hut.
```

Dann unter dem Grid — volle Breite, zentriert, Licht-Hintergrund:

H3 (Cormorant Italic, Bordeaux, sehr groß):
```
Dann meldet sich der Körper.
```

Kleiner Text (Jost 300, #4A4A4A):
```
Nicht dramatisch.
Einfach hartnäckig.
```

Liste (Terrakotta-Dash, Jost 300, #1A1A1A):
```
— Schlaf, der nicht mehr richtig erholt.
— Verspannungen, die bleiben.
— Eine Müdigkeit, die kein freies Wochenende löst.
— Reizbarkeit ohne klaren Grund.
— Manchmal Tinnitus. Oder der Magen. Auch der Kiefer.
```

Fett (Jost 400, Bordeaux):
```
Der Körper erfindet das nicht.
Er zeigt etwas.
```

Button (Terrakotta, zentriert):
```
Klarheitsgespräch anfragen →
```

---

### 04 · TESTIMONIAL 1 (Licht · WOW: maximale Stille)

WOW-LAYOUT:
- Großes Cormorant-Anführungszeichen in Terrakotta (opacity 0.12, sehr groß, oben links)
- Das Zitat in der Mitte, groß, viel Luft
- Name unten, klein, Terrakotta

Zitat (Cormorant Italic, Bordeaux, clamp(1.5rem, 3vw, 2.4rem)):
```
„Ich habe funktioniert — aber innerlich war da ständig dieser Druck.
Nach unserer Arbeit war er weg. Einfach weg.
Und Dinge, die sich unmöglich angefühlt haben,
haben sich von allein gelöst."
```

Name (Jost 400, Terrakotta):
```
Sarah L. · Unternehmerin
```

---

### 05 · REFRAMING (Bordeaux)

WOW-LAYOUT:
- Block 1: breiter Fließtext zentriert, max-width 680px
- Terrakotta-Divider zentriert
- Block 2: "Ich höre das anders" als riesige Cormorant-Headline
- Die 5 Reframe-Zeilen: SEHR GROSS, Cormorant Italic, #FFFFFF, zentriert, mit Terrakotta-Linie links
- Abschlusstext: Jost 300, rgba(255,255,255,0.92)

H2 (Cormorant Italic, #FFFFFF, clamp(2rem, 4vw, 3.5rem)):
```
Vielleicht hast du schon vieles ausprobiert.
```

Text (Jost 300, rgba(255,255,255,0.92)):
```
Therapie. Coaching. Meditation. Journaling.

Und manches hat auch geholfen.

Aber irgendetwas bleibt.

Nicht weil du etwas falsch gemacht hast.

Sondern weil die Ursache tiefer sitzt als Gedanken.
Unterhalb von Willenskraft.
Unterhalb von Verstand.

Im Unterbewusstsein.
Dort wo sie entstanden ist.
Und dort wo sie sich wirklich auflösen lässt.
```

Terrakotta-Divider zentriert.

H2 (Cormorant Italic, #FFFFFF, sehr groß):
```
Ich höre das anders.
```

Intro (Jost 300, rgba(255,255,255,0.92)):
```
Vielleicht wurde dir irgendwann gesagt:
Du bist zu kontrollierend! Zu perfektionistisch! Zu viel!
```

5 Reframe-Zeilen (Cormorant Italic, #FFFFFF, clamp(1.8rem, 3.5vw, 3rem), mit 4px Terrakotta-Linie links, padding-left 1.5rem, zentriert im Container):
```
Kontrolle ist Organisationskraft.
Perfektionismus ist Qualitätswille.
Verantwortung ist Stärke.
Ausgleichen ist Fürsorge.
Harmonie halten — eine Kunst.
```

Abschlusstext (Jost 300, rgba(255,255,255,0.92)):
```
Das sind keine Fehler. Das sind Kräfte.
Kräfte, die dich weit gebracht haben.

Das Problem ist nicht, wer du bist.
Sondern: Irgendwann dienen dir diese Kräfte nicht mehr.
Sie halten dein System rund um die Uhr unter Strom.

Und das kostet. Jeden Tag.
```

---

### 06 · METHODE (Licht)

WOW-LAYOUT: Kein normales 3-Karten-Grid.
- Volle Breite: Einleitungstext linksbündig, groß
- Darunter: Horizontales Layout mit 3 Blöcken — UNTERSCHIEDLICHE HÖHEN
  - Block 1: kurz, oben
  - Block 2: mittel, versetzt nach unten (margin-top: 3rem)
  - Block 3: lang, oben
  - Terrakotta-Linie wächst von links beim Hover

Label (Jost 400, Terrakotta):
```
METHODE
```

H2 (Cormorant Italic, Bordeaux, groß):
```
Wie ich arbeite.
```

Terrakotta-Divider.

Einleitungstext (Jost 300, #1A1A1A, max-width 700px, groß 1.1rem):
```
Ich arbeite nicht an deinen Symptomen.
Nicht an deinem Verhalten.

Es bringt nichts, die Mitfahrer auszutauschen.
Wenn derselbe Fahrer am Steuer sitzt,
führt die Reise immer wieder an denselben Ort.

Darum arbeite ich direkt mit dem Fahrer.
```

Methodenname (Jost 400, Terrakotta, letter-spacing 0.15em):
```
Bewusstseinsarchitektur.
```

3 Blöcke (Licht-Hintergrund, Border 1px rgba(46,15,20,0.1), Terrakotta-Hover-Linie):

**Block 1 — An der Wurzel**
Nummer: `01` (Cormorant Italic, Terrakotta, opacity 0.3, groß)
```
Er setzt dort an,
wo Muster tatsächlich entstehen.

Nicht im Denken.
Nicht im Verhalten.

Sondern darunter.
Im System. Deinem Unterbewusstsein.
```

**Block 2 — Bernstein**
Nummer: `02`
```
Alles, was du erlebt hast, hinterlässt Spuren.
Manche sehr früh. Manche sehr tief.

Manche bleiben wie eingefroren —
wie kleine Bernsteinstücke.

Sie entwickeln sich nicht weiter.
Aber sie wirken weiter.
Oft ohne, dass wir es merken.
```

**Block 3 — Ohne Umweg**
Nummer: `03`
```
Darum gibt es hier
keinen Analyse-Marathon.

Wir gehen direkt dorthin,
wo diese Muster entstanden sind.
Und verändern sie dort.

Ohne Retraumatisierung.
Ohne Wühlen in alten Geschichten.
Ohne Drama.

Dafür mit Respekt.
Mit Wertschätzung.

Denn auch das,
was wir auflösen,
hat einmal eine wichtige Aufgabe erfüllt.
```

---

### 07 · TESTIMONIALS 2+3 (Licht · WOW: überlappend)

WOW-LAYOUT:
- Karte links beginnt oben
- Karte rechts beginnt 4rem tiefer (margin-top)
- Beide mit großem Cormorant-Anführungszeichen (Terrakotta, opacity 0.1)
- Border 1px rgba(46,15,20,0.1)

Karte links:
```
„Ich habe nicht erwartet, dass sich mein Körper verändert.
Aber auch nicht, dass ich aufhöre,
mein Wohlbefinden von der Meinung anderer abhängig zu machen.
Beides ist passiert."

Elena C. · Projektleiterin
```

Karte rechts:
```
„Die Schuldgefühle, die ich jahrelang mit mir getragen habe —
sie sind einfach nicht mehr da.
Ich weiß selbst nicht genau wie. Aber es ist so."

Nadine H. · Ärztin
```

---

### 08 · WAS SICH VERÄNDERT (Licht)

WOW-LAYOUT:
- Linke Seite (40%): Großes Einleitungszitat + 4 konkrete innere Momente
- Rechte Seite (60%): 4 Bereiche gestapelt mit Terrakotta-Checkmarks

Intro (Cormorant Italic, Bordeaux, groß, linksbündig):
```
Vielleicht spürst du zuerst Müdigkeit.
Ein erstes Loslassen aus der dauernden Spannung heraus.

Dann wird es klarer.
Nicht dramatisch. Eher in kleinen Momenten.
```

4 Momente links (Cormorant Italic, Bordeaux, 4px Terrakotta-Linie links, padding-left 1.2rem):
```
Es ist völlig in Ordnung,
mich mit einem Kaffee hinzusetzen —
auch wenn der Haushalt nicht perfekt ist.

Und: Nein. Es ist nicht ok,
dass der Kunde mich versetzt hat ohne abzusagen.

Ich habe seit Wochen Nackenverspannungen.
Also buche ich jetzt die Massage.
Einfach weil es mir gut tut.

Ich meditiere.
Ganz ohne Zwang.
Sondern weil es mir ein Bedürfnis ist.
```

4 Bereiche rechts (Terrakotta-Checkmark vor dem Titel):

✓ Körperlich (Jost 400, Bordeaux als Titel):
```
Das Nervensystem beruhigt sich.
Die Symptome flachen ab.
Der Schlaf wird tiefer.
```

✓ Zwischenmenschlich:
```
Du nimmst deinen Partner wieder wahr.
Wählst bewusst, wann du Freunde treffen willst.
Kannst Grenzen setzen, ohne zu verletzen.
```

✓ Beruflich:
```
Du beendest ein großes Projekt.
Stehst vor dem Ergebnis.
Und sagst dir: Ja. Das habe ich gut gemacht.
```

✓ Innerlich:
```
Du reagierst nicht mehr automatisch.
Du atmest aus. Und wählst.

Nicht weil du es dir antrainiert hast.
Sondern weil innen etwas anders geworden ist.
```

Darunter — volle Breite, zentriert, viel Luft:

Großes Zitat (Cormorant Italic, Bordeaux, sehr groß):
```
Du weißt was du weißt.
Und das reicht.
```

Kleiner Text (Jost 300, #4A4A4A, zentriert):
```
Das ist die wahre Qualität
in dem Spalt zwischen Reiz und Reaktion.

Innere Stimmigkeit. Das Äußere folgt nach.
```

---

### 09 · ANGEBOTE (Bordeaux · Noise-Textur)

WOW-LAYOUT:
- 3 Karten nebeneinander
- Mittlere (Deep Shift): transform translateY(-2rem), Terrakotta-Rand oben 3px, heller Hintergrund rgba(255,255,255,0.06)
- Äußere: einfache Karten mit Rand rgba(255,255,255,0.15)

Label (Jost 400, Terrakotta):
```
ANGEBOTE
```

H2 (Cormorant Italic, #FFFFFF):
```
So arbeiten wir zusammen.
```

**Karte 1 — Klarheitsgespräch:**
Preis (Cormorant Italic, #FFFFFF, groß): `0 €`
Subtitle (Jost 400, rgba(255,255,255,0.8)): `30 Minuten`
```
Du willst wissen, ob das hier das Richtige für dich ist.
Kein Pitch. Keine Agenda.
Wir schauen gemeinsam hin —
und du gehst mit einer klaren Einschätzung raus.
```
Button (btn--light): `Anfragen →`

**Karte 2 — Deep Shift (HERO):**
Tag (Jost 400, Terrakotta): `KERNANGEBOT`
Preis (Cormorant Italic, Terrakotta, sehr groß): `3.500 €`
Subtitle (Jost 400, rgba(255,255,255,0.9)): `12 Wochen · 6–8 Sessions · 1:1 online`
```
Die tiefgreifendste Form der Zusammenarbeit.

Wir arbeiten nicht an Symptomen.
Wir ordnen dein System neu.

Meine Arbeit ist gut,
wenn du mich danach nicht mehr brauchst.

Nicht weil sie oberflächlich ist.
Sondern weil du lernst,
dein eigenes System zu führen.
Ohne dauerhafte Begleitung.
Ohne Abhängigkeit.
```
Button (btn--filled, Weiß-Hintergrund, Bordeaux-Text): `Klarheitsgespräch buchen →`

**Karte 3 — Focus Shift:**
Preis (Cormorant Italic, #FFFFFF, groß): `450 €`
Subtitle (Jost 400, rgba(255,255,255,0.8)): `2 Sessions · 1 Thema`
```
Ein Thema. Zwei Sitzungen.
Ein gezielter Wendepunkt.

Für alle, die wissen, was sie bewegt —
und bereit sind, genau dort anzusetzen.
```
Button (btn--light): `Anfragen →`

---

### 10 · ÜBER MICH (Licht)

WOW-LAYOUT:
- Linke Spalte: Ballett_Julia.JPEG (55% Breite, volle Höhe, object-fit cover)
  - Darunter versetzt (+2rem rechts): IMG_7914.JPEG (kleiner, quadratisch)
- Rechte Spalte: Text mit Label + H2 + Fließtext + Zitat

Label (Jost 400, Terrakotta):
```
ÜBER MICH
```

H2 (Cormorant Italic, Bordeaux, groß):
```
Ich rede nicht über diesen Zustand.
Ich habe ihn im Körper erlebt.
```

Text (Jost 300, #1A1A1A):
```
Klassisches Ballett ab fünf Jahren.
Mit 13 München, Talentschmiede des Bayerischen Staatstheaters.
Leisten, funktionieren, psychosomatische Beschwerden —
über jede Grenze hinaus.

Mit 15 die Prüfung vor John Neumeier.
Der erkannte, was ich mir selbst vorher nicht eingestehen konnte.

Und dann stellte er mir eine Frage:

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

Abschluss-Zitat (Cormorant Italic, Terrakotta, mit Terrakotta-Linie links):
```
Yager ist der Ursprung.
Bewusstseinsarchitektur ist mein Weg.
```

---

### 11 · FAQ (Licht · 2-Spalten-Accordion)

Label (Jost 400, Terrakotta):
```
FRAGEN & ANTWORTEN
```

Linke Spalte — 3 Fragen:

**Für wen ist das gedacht?**
```
Für Frauen, die das Gefühl haben, mit dem Kopf allein nicht weiterzukommen.
Die innerlich an eine Grenze gestoßen sind und spüren,
dass da etwas ist, was sich verändern will.
Keine Vorkenntnisse nötig. Nur die Bereitschaft, wirklich hinzuschauen.
```

**Wie läuft eine Sitzung ab?**
```
Jede Sitzung ist anders, weil jeder Mensch anders ist.
Wir starten dort, wo du gerade bist —
was dich beschäftigt, was sich zeigt, was du mitbringst.
Von da aus arbeiten wir gemeinsam.
```

**Wie lange dauert der Prozess?**
```
Das lässt sich nicht pauschal sagen.
Manche spüren nach wenigen Sitzungen eine spürbare Veränderung,
andere brauchen mehr Zeit.
Wir schauen gemeinsam, was sinnvoll ist — ohne künstlichen Druck.
```

Rechte Spalte — 3 Fragen:

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

**Ist das Hypnose?**
```
Nein. Du bleibst während der gesamten Arbeit vollständig bewusst und in Kontrolle.
Die Methode arbeitet über spezifische Kommunikationswege mit dem Unterbewusstsein —
ohne Trancezustand, ohne Suggestion.
```

FAQ-Stil: Frage in Jost 400, Bordeaux. Plus/Minus Icon Terrakotta. Antwort Jost 300, #4A4A4A. Sanfte Accordion-Animation.

---

### 12 · FINAL CTA (Bordeaux · Noise · zentriert · viel Luft)

WOW-LAYOUT: Maximale Stille. Nur Text und ein Button.
Sehr viel padding-block (min 8rem).

Label (Jost 400, Terrakotta):
```
BEREIT?
```

H2 (Cormorant Italic, #FFFFFF, sehr groß, clamp(2rem, 5vw, 4rem)):
```
Wenn du beim Lesen gemerkt hast,
dass irgendwo etwas in dir
ruhig genickt hat —
```

Text (Jost 300, rgba(255,255,255,0.9)):
```
dann können wir sprechen.

In einem Gespräch schauen wir gemeinsam,
ob diese Arbeit für dich passt.
```

Button (btn--light, groß, padding 1rem 3rem):
```
Klarheitsgespräch anfragen →
```

Garantien (Jost 400, rgba(255,255,255,0.75)):
```
Kostenlos  ·  30 Minuten  ·  Kein Verkaufsdruck
```

---

### 13 · FOOTER (Bordeaux)

Links: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic, rgba(255,255,255,0.75))
Mitte: `© 2026` (Jost 400, rgba(255,255,255,0.5))
Rechts: `Impressum · Datenschutz` (Jost 400, rgba(255,255,255,0.75), hover: #FFFFFF)

---

## ANIMATIONEN & DETAILS

**Custom Cursor (nur pointer:fine):**
Terrakotta-Dot 6px + Ring 32px border Terrakotta.
Hover: Dot scale 1.6, Ring 48px.

**Scroll Reveal:**
opacity 0 → 1, translateY 30px → 0, 0.8s ease.
Intersection Observer threshold 0.1.

**Hero:**
H1 Zeilen: clip-reveal von unten, sequenziell 0.1s Delay.
Subtext + CTA: fadeUp, animiert nach H1.
Foto: scale(1.06) → scale(1), 8s ease-out.

**Terrakotta-Divider:**
width 0 → 48px, 0.8s cubic-bezier(0.16, 1, 0.3, 1).

**Buttons:**
scaleX(0) → scaleX(1) von links, 0.35s.
Magnetisch: sanftes Maus-Folgen (±8px max).

**Proof-Bar Counter:**
0 → 100+, 1.8s ease-out cubic.

**Methode-Karten:**
Terrakotta-Linie wächst von links (right: 100% → 0%), height 2px, bottom.

**FAQ Accordion:**
max-height 0 → auto, 0.45s cubic-bezier(0.16, 1, 0.3, 1).

**prefers-reduced-motion:**
Alle Animationen deaktiviert. Elemente sofort sichtbar.

---

## TECHNISCHE ANFORDERUNGEN

- Einzelne HTML-Datei (CSS + JS inline)
- Responsive: Mobile-first
  - 860px: Nav-Links ausblenden, Hamburger-Menü
  - 640px: Alle Grids auf 1 Spalte
  - Hero Mobile: Bild unter Text, Höhe auto
- Smooth Scroll
- Accessibility: Skip-Link, ARIA-Labels, focus-visible (Terrakotta-Outline)
- Google Fonts: preconnect + preload

**Meta/SEO:**
```
<title>Julia Lauer · Bewusstseinsarchitektur — für hochleistende Frauen</title>
<meta name="description" content="Für Frauen, die funktionieren — und aufgehört haben zu spüren, was es kostet. Die Bewusstseinsarchitektur-Methode arbeitet unterhalb des Denkens. 1:1 online.">
<link rel="canonical" href="https://bewusstseinsarchitektur.de/">
<meta name="theme-color" content="#2E0F14">
```

**JSON-LD:**
Person: Julia Lauer, Bewusstseinsarchitektin, URL bewusstseinsarchitektur.de
ProfessionalService + 3 Offers: Klarheitsgespräch (0€), Focus Shift (450€), Deep Shift (3500€)
Calendly: https://calendly.com/zentrum-bewusstseinsarchitektur/30min

---

## QUALITÄTSANSPRUCH

Diese Seite muss wirken wie eine 10.000€-Agentur-Arbeit.

Sara landet hier. Liest den ersten Satz.
Denkt: Die meint mich.

Scrollt durch den Körper-Abschnitt.
Denkt: Das bin ich.

Liest "Ich höre das anders."
Denkt: Endlich jemand, der das versteht.

Sieht den Preis.
Denkt: Das ist es wert.

Bucht.

Das ist das Ziel. Keine Kompromisse.
