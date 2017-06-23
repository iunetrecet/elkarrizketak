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
        <h1>
          <a href="http://berria.eus/ahomentan">
            <img class="smallHeader"
              src="assets/images/ahomentan_txikia.svg" alt="Ahomentan">
          </a>
        </h1>
        <div class="headerTestua">
          <h2><a href="#lehenengoa">Unai Iturriaga</a></h2>
          <div class="bigHeader">
            <a class="ahomentan" href="http://berria.eus/ahomentan">
              <img src="assets/images/ahomentan.svg" alt="Ahomentan"/></a>
            <a class="down" href="#titularra">
              <span class="glyphicon glyphicon-chevron-down"></span></a>
          </div>
          <h2><a href="#bigarrena">Igor Elortza</a></h2>
        </div>
      </header>

    Lehenengoa eta bigarrena dagoen lekuan jarri beharko dira.

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

      <p class="sinadura"><span class="glyphicon glyphicon-pencil"></span>
        Izena eta Abizena <span class="sinadura-data">Arrasate</span></p>

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
