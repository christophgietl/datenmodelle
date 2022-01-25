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
    - Zusammenfassung analog zu den Entitätstypen

---

#### Weitere Grundbegriffe des Entity-Relationship-Modells

- Attribute
    - dienen der Charakterisierung von Entitäten und Beziehungen
- Schlüsselkandidaten und Schlüssel
    - analog zum relationalen Datenmodell
- Kardinalität
- Obertyp *(super type)* und Untertyp *(sub type)*

---

#### Beispiel für ein konzeptuelles Schema im Entity-Relationship-Modell

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

##### Konzeptuelles Schema in grafischer Notation des Entity-Relationship-Modells

TODO: Grafik

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
            <td style="border-style: none">TODO</td>
            <td style="border-style: none">TODO</td>
        </tr>
        <tr>
            <td style="border-style: none">TODO</td>
            <td style="border-style: none">TODO</td>
            <td style="border-style: none">TODO</td>
        </tr>
    </tbody>
</table>
