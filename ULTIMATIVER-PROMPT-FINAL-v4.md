# CLAUDE CODE — ULTIMATIVE FINALE INDEX.HTML
# bewusstseinsarchitektur.de · Julia Lauer
# Baue von Grund auf neu. Kein Kompromiss. Keine halben Sachen.

---

## MISSION

Diese Seite hat eine einzige Aufgabe:
Sara landet hier. Liest drei Sätze. Denkt: Die meint mich.
Scrollt. Nickt. Bucht.

Nicht erklären. Nicht überzeugen. Treffen.

---

## FARB-SYSTEM

```css
--bordeaux:    #3D1219;
--terrakotta:  #B5603A;
--licht:       #FAF8F5;
--weiss:       #FFFFFF;
--text-dunkel: #1A1A1A;
--text-mittel: #4A4A4A;
```

KONTRAST-GESETZ — keine Ausnahmen:
- Text auf Bordeaux: #FFFFFF — niemals unter opacity 0.88
- Kleintexte auf Bordeaux: font-weight 400, niemals unter opacity 0.75
- Text auf Licht: #1A1A1A (primär), #4A4A4A (sekundär)
- font-weight 200 existiert nicht auf dieser Seite
- Buttons: immer sichtbar, immer klickbar wirkend

---

## TYPOGRAFIE

```
Cormorant Garamond: ital 300+400 → Headlines, Zitate, Preise
Jost: 300+400 → Body, Labels, Buttons, Nav
```

Faustregel: Je kleiner der Text, desto höher das weight.
Unter 13px: immer Jost 400.

---

## BILDER

Alle im gleichen Ordner:
- Hero: `3H0A0008.jpeg` (Porträt, dunkel, direkt)
- Problem: `IMG_2795.JPEG` (Kopf in Hand, erschöpft)
- Über mich: `Ballett_Julia.JPEG` (S/W, dramatisch)
- Über mich klein: `IMG_7914.JPEG`

---

## CONVERSION-LOGIK (Seitenaufbau)

```
AUFMERKSAMKEIT  →  Sara erkennt sich
PROBLEM         →  Sara fühlt sich verstanden
VERTRAUEN 1     →  jemand wie sie hat es geschafft
WARUM ANDERS    →  der USP wird klar
LÖSUNG          →  kurz, präzise, überzeugend
JULIA           →  Credibility durch Erfahrung
VERTRAUEN 2     →  mehr Erfahrungsberichte
TRANSFORMATION  →  wie ihr Leben danach aussieht
ANGEBOT         →  jetzt bereit zu kaufen
EINWÄNDE        →  letzten Zweifel beseitigen
HANDLUNG        →  buchen
```

---

## SEITENSTRUKTUR

---

### NAV (fixed)

- Transparent auf Bordeaux-Sektionen
- rgba(250,248,245,0.96) + backdrop-blur auf hellen Sektionen
- Logo: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic, Bordeaux/Weiß je nach Hintergrund)
- Links: Methode · Angebote · Über mich · FAQ (Jost 400)
- CTA-Button: `Klarheitsgespräch →` (Terrakotta-Rand, Terrakotta-Text → füllt sich)
- Mobile: Hamburger + Drawer

---

### 01 · HERO (Bordeaux · 100svh · 2 Spalten)

Links: Text (55%). Rechts: Foto (45%), object-fit cover, object-position top, Bordeaux-Gradient nach links.
Noise-Textur. Foto: scale(1.06)→scale(1) beim Laden, 8s ease.

```
[Jost 400, Terrakotta, 0.68rem, letter-spacing 0.22em, uppercase]
BEWUSSTSEINSARCHITEKTUR

[Cormorant Italic, #FFFFFF, clamp(1.3rem, 2.2vw, 1.8rem), leicht verzögert]
Alles läuft. Aber es kostet.

[Cormorant Italic, #FFFFFF, clamp(2.6rem, 5vw, 5rem), Zeile für Zeile animiert]
Für Frauen, die funktionieren.
Und die spüren:
Ich kann so weitermachen.
Aber ich will es nicht.

[Jost 300, rgba(255,255,255,0.92), 1rem, line-height 1.9]
Du trägst Verantwortung.
Du entscheidest.
Menschen verlassen sich auf dich.

Und lange funktioniert das auch.

Bis dein Körper irgendwann beginnt zu zeigen,
dass etwas unter der Oberfläche nicht mehr stimmt.

Nicht laut. Eher leise. Aber deutlich.

[Button: btn--filled, Terrakotta]
Klarheitsgespräch anfragen →

[Jost 400, rgba(255,255,255,0.75), klein]
0 € · 30 Minuten
```

---

### 02 · PROOF BAR (Bordeaux · kein section-padding · border-top 1px rgba(255,255,255,0.08))

3 Zahlen. Zahlen: Cormorant Italic, #FFFFFF, 2rem.
Labels: Jost 400, rgba(255,255,255,0.8), 0.68rem.
Trennlinie: 1px rgba(255,255,255,0.15).

```
20 Jahre          |     1:1 online      |     100+
Körperarbeit      |     weltweit        |     Klientinnen
```

---

### 03 · PROBLEM (Licht)

WOW-LAYOUT:
Foto links (sticky auf Desktop, 3:4 Format).
Terrakotta-Rahmen: top +1.5rem right -1.5rem, z-index -1.
Text scrollt rechts daneben.

```
[Label: FÜR WEN]

[H2, Cormorant Italic, Bordeaux, clamp(2rem, 3.5vw, 3.2rem)]
Die meisten Frauen kommen nicht zu mir,
weil sie nicht mehr können.

[Terrakotta-Divider 48px]

[Jost 300, #1A1A1A, 1rem, line-height 1.9]
Sie kommen, weil sie merken:
[Jost 400, Bordeaux] So will ich nicht weitermachen.

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

[Cormorant Italic, #4A4A4A]
Entspann dich doch mal. Du musst mal was für dich tun.

Dein Modus ist der Normalzustand geworden.
Es gibt keinen Ausknopf mehr.

Morgens. Noch im Halbschlaf.
Und schon scannt dein System:
War gestern was? Was steht heute an?

Noch nicht wach, schon auf der Hut.
```

Dann — volle Breite, unter dem Grid, zentriert:

```
[H3, Cormorant Italic, Bordeaux, clamp(2rem, 4vw, 3.5rem), zentriert]
Dann meldet sich der Körper.

[Jost 300, #4A4A4A, zentriert]
Nicht dramatisch. Einfach hartnäckig.

[Liste, Jost 300, #1A1A1A, Terrakotta-Dash, max-width 600px, zentriert]
— Schlaf, der nicht mehr richtig erholt.
— Verspannungen, die bleiben.
— Eine Müdigkeit, die kein freies Wochenende löst.
— Reizbarkeit ohne klaren Grund.
— Manchmal Tinnitus. Oder der Magen. Auch der Kiefer.

[Jost 400, Bordeaux, zentriert]
Der Körper erfindet das nicht.
Er zeigt etwas.

[Button zentriert, Terrakotta, btn--filled]
Klarheitsgespräch anfragen →
```

---

### 04 · TESTIMONIAL 1 (Bordeaux · maximale Stille)

WOW-LAYOUT:
Riesiges " in Cormorant Italic, Terrakotta, opacity 0.12, absolut positioniert oben links.
Zitat zentriert, viel Luft.
Name klein, Terrakotta, zentriert.

```
[Cormorant Italic, #FFFFFF, clamp(1.6rem, 3vw, 2.4rem), zentriert, max-width 800px]
„Ich habe funktioniert — aber innerlich war da ständig dieser Druck.
Nach unserer Arbeit war er weg. Einfach weg.
Und Dinge, die sich unmöglich angefühlt haben,
haben sich von allein gelöst."

[Jost 400, Terrakotta, 0.75rem, letter-spacing 0.12em]
Sarah L. · Unternehmerin
```

---

### 05 · USP-BLOCK (Licht · WOW: Editorial-Split)

WOW-LAYOUT:
Links: Eine große, ruhige Aussage. (40% Breite)
Rechts: 5 konkrete Punkte — was dich von allem anderen unterscheidet. (60% Breite)
Vertikale Terrakotta-Linie 1px zwischen beiden Hälften.
Nummern: Cormorant Italic, Terrakotta, opacity 0.4, groß.

```
[Links — Cormorant Italic, Bordeaux, clamp(2rem, 4vw, 3.5rem), max-width 380px]
Ich denke anders.
Ich arbeite anders.

[Jost 300, #4A4A4A, 1rem, margin-top 1.5rem, line-height 1.8]
Nicht weil die anderen falsch liegen.
Sondern weil ich auf einer anderen Ebene ansetze.

[Rechts — 5 Punkte, je mit Terrakotta-Nummer + Border-bottom rgba(46,15,20,0.08)]

[01]
[Jost 400, Bordeaux, 1rem]
Keine Hypnose.
[Jost 300, #4A4A4A]
Du bleibst vollständig bewusst und in Kontrolle.
Die gesamte Sitzung.

[02]
[Jost 400, Bordeaux]
Keine Ursachensuche. Keine Retraumatisierung.
[Jost 300, #4A4A4A]
Wir müssen nicht verstehen, woher etwas kommt.
Wir müssen es nur dort verändern, wo es sitzt.

[03]
[Jost 400, Bordeaux]
Direkt an der Wurzel.
[Jost 300, #4A4A4A]
Nicht am Symptom. Nicht am Verhalten.
Sondern da, wo Muster tatsächlich entstehen.

[04]
[Jost 400, Bordeaux]
Die Lösung liegt in dir.
[Jost 300, #4A4A4A]
Ich arbeite mit der Instanz in dir,
die über alles bescheid weiß —
und immer für dich arbeitet.

[05]
[Jost 400, Bordeaux]
Alles kann bearbeitet werden.
[Jost 300, #4A4A4A]
Körperlich. Mental. Emotional.
Was auch immer dein System zeigt —
es zeigt es aus einem Grund.
```

---

### 06 · REFRAMING (Bordeaux)

```
[H2, Cormorant Italic, #FFFFFF, clamp(2rem, 4vw, 3.5rem)]
Vielleicht hast du schon vieles ausprobiert.

[Jost 300, rgba(255,255,255,0.92)]
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

[Terrakotta-Divider zentriert]

[H2, Cormorant Italic, #FFFFFF, sehr groß]
Ich höre das anders.

[Jost 300, rgba(255,255,255,0.92)]
Vielleicht wurde dir irgendwann gesagt:
Du bist zu kontrollierend! Zu perfektionistisch! Zu viel!

[5 Zeilen — Cormorant Italic, #FFFFFF, clamp(1.8rem, 3.5vw, 3rem),
 mit 4px Terrakotta-Linie links, padding-left 2rem, display block, zentriert im Container]
Kontrolle ist Organisationskraft.
Perfektionismus ist Qualitätswille.
Verantwortung ist Stärke.
Ausgleichen ist Fürsorge.
Harmonie halten — eine Kunst.

[Jost 300, rgba(255,255,255,0.92)]
Das sind keine Fehler. Das sind Kräfte.
Kräfte, die dich weit gebracht haben.

Das Problem ist nicht, wer du bist.
Sondern: Irgendwann dienen dir diese Kräfte nicht mehr.
Sie halten dein System rund um die Uhr unter Strom.

Und das kostet. Jeden Tag.
```

---

### 07 · METHODE (Licht · präzise, kein Überblick)

WOW-LAYOUT:
Nicht 3 gleichgroße Karten.
Großer Einleitungstext. Darunter: asymmetrisches Grid.
Block 1 links oben, Block 2 rechts versetzt (margin-top 4rem), Block 3 links unten.

```
[Label: METHODE]

[H2, Cormorant Italic, Bordeaux, groß]
Wie ich arbeite.

[Terrakotta-Divider]

[Jost 300, #1A1A1A, 1.05rem, max-width 680px]
Ich arbeite nicht an deinen Symptomen.
Nicht an deinem Verhalten.

Es bringt nichts, die Mitfahrer auszutauschen.
Wenn derselbe Fahrer am Steuer sitzt,
führt die Reise immer wieder an denselben Ort.

Darum arbeite ich direkt mit dem Fahrer.

[Jost 400, Terrakotta, letter-spacing 0.1em]
Diesen Ansatz nenne ich Bewusstseinsarchitektur.
```

3 Blöcke asymmetrisch:

```
[Block 1 — Karte mit Border, Terrakotta hover-Linie unten]
[Nummer: 01 — Cormorant Italic, Terrakotta, opacity 0.3, 3.5rem]

Er setzt dort an,
wo Muster tatsächlich entstehen.

Nicht im Denken.
Nicht im Verhalten.

Sondern darunter.
Im System. Deinem Unterbewusstsein.

[Block 2 — versetzt margin-top 4rem]
[Nummer: 02]

Alles, was du erlebt hast, hinterlässt Spuren.
Manche sehr früh. Manche sehr tief.

Manche bleiben wie eingefroren —
wie kleine Bernsteinstücke.

Sie entwickeln sich nicht weiter.
Aber sie wirken weiter.
Oft ohne, dass wir es merken.

[Block 3]
[Nummer: 03]

Darum gibt es hier
keinen Analyse-Marathon.

Wir gehen direkt dorthin,
wo diese Muster entstanden sind.
Und verändern sie dort.

Ohne Retraumatisierung.
Ohne Wühlen in alten Geschichten.
Ohne Drama.

Dafür mit Respekt. Mit Wertschätzung.
Denn auch das, was wir auflösen,
hat einmal eine wichtige Aufgabe erfüllt.
```

---

### 08 · JULIA (Licht · WOW · Credibility vor Angeboten)

WOW-LAYOUT:
Ballett-Foto 55% Breite, volle Höhe links.
Darunter IMG_7914.JPEG versetzt (+3rem rechts, kleineres Format).
Text rechts.

```
[Label: ÜBER MICH]

[H2, Cormorant Italic, Bordeaux, groß]
Ich rede nicht über diesen Zustand.
Ich habe ihn im Körper erlebt.

[Jost 300, #1A1A1A, 1rem, line-height 1.9]
Klassisches Ballett ab fünf Jahren.
Mit 13 München, Talentschmiede des Bayerischen Staatstheaters.
Leisten, funktionieren, psychosomatische Beschwerden —
über jede Grenze hinaus.

Mit 15 die Prüfung vor John Neumeier.
Der erkannte, was ich mir selbst vorher nicht eingestehen konnte.

Und dann stellte er mir eine Frage:

[Cormorant Italic, #4A4A4A]
Du kannst. Aber willst du das hier wirklich?

[Jost 300, #1A1A1A]
Danach: ALL-AACHT-Kampfkunst. Faszien. Atem. Somatik.
20 Jahre Körperarbeit mit Frauen.

Und immer wieder derselbe Punkt:
Symptome, die bleiben — egal wie präzise die Arbeit ist.
Weil ihre Ursachen woanders sitzen.

Das hat mich zur Yager Mind Matrix geführt.
Und zu der Erkenntnis,
dass Veränderung oft nicht dort passiert,
wo wir sie normalerweise suchen.

Daraus ist mein eigener Ansatz entstanden.

[Cormorant Italic, Terrakotta, mit Terrakotta-Linie links, padding-left 1.5rem]
Yager ist der Ursprung.
Bewusstseinsarchitektur ist mein Weg.
```

---

### 09 · TESTIMONIALS 2+3 (Bordeaux · überlappend)

WOW-LAYOUT:
2 Karten auf Bordeaux.
Linke Karte: normaler Start.
Rechte Karte: margin-top 4rem.
Beide mit großem Anführungszeichen Terrakotta opacity 0.1.
Karten: rgba(255,255,255,0.05) Hintergrund, 1px rgba(255,255,255,0.12) Rand.

```
[Karte links — Cormorant Italic, #FFFFFF, 1.3rem]
„Ich habe nicht erwartet, dass sich mein Körper verändert.
Aber auch nicht, dass ich aufhöre,
mein Wohlbefinden von der Meinung anderer abhängig zu machen.
Beides ist passiert."

[Jost 400, Terrakotta, 0.75rem]
Elena C. · Projektleiterin

[Karte rechts]
„Die Schuldgefühle, die ich jahrelang mit mir getragen habe —
sie sind einfach nicht mehr da.
Ich weiß selbst nicht genau wie. Aber es ist so."

[Jost 400, Terrakotta, 0.75rem]
Nadine H. · Ärztin
```

---

### 10 · WAS SICH VERÄNDERT (Licht)

WOW-LAYOUT:
Links (45%): Intro-Text + 4 konkrete Momente (Cormorant Italic mit Terrakotta-Linie links).
Rechts (55%): 4 Bereiche im 2x2 Grid mit Terrakotta-Checkmarks.

```
[Cormorant Italic, Bordeaux, clamp(1.8rem, 3vw, 2.8rem)]
Vielleicht spürst du zuerst Müdigkeit.
Ein erstes Loslassen.

[Jost 300, #4A4A4A]
Dann wird es klarer. Nicht dramatisch.
Eher in kleinen Momenten.

[4 Momente — Cormorant Italic, Bordeaux, 1.2rem,
 4px Terrakotta-Linie links, padding-left 1.2rem, margin-bottom 2rem]
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

[Rechts — 4 Quadranten 2x2]
[Titel: Jost 400, Bordeaux]
[Text: Jost 300, #4A4A4A]

✓ Körperlich
Das Nervensystem beruhigt sich.
Die Symptome flachen ab.
Der Schlaf wird tiefer.

✓ Zwischenmenschlich
Du nimmst deinen Partner wieder wahr.
Wählst bewusst, wann du Freunde treffen willst.
Kannst Grenzen setzen, ohne zu verletzen.

✓ Beruflich
Du beendest ein großes Projekt.
Stehst vor dem Ergebnis.
Und sagst dir: Ja. Das habe ich gut gemacht.

✓ Innerlich
Du reagierst nicht mehr automatisch.
Du atmest aus. Und wählst.
Nicht weil du es dir antrainiert hast —
sondern weil innen etwas anders geworden ist.
```

Abschluss — volle Breite, zentriert:

```
[Cormorant Italic, Bordeaux, sehr groß, zentriert]
Du weißt was du weißt.
Und das reicht.

[Jost 300, #4A4A4A, zentriert]
Das ist die wahre Qualität
in dem Spalt zwischen Reiz und Reaktion.

Innere Stimmigkeit. Das Äußere folgt nach.
```

---

### 11 · ANGEBOTE (Bordeaux)

WOW-LAYOUT:
Mittlere Karte (Deep Shift): transform translateY(-2.5rem).
Terrakotta-Rand oben 3px auf mittlerer Karte.
Mittlere Karte: rgba(255,255,255,0.07) Hintergrund.
Äußere: rgba(255,255,255,0.03) Hintergrund.
Alle Karten: 1px rgba(255,255,255,0.12) Rand.

```
[Label: ANGEBOTE]
[H2, Cormorant Italic, #FFFFFF]
So arbeiten wir zusammen.

[Karte 1 — Klarheitsgespräch]
[Preis: Cormorant Italic, #FFFFFF, 2.5rem]
0 €
[Jost 400, rgba(255,255,255,0.8)]
30 Minuten
[Jost 300, rgba(255,255,255,0.9)]
Du willst wissen, ob das hier das Richtige für dich ist.
Kein Pitch. Keine Agenda.
Wir schauen gemeinsam hin.
[btn--light]
Anfragen →

[Karte 2 — Deep Shift — translateY(-2.5rem)]
[Tag: Jost 400, Terrakotta, letter-spacing 0.18em]
KERNANGEBOT
[Preis: Cormorant Italic, Terrakotta, 3rem]
3.500 €
[Jost 400, rgba(255,255,255,0.9)]
12 Wochen · 6–8 Sessions · 1:1 online
[Jost 300, rgba(255,255,255,0.9)]
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
[btn--filled, weißer Hintergrund, Bordeaux-Text]
Klarheitsgespräch buchen →

[Karte 3 — Focus Shift]
[Preis: Cormorant Italic, #FFFFFF, 2.5rem]
450 €
[Jost 400, rgba(255,255,255,0.8)]
2 Sessions · 1 Thema
[Jost 300, rgba(255,255,255,0.9)]
Ein Thema. Zwei Sitzungen.
Ein gezielter Wendepunkt.

Für alle, die wissen, was sie bewegt —
und bereit sind, genau dort anzusetzen.
[btn--light]
Anfragen →
```

---

### 12 · FAQ (Licht · 2-Spalten-Accordion)

```
[Label: FRAGEN & ANTWORTEN]

[Linke Spalte — 3 Fragen]

Für wen ist das gedacht?
Für Frauen, die das Gefühl haben, mit dem Kopf allein nicht weiterzukommen.
Die innerlich an eine Grenze gestoßen sind und spüren,
dass da etwas ist, was sich verändern will.
Keine Vorkenntnisse nötig. Nur die Bereitschaft, wirklich hinzuschauen.

Wie läuft eine Sitzung ab?
Jede Sitzung ist anders, weil jeder Mensch anders ist.
Wir starten dort, wo du gerade bist.
Von da aus arbeiten wir gemeinsam.

Wie lange dauert der Prozess?
Das lässt sich nicht pauschal sagen.
Manche spüren nach wenigen Sitzungen eine spürbare Veränderung.
Wir schauen gemeinsam, was sinnvoll ist — ohne künstlichen Druck.

[Rechte Spalte — 3 Fragen]

Ich habe schon vieles versucht. Warum jetzt anders?
Weil wir auf einer anderen Ebene arbeiten.
Nicht an dem, was du denkst oder weißt.
Sondern an dem, was sich festgehalten hat.
Manchmal braucht es einfach einen anderen Zugang.

Ist das Therapie?
Nein. Bewusstseinsarchitektur ist kein therapeutisches Verfahren
und ersetzt keine psychotherapeutische oder medizinische Behandlung.
Bei akuten Erkrankungen wende dich an einen Arzt oder Therapeuten.

Ist das Hypnose?
Nein. Du bleibst vollständig bewusst und in Kontrolle.
Die Methode arbeitet über spezifische Kommunikationswege
mit dem Unterbewusstsein — ohne Trancezustand.
```

FAQ-Stil: Frage Jost 400 Bordeaux. Icon Terrakotta. Antwort Jost 300 #4A4A4A.

---

### 13 · FINAL CTA (Bordeaux · maximale Stille · viel Luft)

padding-block: min(10rem, 14vw).

```
[Label: BEREIT?]

[Cormorant Italic, #FFFFFF, clamp(2rem, 5vw, 4.5rem), zentriert, max-width 760px]
Wenn du beim Lesen gemerkt hast,
dass irgendwo etwas in dir
ruhig genickt hat —

[Jost 300, rgba(255,255,255,0.9), zentriert]
dann können wir sprechen.

In einem Gespräch schauen wir gemeinsam,
ob diese Arbeit für dich passt.

[btn--light, groß, padding 1rem 3.5rem, zentriert]
Klarheitsgespräch anfragen →

[Jost 400, rgba(255,255,255,0.75), sehr klein, zentriert]
Kostenlos · 30 Minuten · Kein Verkaufsdruck
```

---

### 14 · FOOTER (Bordeaux · border-top 1px rgba(255,255,255,0.08))

Links: `Julia Lauer · Bewusstseinsarchitektur` (Cormorant Italic, rgba(255,255,255,0.75))
Mitte: `© 2026` (Jost 400, rgba(255,255,255,0.5))
Rechts: `Impressum · Datenschutz` (Jost 400, rgba(255,255,255,0.75), hover #FFFFFF)

---

## ANIMATIONS & INTERAKTION

**Custom Cursor (pointer:fine only):**
Terrakotta Dot 6px + Ring 32px 1.5px border. Hover: scale(1.6) + 48px.

**Scroll Reveal:**
opacity 0→1 + translateY(30px)→0, 0.8s cubic-bezier(0.16,1,0.3,1).
Intersection Observer threshold 0.1.

**Hero:**
Label: fadeUp 0.8s delay 0.1s.
Tagline: fadeUp 0.8s delay 0.25s.
H1: Zeile für Zeile, clip von unten, 0.9s, 0.15s Delay zwischen Zeilen, ab delay 0.4s.
Subtext: fadeUp 0.8s delay 1s.
CTA: fadeUp 0.8s delay 1.2s.
Foto: scale(1.06)→scale(1), 8s ease-out, sofort.

**Terrakotta-Divider:**
width 0→48px, 0.8s cubic-bezier(0.16,1,0.3,1) beim Einblenden.

**Buttons:**
::before scaleX(0)→scaleX(1) from left, 0.35s. Magnetisch: ±8px max.

**Proof-Bar Counter:**
0→100+, 1.8s ease-out, beim Einblenden.

**Methode-Karten:**
::after Terrakotta-Linie: right 100%→0%, height 2px, bottom 0, 0.5s beim Hover.

**FAQ Accordion:**
max-height 0→content, 0.45s cubic-bezier(0.16,1,0.3,1).

**Noise auf Bordeaux-Sektionen:**
SVG fractalNoise, opacity 0.03.

**prefers-reduced-motion:**
Alle Animationen off. Alle data-reveal sofort sichtbar.

---

## TECHNISCHE ANFORDERUNGEN

- Eine HTML-Datei. Alles inline.
- Responsive: Mobile-first.
  - 860px: Nav-Links weg, Hamburger. Grids 1 Spalte.
  - 640px: Hero 1 Spalte (Bild unter Text). Proof-Bar wrap.
- Smooth Scroll
- Skip-Link, ARIA-Labels, focus-visible (Terrakotta)
- Google Fonts: preconnect + display=swap
- JSON-LD: Person + ProfessionalService + 3 Offers

```
title: Julia Lauer · Bewusstseinsarchitektur — für hochleistende Frauen
description: Für Frauen, die funktionieren — und die spüren: Ich kann so weitermachen. Aber ich will es nicht. Die Bewusstseinsarchitektur-Methode arbeitet unterhalb des Denkens.
canonical: https://bewusstseinsarchitektur.de/
theme-color: #3D1219
```

---

## DAS ZIEL

Sara landet hier. Liest drei Sätze.
Denkt: Die meint mich.

Scrollt.
Versteht: Das ist anders.

Liest die Testimonials.
Denkt: Das will ich auch.

Sieht den Preis.
Denkt: Das ist es wert.

Bucht.

Keine halben Sachen.
