## <em style="color: #ff2c2d; font-style: normal">Semantisches Datenmodell<br/>der Informationsanalyse</em>

---

### Informationsanalyse

- systematisches Vorgehen zur Entwicklung und Beschreibung des konzeptuellen Schemas
- besteht aus mehreren Vorgehensschritten

---

#### Vorgehensschritte der Informationsanalyse

1. Sammle alle relevanten **Objekte**.
2. Fasse Objekte zu **Objekttypen** zusammen.
3. Formuliere alle **Beziehungen** zwischen den Objekttypen.
4. Sammle für alle Objekttypen alle **Eigenschaften** der Objekte.
5. Lege für alle Objekttypen eine **Namenskonvention** fest, d.&thinsp;h. eine eindeutige Benennung der Objekte.
6. Erfasse **Metainformationen**,<br/>
   d.&thinsp;h. weitere semantische Gesetzmäßigkeiten<br/>
   (z.&thinsp;B. Bedingungen oder Konsistenzregeln).

---

### Semantisches Datenmodell der Informationsanalyse

- textuelle Notation für das Ergebnis der Informationsanalyse
- grafische Notation für das Ergebnis der Informationsanalyse

---

#### Beispiel: Lieferanteninformation in grafischer Notation

<figure>
    <img alt="Aus dem konzeptuellen Schema werden ein internes Schema (für die Datenbanken) und mehrere externe Schemata (für Gruppen menschlicher Nutzer:innen und für Anwendungen) abgeleitet."
         src="images/semantisches-datenmodell-lieferanteninformation.png"/>
    <figcaption style="font-size: 0.5em">Quelle: Kern-Bausch, Jeckle (2001)</figcaption>
</figure>

---

#### Konzepte des semantischen Datenmodells der Informationsanalyse

- Objekttyp
- Assoziationstyp
    - *n*-näre Beziehung zwischen Objekttypen *(n≥2)*,<br/>
      die in dieser Beziehung bestimmte Rollen spielen
- Kardinalität (Mitgliedschaftsintervall)
    - TODO
- Obertypen und Untertypen
- verpflichtende Eigenschaften (Kardinalität ≥1)
- optionale Eigenschaften (Kardinalität ≥0)
- Namenskonventionen (TODO)
- Datentypen
- Metainformationen

---

#### Semantische Irreduzibilität von Assoziationstypen

- Definition
    - Ein Assoziationstyp heißt *semantisch irreduzibel*, wenn er nicht ohne Informationsverlust weiter zerlegt werden
      kann.
- Vorteile  <!-- .element: class="fragment" -->
    - macht das konzeptuelle Schema stabil gegenüber Erweiterungen
    - ermöglicht die Ableitung anomaliefreier Datenbankstrukturen
