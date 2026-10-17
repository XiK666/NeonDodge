# NEON DODGE · KI – Anleitung

Diese Anleitung erklärt dir, wie du die KI startest, wie sie lernt und was die Anzeigen bedeuten.
Du brauchst nichts zu installieren. Alles läuft in deinem Browser, ohne Internet und ohne dein Claude-Limit.

---

## 1. Starten

1. Öffne den Ordner **„Neon Dodge“**.
2. Doppelklicke auf **`neon-dodge-ki.html`**. Die Seite öffnet sich in deinem Browser.
3. Klicke rechts oben auf **„▶ TRAINING STARTEN“**.

Mehr musst du nicht tun. Links siehst du die KI spielen, rechts liest du ihre Gedanken.

> Dein normales Spiel `neon-dodge.html` bleibt unverändert. Deine Bestwerte und Shop-Käufe dort werden von der KI nicht angerührt.

---

## 2. Was du am Anfang siehst

Vor dem Training hat die KI ein **Zufalls-Gehirn**. Sie zappelt herum und stirbt schnell. Das ist normal.

Sobald das Training läuft, wird sie besser. Erwarte ungefähr:

| Trainingszeit | Was passiert |
|---|---|
| erste Minute | Die KI bekommt ein Gefühl für die Wände und weicht ab und zu aus. |
| 5–15 Minuten | Sie weicht Kugeln gezielt aus und überlebt öfter einen Boss. |
| 30–60 Minuten und mehr | Sie spielt deutlich ruhiger und überlebt auf „Easy“ oft lange. |

Diese Zeiten sind nur Richtwerte. Lernen ist ein Zufallsprozess: Mal gibt es Sprünge, mal geht es eine Weile kaum voran.

---

## 3. Wie die KI lernt (einfach erklärt)

Die KI lernt wie in der **Evolution**:

1. Es gibt **60 KIs**, jede mit einem eigenen kleinen Gehirn.
2. Jede KI spielt **3 Runden**. Gezählt werden ihre Punkte.
3. Die **besten KIs** bekommen „Kinder“. Das sind Kopien mit kleinen, zufälligen Änderungen am Gehirn.
4. Die schlechten KIs fallen weg.
5. Das ist eine **Generation**. Danach geht alles von vorn los.

So setzen sich über viele Generationen die Gehirne durch, die gut ausweichen.

Das Training läuft im Hintergrund **viel schneller als Echtzeit**, auf deinem Rechner etwa 2.000- bis 4.000-mal so schnell. Deshalb schafft die KI in einer Minute Tausende Trainingsrunden.

**Was die KI wahrnimmt:**
- Wie nah Gefahren sind, aufgeteilt in 16 Richtungen rund um sich herum
- Ob eine Gefahr auf **Kollisionskurs** ist, also ob sie treffen würde, wenn die KI stehen bleibt
- Wie nah die Wände sind
- Ob ihr Dash bereit ist, ob sie einen Schild hat und wo das nächste Power-up liegt

**Was die KI tun kann:** sich in 8 Richtungen bewegen, stehen bleiben und den Dash benutzen.

---

## 4. Die Anzeigen

### Lernfortschritt
- **Generation:** Wie viele Lern-Durchgänge schon fertig sind.
- **Rekord:** Die höchste Punktzahl, die je eine KI in einem einzelnen Trainingsspiel geholt hat.
- **Beste KI der letzten Generation:** Die Durchschnittspunkte der besten KI über ihre 3 Runden.
- **Durchschnitt aller KIs:** Wie gut die ganze Gruppe im Schnitt ist. Wenn diese Zahl steigt, lernt die KI wirklich.

### Gedanken der KI (innerer Monolog)
Etwa alle 1,5 Sekunden erklärt die KI, was sie gerade tut:

- **Was sie sieht:** zum Beispiel „Eine Kugel von rechts ist auf Kollisionskurs – Einschlag in 0,4 s“.
- **Was sie entscheidet:** zum Beispiel „Entscheidung: nach oben (80 % sicher)“. Die Prozentzahl zeigt, wie klar diese Richtung gegenüber den anderen gewinnt.
- **Warum:** Hier wird die KI wirklich geprüft. Wir blenden jede Gefahr testweise aus und schauen, ob sie sich dann anders entscheiden würde. Wenn ja, war diese Gefahr ein echter Grund.

> **Ehrlicher Hinweis:** Ein neuronales Netz denkt nicht in Worten. Die Sätze sind eine Übersetzung dessen, was das Netz tatsächlich wahrnimmt und wie es tatsächlich entscheidet. Erfunden wird nichts. Ein Sprachmodell wie Claude ist dafür nicht im Spiel.

Farben im Monolog:
- **blau** = normaler Gedanke
- **rot** = Gefahr oder Treffer
- **gelb** = Ereignis (Power-up, Boss, knapp vorbei)
- **lila** = Das Spiel selbst stellt der KI eine Falle

Das **Kästchen mit den Pfeilen** zeigt live, wie stark die KI jede Richtung gerade bevorzugt. Je heller, desto lieber.

### Zuschauen
- **Tempo 1× / 2× / 4×:** Die KI im Bild spielt schneller. Auf das Training hat das keinen Einfluss.
- **Sinne anzeigen:** Um die KI erscheint ein Radar. **Blau** heißt, da ist etwas in der Nähe. **Rot** heißt, das ist auf Kollisionskurs. Der **grüne Pfeil** zeigt, wohin sie gehen will.
- **Spiel passt sich an:** Das Spiel hat einen eingebauten Gegner, der sich merkt, wie du spielst. Ist das Häkchen gesetzt, merkt er sich beim Zuschauen auch die KI. Im Training ist das immer aus, damit die KI ein faires, gleichbleibendes Ziel hat.

Im Bild spielt immer die **beste KI der zuletzt fertigen Generation**. Nach jeder Runde kommt automatisch die neueste beste KI dran.

### Verlauf
Die **Lernkurve**: Die grüne Linie zeigt die beste KI je Generation, die blaue den Durchschnitt. Wenn beide nach oben gehen, lernt die KI.

---

## 5. Einstellungen

- **Schwierigkeit:** Fang mit **Easy** an. Wenn die KI dort gut ist, schalte auf Medium und später höher. Sie behält dabei alles, was sie schon gelernt hat, und trainiert auf der neuen Stufe weiter.
- **Rechenleistung:**
  - **Sparsam:** 1 Prozessorkern. Leise und kühl, aber langsameres Lernen.
  - **Normal:** die Hälfte der Kerne. Das ist die Voreinstellung.
  - **Maximal:** fast alle Kerne. Am schnellsten, aber der Lüfter wird lauter.

  Eine Grafikkarte wird nicht gebraucht.

**Tastenkürzel:** Die **Leertaste** startet oder pausiert das Training.

---

## 6. Speichern

- Der Fortschritt wird **automatisch im Browser gespeichert**. Du kannst die Seite schließen und später einfach weitermachen.
- **„Stand sichern (Datei)“** lädt eine Sicherungsdatei herunter. Das ist sinnvoll, bevor du den Browserverlauf löschst oder einen anderen Browser benutzt.
- **„Stand laden“** holt eine Sicherungsdatei zurück.
- **„Neu anfangen“** löscht alles Gelernte. Vorher wirst du gefragt.

> Wichtig: Der automatische Speicherstand hängt am Browser. Öffnest du die Datei in einem anderen Browser, etwa Firefox statt Chromium, fängt die KI dort von vorn an. Nimm dann „Stand sichern“ und „Stand laden“.

---

## 7. Häufige Fragen

**Die KI wird nicht besser.**
Gib ihr Zeit. Zwischendurch gibt es oft Phasen, in denen sich lange wenig tut. Schau auf die blaue Durchschnittslinie: Sie ist aussagekräftiger als einzelne Spiele.

**Die KI im Bild spielt schlechter, als die Zahlen sagen.**
Jedes Spiel ist anders, und auch eine gute KI hat mal Pech. Die Zahlen sind Durchschnitte über mehrere Runden.

**Mein Laptop wird warm oder laut.**
Stell die Rechenleistung auf „Sparsam“ oder pausiere das Training.

**Braucht das Internet oder mein Claude-Limit?**
Nein. Alles läuft nur auf deinem Rechner.

**Was bedeutet „Rundenlimit“?**
Damit eine Generation nicht ewig dauert, endet ein Trainingsspiel nach einer Höchstzeit, anfangs 90 Sekunden. Wird die KI so gut, dass sie das regelmäßig schafft, wird das Limit automatisch verlängert, bis maximal 10 Minuten.
