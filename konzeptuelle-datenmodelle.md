## Konzeptuelle Datenmodelle

---

### Wiederholung: Schemata und Datenmodelle

<table style="font-size:0.5em">
    <thead>
        <tr>
            <th style="border-style: none">Typ des Schemas</th>
            <th style="border-style: none">Aufgabe des Schemas</th>
            <th style="border-style: none">Datenmodelle für das Schema</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border-style: none">logisches Schema</td>
            <td style="border-style: none">Beschreibung logischer Datenbankstrukturen</td>
            <td style="border-style: none">logische Datenmodelle</td>
        </tr>
        <tr class="fragment">
            <td style="border-style: none">physisches Schema</td>
            <td style="border-style: none">Beschreibung physischer Datenbankstrukturen</td>
            <td style="border-style: none">physische Datenmodelle</td>
        </tr>
    </tbody>
</table>

---

### Datenbankentwurf in zwei Phasen?

<table style="font-size:0.5em">
    <thead>
        <tr>
            <th style="border-style: none">Phasennr.</th>
            <th style="border-style: none">Phasenname</th>
            <th style="border-style: none">Typ des resultierenden Schemas</th>
            <th style="border-style: none">Aufgabe des resultierenden Schemas</th>
            <th style="border-style: none">Datenmodelle für das resultierende Schema</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="border-style: none">1</td>
            <td style="border-style: none">logischer Datenbankentwurf</td>
            <td style="border-style: none">logisches Schema</td>
            <td style="border-style: none">Beschreibung logischer Datenbankstrukturen</td>
            <td style="border-style: none">logische Datenmodelle</td>
        </tr>
        <tr class="fragment">
            <td style="border-style: none">2</td>
            <td style="border-style: none">physischer Datenbankentwurf</td>
            <td style="border-style: none">physisches Schema</td>
            <td style="border-style: none">Beschreibung physischer Datenbankstrukturen</td>
            <td style="border-style: none">physische Datenmodelle</td>
        </tr>
    </tbody>
</table>

---

#### Nachteile des zweiphasigen Datenbankentwurfs

- Resultierende Schemata sind abhängig von
    - der Wahl des logischen und physischen Datenmodells und damit
    - der Wahl des Datenbankverwaltungssystems.
- Resultierende Schemata beschreiben Implementierungssicht statt Anwendersicht.

---

### Datenbankentwurf in drei Phasen

<table style="font-size:0.5em">
    <thead>
        <tr>
            <th style="border-style: none">Phasennr.</th>
            <th style="border-style: none">Phasenname</th>
            <th style="border-style: none">Typ des resultierenden Schemas</th>
            <th style="border-style: none">Aufgabe des resultierenden Schemas</th>
            <th style="border-style: none">Datenmodelle für das resultierende Schema</th>
        </tr>
    </thead>
    <tbody>
        <tr class="fragment" style="color: #1b91ff">
            <td style="border-style: none">1</td>
            <td style="border-style: none">konzeptueller Datenbankentwurf</td>
            <td style="border-style: none">konzeptuelles Schema</td>
            <td style="border-style: none">Beschreibung der Miniwelt und ihrer Gesetzmäßigkeiten</td>
            <td style="border-style: none">konzeptuelle Datenmodelle</td>
        </tr>
        <tr>
            <td style="border-style: none">2</td>
            <td style="border-style: none">logischer Datenbankentwurf</td>
            <td style="border-style: none">logisches Schema</td>
            <td style="border-style: none">Beschreibung logischer Datenbankstrukturen</td>
            <td style="border-style: none">logische Datenmodelle</td>
        </tr>
        <tr>
            <td style="border-style: none">3</td>
            <td style="border-style: none">physischer Datenbankentwurf</td>
            <td style="border-style: none">physisches Schema</td>
            <td style="border-style: none">Beschreibung physischer Datenbankstrukturen</td>
            <td style="border-style: none">physische Datenmodelle</td>
        </tr>
    </tbody>
</table>

Anmerkungen:

- Alternative Bezeichnung ist <q>semantisches Datenmodell</q> anstelle von <q>konzeptuelles Datenmodell</q>.
- Aber dann geht die schöne Regelmäßigkeit in dieser Tabelle kaputt.
- Deshalb verwenden wir in dieser Vorlesung bevorzugt den Begriff <q>konzeptuelles Datenmodell</q>.

---

### Konzeptuelles Datenmodell

<ul>
  <li>
    Definition
    <ul>
      <li>formales Konzept zur Beschreibung der Miniwelt und ihrer Gesetzmäßigkeiten</li>
    </ul>
  <li class="fragment" data-fragment-index="1">
    alternative Bezeichnung
    <ul>
      <li>semantisches Datenmodell</li>
    </ul>
  </li>
  <li class="fragment" data-fragment-index="2">
    Beispiele
    <ul>
      <li>
        objektorientierte Entwurfsmodelle (z.&thinsp;B. UML)
      </li>
      <li class="fragment highlight-red" data-fragment-index="2">
        Entity-Relationship-Modell (ERM)
      </li>
      <li class="fragment highlight-red" data-fragment-index="2">
        semantisches Datenmodell der Informationsanalyse
      </li>
    </ul>
  </li>
</ul>

Anmerkungen:

- UML haben Sie sicher schon im Rahmen der objektorientierten Programmierung kennengelernt.
- Die anderen beiden Beispiele werden wir uns jetzt genauer ansehen.
