## Rückblick:<br/>Logische Datenmodelle

---

### Logisches Datenmodell

<ul>
  <li>
    Definition
    <ul>
      <li>formales Konzept zur Beschreibung von logischen Datenbankstrukturen</li>
    </ul>
  <li class="fragment">
    Beispiele
    <ul>
      <li>
        <strong>RDM:</strong>
        <span class="fragment">relationales Datenmodell</span>
      </li>
      <li>
        <strong>ODM:</strong>
        <span class="fragment">Objektdatenmodell</span>
      </li>
      <li>
        <strong>ORDM:</strong>
        <span class="fragment">objektrelationales Datenmodell</span>
      </li>
    </ul>
  </li>
</ul>

---

### Relationales Datenmodell

<ul>
  <li>
    <strong>Domäne:</strong>
    Menge, die nur atomare Elemente enthält.
  </li>
  <li class="fragment">
    <strong><em>n</em>-Tupel:</strong>
    Element des kartesischen Produkts<br/>von <em>n</em> Domänen: <em>(d1,d2,…,dn)∈D1⨯D2⨯⋯⨯Dn</em>.
  </li>
  <li class="fragment">
    <strong><em>n</em>-stellige Relation:</strong>
    Teilmenge des kartes. Produkts<br/>von <em>n</em> Domänen: <em>R⊆D1⨯D2⨯⋯⨯Dn</em>.
  </li>
  <li class="fragment">
    <strong>Tabelle:</strong>
    Multimenge über <em>D1⨯D2⨯⋯⨯Dn</em>.<br/>Kann jeden Tupel mehrfach enthalten.
  </li>
</ul>

---

#### Beispiel: Lieferantendatenbank

<div style="float: left; width: 60%">
    <h5>Informationszusammenhänge</h5>
    <ol style="font-size: 0.7em">
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
            Ein <strong>Systemhersteller</strong> produziert <strong>Produkte</strong> an einem <strong>Ort</strong>.
        </li>
    </ol>
</div>
<div class="fragment" style="float: right; width: 35%">
    <h5>Relationale Datenbank</h5>
    <figure>
        <img alt="Die Lieferantendatenbank enthält die Tabellen LIEFERANT, KAPAZITÄT, SYSTEMHERSTELLER und PRODUKT"
             src="images/lieferantendatenbank.png"
             style="margin-top: 0"/>
        <figcaption style="font-size: 0.5em">Quelle: Kern-Bausch, Jeckle (2001)</figcaption>
    </figure>
</div>
