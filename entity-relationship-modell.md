## <em style="color: #ff2c2d; font-style: normal">Entity-Relationship-Modell</em>

---

### Entity-Relationship-Modell

- konzeptuelles Datenmodell
- basiert auf dem Begriff der <q style="font-style: normal">Entität</q>
- bietet grafische Notation<br/>(sogenannte Entity-Relationship-Diagramme, ERD)

---

#### Grundbegriffe des Entity-Relationship-Modells

- Entitäten
    - wohlunterscheidbare Konzepte der Miniwelt
    - existieren physisch oder gedanklich
- Entitätstyp
    - Zusammenfassung ähnlicher Entitäten
- Beziehung *(relationship)*
    - zwischen Entitäten
    - benannt
- Beziehungstyp *(relationship type)*
    - Zusammenfassung ähnlicher Beziehungen
    - analog zu den Entitätstypen

---

#### Warnhinweis zum Sprachgebrauch <!-- .element style="color: #ff2c2d; font-style: normal" --> 

- Häufig wird von <q style="font-style: normal">Entität</q> gesprochen,<br/>
  obwohl eigentlich <q style="font-style: normal">Entitätstyp</q> gemeint ist.
- Häufig wird von <q style="font-style: normal">Beziehung</q> gesprochen,<br/>
  obwohl eigentlich <q style="font-style: normal">Beziehungstyp</q> gemeint ist.

---

#### Weitere Grundbegriffe des Entity-Relationship-Modells

- Attribute
    - dienen der Charakterisierung von Entitäten und Beziehungen
- Schlüsselkandidaten und Primärschlüssel
    - analog zum relationalen Datenmodell
- Kardinalität
- Obertyp *(super type)* und Untertyp *(sub type)*
    - Erweiterung des ursprünglichen Entity-Relationship-Modells

---

#### Beispiel für ein konzeptuelles Schema gemäß Entity-Relationship-Modell

#### Semantische Regeln der Lieferanteninformation (Kern-Bausch, Jeckle (2001))

<ol style="font-size: 0.8em">
    <li>
        Ein <strong>Lieferant</strong> hat
        <ul>
            <li>eine eindeutige Nummer,</li>
            <li>einen eindeutigen Namen und</li>
            <li>einen Firmensitz, der zu einer Region gehört.</li>
        </ul>
    </li>
    <li class="fragment">
        Ein <strong>Produkt</strong> hat
        <ul>
            <li>einen eindeutigen Produkttyp,</li>
            <li>einen Namen,</li>
            <li>eine optionale Materialangabe und</li>
            <li>einen Richtpreis.</li>
        </ul>
    </li>
    <li class="fragment">
        Ein <strong>Lieferant</strong> kann von einem <strong>Produkt</strong> eine maximale Menge (Kapaz) liefern.
    </li>
    <li class="fragment">
        Ein <strong>Systemhersteller</strong> produziert <strong>Produkte</strong> an <strong>Orten</strong>.
    </li>
</ol>

---

##### Konzeptuelles Schema der Lieferanteninformation<br/>gemäß Entity-Relationship-Modell

<figure>
    <img alt="Aus dem konzeptuellen Schema werden ein internes Schema (für die Datenbanken) und mehrere externe Schemata (für Gruppen menschlicher Nutzer:innen und für Anwendungen) abgeleitet."
         src="images/erm-lieferanteninformation.png"/>
    <figcaption style="font-size: 0.5em">Quelle: Skizze des Dozenten</figcaption>
</figure>

---

##### Grafische Darstellung der Grundbegriffe des Entity-Relationship-Modells

<table style="font-size:0.5em">
    <thead>
        <tr>
            <th style="border-style: none">Grundbegriff</th>
            <th style="border-style: none">grafische Darstellung</th>
            <th style="border-style: none">Instanzen</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border-style: none">Entitätstyp</td>
            <td style="border-style: none">Rechteck mit Name</td>
            <td style="border-style: none">Lieferant, Ort, Produkt, Region, Systemhersteller</td>
        </tr>
        <tr>
            <td style="border-style: none">Beziehungstyp</td>
            <td style="border-style: none">Rhombus mit Name, Linien zu den Entitätstypen</td>
            <td style="border-style: none">gehört zu, kann liefern, produziert, sitzt in</td>
        </tr>
        <tr>
            <td style="border-style: none">Attribut</td>
            <td style="border-style: none">Oval mit Name, Linie zum Entitätstyp</td>
            <td style="border-style: none">Herstellername, Herstellernr., Kapazität, Lieferantenname, Lieferantennr., …</td>
        </tr>
        <tr>
            <td style="border-style: none">Schlüsselkandidat</td>
            <td style="border-style: none">keine</td>
            <td style="border-style: none">Lieferantenname</td>
        </tr>
        <tr>
            <td style="border-style: none">Primärschlüssel</td>
            <td style="border-style: none">Unterstreichung</td>
            <td style="border-style: none">Herstellernr., Lieferantennr., Postleitzahl, Produkttyp, Regionenname</td>
        </tr>
        <tr>
            <td style="border-style: none">Kardinalität</td>
            <td style="border-style: none">Zeichen am Entitätstyp-Ende der Linie</td>
            <td style="border-style: none">1, L, M, N</td>
        </tr>
    </tbody>
</table>
