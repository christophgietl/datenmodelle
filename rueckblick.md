## Zuletzt in der<br/>Datenbanken-Vorlesung

---

### Grundbegriffe

- Datenbank *(database, DB)*
- Datenbankverwaltungssystem<br/>*(database management system, DBMS)*
- Datenbanksystem *(database system, DBS)*
- Schema *(schema)*
- konzeptuelles Schema *(conceptual schema)*

---

### Anforderungen an Datenbankverwaltungssysteme (Auszug)

- **Physische Datenunabhängigkeit**
    - Ort und Art der physischen Abspeicherung dürfen Anwendungen nicht beeinflussen.
- **Logische Datenunabhängigkeit**
    - Informationserhaltende Änderungen der Datenbanklogik dürfen Anwendungen nicht beeinflussen.
- **Sichten auf die Datenbank**
- **Rechtevergabe**

---

### Drei-Schema-Architektur

- **externes Schema**
    - beschreibt
        - benötigte Sicht externer Nutzer:innen und Applikationen
        - die ihnen eingeräumten Rechte
    - leitet sich aus dem *konzeptuellen Schema* ab
- **internes Schema**
    - beschreibt
        - physische Abspeicherung
        - Zugriffsorganisation
    - leitet sich aus dem *konzeptuellen Schema* ab

Anmerkungen:

- physische Abspeicherung und Zugriffsorganisation später im Semester
- heute mehr zum konzeptuellen Schema

---

#### Visualisierung der Drei-Schema-Architektur

<figure>
    <img alt="Aus dem konzeptuellen Schema werden ein internes Schema (für die Datenbanken) und mehrere externe Schemata (für Gruppen menschlicher Nutzer:innen und für Anwendungen) abgeleitet."
         src="images/drei-schema-architektur.png"/>
    <figcaption style="font-size: 0.5em">Quelle: Kern-Bausch, Jeckle (2001)</figcaption>
</figure>


Anmerkungen:

- *mehrere* externe Schemata
    - für verschiedene Gruppen menschlicher Nutzer:innen
    - für verschiedene Applikationen
- *ein* internes Schema
- Alle werden aus dem konzeptuellen Schema abgeleitet.
