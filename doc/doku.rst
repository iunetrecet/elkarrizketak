=========
Ahomentan
=========

Ahomentanen karpetaren barnean, fitxategi hauek edukiko ditugu:

- **bower_components** Bootstrapen osagai guztiak *(ez dugu ikutuko)*
- **doc** Dokumentazioa
- **liburutegia** Hemen edukiko ditugu html-an sartu beharreko osagaiak
- **index.html** Hemen kopiatuko dugu elkarriketaren html
- **assets**

  - **css** Igo beharreko css fitxategiak *(ez dugu ikutuko)*
  - **fonts** Webgunerako igoko diren letra tipoak *(ez dugu ikutuko)*
  - **less** Estiloak hemen daude definituak *(ez dugu ikutuko)*
  - **images** Irudi guztiak hemen egongo dira, hemen igo beharko ditugu elkarrizketan sartuko ditugun argazki guztiak

Edukia sartzeko eman beharreko pausoak
--------------------------------------

Headerrean izenak
`````````````````

Lehenengo pausoa, headerrean izenak jartzea da. *index.html* fitxategian,
*header* etiketak dauden lekuan, elkarrizketatuaren izenak sartu behar dira.

    .. code:: html
      <header>
        <div class="headerTestua">
          <h2><a href="#lehenengoa">Unai Iturriaga</a></h2>
          <h1><a href="http://berria.eus/ahomentan"><svg xmlns:svg="http://www.w3.org/2000/svg" xmlns="http://www.w3.org/2000/svg" xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd" xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape" width="76.00116mm" height="53.491154mm" viewBox="0 0 76.00116 53.491154" id="svg6292" sodipodi:docname="ahomentan.svg"><g inkscape:label="Capa 1" inkscape:groupmode="layer" id="layer1" transform="translate(-67.454803,-79.009331)"><path style="fill:#ff0066;fill-opacity:1;stroke:none;stroke-width:0.36387315;stroke-miterlimit:4;stroke-dasharray:none;stroke-opacity:1" d="m 137.55214,79.009331 -7.43544,11.67078 H 70.617379 c -1.752212,0 -3.162576,1.410411 -3.162576,3.162468 v 23.824631 c 0,1.75206 1.410364,3.1625 3.162576,3.1625 h 2.741609 v 11.67078 l 7.43532,-11.67078 h 59.499082 c 1.75209,0 3.16257,-1.41044 3.16257,-3.1625 V 93.842579 c 0,-1.752057 -1.41048,-3.162468 -3.16257,-3.162468 h -2.74125 z" id="karratua" inkscape:connector-curvature="0" sodipodi:nodetypes="ccsssscccsssscc" /><text font-size="26.238" id="text5806-9" x="74.104805" y="109.82698"><tspan style="font-weight:bold;font-family:LatoRegular;font-size:12.57639217px;fill:#ffffff;"id="tspan5898-3">ahomentan</tspan></text></g></svg></a><a href="#titularra"><span class="glyphicon glyphicon-chevron-down"></span></a></h1>
          <h2><a href="#bigarrena">Igor Elortza</a></h2>
        </div>
      </header>

Headerrarena irudia
```````````````````

Azaleko irudiak beti izen berdina izango du, *azala.jpg*. *assets/images*
karpetaren barnean *azala.jpg* izenarekin sartuko dugu hasieran fondoan jarri
nahi dugun irudia.


Sinadura
````````

Kazetariaren sinadura jartzeko *sinadura.html*-en dagoena kopiatu eta pegatu
beharko da.

    .. code:: html

      <p class="sinadura"><span class="glyphicon glyphicon-pencil"></span> Izena eta Abizena
          <span class="sinadura-data">Arrasate</span></p>

Irudi horizontalak
``````````````````

Irudi horizontalak bi motatakoak izango dira:

1. **Azpitutalarren azpian doana,** *irudi_horizontala_azpititularra.html*
   fitxategian dagoena kopiatu eta pegatu behar da.

    .. code:: html

      <div class="irudi horizontala">
        <img src="assets/images/horizontala.png"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</label></p>
      </div>

  Irudiaren izena, oina eta sinadura bete behar dira.

2. **Testuaren barruan doana,** *irudi_horizontala.html* fitxategian dagoena
   kopiatu eta pegatu behar da nahi den lekuan.

    .. code:: html

      </p>
      <div class="irudi horizontala">
        <img src="assets/images/bertikala.png"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</label></p>
      </div>
      <p class="testua">

  Irudiaren izena, oina eta sinadura bete behar dira.

Irudi bertikala
```````````````

Irudi bertikalak beti testu barruan sartuko dira.
*irudi_bertikala.html* fitxategian dagoena kopiatu eta pegatu behar da nahi
den lekuan.

    .. code:: html

      <span class="irudi bertikala">
        <img src="assets/images/bertikala.png"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</span></label>
      </span>

  Irudiaren izena, oina eta sinadura bete behar dira.

Irudi panoramikoa
`````````````````

Irudi panoramikoak beti testu barruan sartuko dira.
*irudi_panoramikoa.html* fitxategian dagoena kopiatu eta pegatu behar da nahi
den lekuan.

    .. code:: html

      <div class="irudi panoramikoa">
        <img src="assets/images/panoramikoa.png"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</span></label>
      </div>

  Irudiaren izena, oina eta sinadura bete behar dira.

Esanak
``````

Esanak beti testu barruan sartuko dira.
Bi esan mota daude *esanak.html* fitxategiaren barruan.

1. **Karetoa ezkerrean** daukan esana, lehenengoa izango dena. Klase bezala *esanak*
   bakarrik du.

    .. code:: html

      <section class="esanak">
        <div class="esanakEdukia">
          <img class="karetoa" src="assets/images/karetoa.png" />
          <div class="esanakTestua">
            <p>"Esaldia hemen kopiatu"</p>
            <p class="sinadura">Izena</p>
          </div>
        </div>
      </section>

    Karetoaren izena, esaldia eta izena bete behar dira.

2. **Karetoa eskubian** daukan esana, bigarrena izango dena. Klase bezala *esanak* eta *bigarrena* ditu.

    .. code:: html

      <section class="esanak bigarrena">
        <div class="esanakEdukia">
          <div class="esanakTestua">
            <p>"Esaldia hemen"</p>
            <p class="sinadura">Izena</p>
          </div>
          <img class="karetoa" src="assets/images/karetoa.png" />
        </div>
      </section>

    Karetoaren izena, esaldia eta izena bete behar dira.

Fitxak
``````

Fitxak beti bukaeran jarri behar dira. *fitxak.html* fitxategian dagoena bete
behar da.

    .. code:: html

      <section class="nor">
        <div class="pertsonaia" id="lehenengoa">
          <h1>Izen Abizenak</h1>
          <h2>(Herria, urtea)</h2>
          <p>Testua</p>
        </div>
        <div class="pertsonaia" id="bigarrena">
          <h1>Izen Abizenak</h1>
          <h2>(Herria, urtea)</h2>
          <p>Testua</p>
        </div>
      </section>
