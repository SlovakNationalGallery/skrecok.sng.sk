<template>
  <div
    @mousemove="onActive"
    @mousedown="onActive"
    @scroll="onActive"
    @mousewheel="onActive"
    @touchstart="onActive"
  >
    <div id="top" class="bg-dots top-0"></div>
    <div class="bg-dots-fadedown top-1"></div>
    <img src="/img/skrecok-lamp.png" class="bg-image lamp" />

    <section class="container my-0 pt-5">
      <Button v-bind:text="backHome" v-bind:href="'/'"  class="mt-0 home-link mb-3" /><br/>
      <div class="mt-2">
        <h1
          class="my-5 bg-dark text-light tilted d-inline-block px-3 pt-2 pb-1"
        >
          Pablo Picasso
        </h1>

        <ArtistProfile
          class="mt-5"
          v-bind:kiosk="kiosk"
          v-bind:profile="{ 
            ...profile, 
            title: '', 
            profileText: `Svetoznámy maliar, sochár, keramikár i dizajnér, ktorý výrazne ovplyvnil umenie 20. storočia a zanechal po sebe obrovské dielo. Jeho unikátny umelecký talent sa prejavil už v detstve a ranej mladosti. Jeho otec bol učiteľom kreslenia, odmalička sa tak veľmi intenzívne venoval kresleniu a maľovaniu. Študoval na Akadémii umenia v Barcelone už ako 15-ročný. S prestávkami prežil celý život  vo Francúzsku.`
           }"
        />
      </div>
    </section>

    <section class="container">
      <div class="row">
        <div class="col-sm-12 col-lg-6 text-left">
          <h4 class="text-left">Diela a témy</h4>
          <p>
            Umelecký svet ovplyvnili začiatkom 20. storočia viaceré vedecko-technické objavy. Vytvorili sa podmienky pre revoltu a vznik nových <b>avantgardných umeleckých smerov</b>, ktoré sa rozchádzali so staršími tendenciami umenia konca 19. storočia. Umelci začali experimentovať vo výtvarnom výraze a zachytávať nové videnie skutočnosti novými výtvarnými prostriedkami. Avantgarda (predvoj) bola vzdorom umelcov voči spoločnosti. Charakterizujú ju aj kolektívne programové úsilia a umelecké manifesty jednotlivých smerov.  
          </p>
        </div>

        <div class="col-sm-12 col-lg-6">
          <img class="framed" src="/img/picasso/picasso_pariz.jpg" />
        </div>
      </div>        

      <div class="row">
        <div class="col-sm-12 col-lg-6 text-left">
          <p>
            Tvorba Pabla Picassa je veľmi rôznorodá a rozsiahla. Za namaľovaním legendárneho diela <i>Avignonské slečny</i> stojí mnoho úsilia, rozhovorov a skíc. Picasso sa tu pokúsil zaznamenať svoj traumatizujúci zážitok z nevestinca. Vyzývavý pohľad slečien má diváka zneistiť. Pred namaľovaním obrazu uchvátilo Picassa umenie vzdialených kultúr. Africké masky privezené z francúzskych kolónií a iberské sochy ho podnietili k rozmýšľaniu o novom spôsobe maľby objektov. 
          </p>
          <p>  
            Na reliéfoch obdivoval plochy a proporcie, ich zjednodušenie na geometrické tvary, ktoré sa stali základom nového umeleckého štýlu – <b>kubizmu</b>. Kubizmus radikálne spochybnil pravidlá zobrazovania, nielen z hľadiska perspektívy a zjednodušovania tvarov. Verejnosťou nebol prijatý s nadšením.    
          </p>
        </div>

        <div class="col-sm-12 col-lg-6">
            <img class="framed" src="/img/picasso/picasso_slecny.jpg" />
        </div>
      </div>
      
      <div class="row">
        <div class="col-sm-12 col-lg-6 text-left">
          <p>
            Obhajcovia kubizmu tvrdili, že prirodzené videnie je ochudobnené, lebo nevidíme predmet zo všetkých strán. Otvára sa tak nová <b>téma mnohoznačnosti znaku</b>. Picasso si napríklad tváre predstavoval ako znaky, ktoré si môže pri maľovaní vybrať zo širokého repertoáru, kombinovať ich a  vytvárať významy v závislosti od kontextu. Príkladom je jeho hravé zamieňanie znakov v kolážach alebo socha s názvom <i>Býčia hlava</i> (1942), v ktorej spojením cyklistických riadidiel a sedadla vytvoril metaforu – obraz býčej hlavy. 
          </p>
        </div>

        <div class="col-sm-12 col-lg-6">
          <img class="framed" src="/img/picasso/picasso_byk.jpg" />
        </div>
      </div>
    </section>

    <section class="container">
      <div class="row">
        <div class="col-sm-12 col-lg-10 offset-lg-1 no-margin">
          <img class="framed" src="/img/picasso/picasso_kubizmus.jpg" />
        </div>
      </div>
    </section>

    <section class="container">
      <div class="row">

        <div class="col-sm-12 col-lg-6 order-2 order-lg-1">
          <img class="framed" src="/img/picasso/picasso_diela.jpg" />
        </div>

        <div class="col-sm-12 col-lg-5 text-left order-1 order-lg-2">
          <h4>Námety na diskusiu</h4>
          <p class="with-circle">Ako ovplyvnil <b>technologický pokrok</b> v 19. storočí umelecký svet? Vynález fotoaparátu, film, farby v tubách, nové dopravné prostriedky a cestovanie, elektrifikácia, väčší prienik informácií zo sveta.</p> 
          <p>Nachádzate aj v Picassovej tvorbe vplyv technologického pokroku?</p> 
        </div>  
      </div>
      <div class="row">
        
        <div class="col-sm-12 col-lg-5 text-left">
          <p class="with-circle">U Picassa, ako aj v tvorbe ostatných avantgardných umelcov, <b>stráca opodstatnenie presné zachytenie podoby</b> človeka, krajiny a vecí.</p> 
          <p>Pozrite si aj ostatné jeho diela a popremýšľajte, čo všetko môže byť v jeho tvorbe hodnotné.</p> 
          <p>Spomeňte si a opíšte situáciu, kedy ste z vlastného rozhodnutia urobili niečo inak, ako sa od vás očakávalo a malo to pozitívny výsledok.</p>
        </div>

        <div class="col-sm-12 col-lg-6">
          <img class="framed" src="/img/picasso/picasso_traja.jpg" />
        </div>
      </div>

      <div class="row">

        <div class="col-sm-12 col-lg-6 order-2 order-lg-1">
          <img class="framed" src="/img/picasso/picasso_masky.png" />
        </div>

        <div class="col-sm-12 col-lg-5 text-left order-1 order-lg-2">
          <p class="with-circle">Preskúmajte <i>Avignonské slečny</i>. Je pravá strana namaľovaná rovnakým štýlom ako ľavá? Na ktorej strane vidno <b>inšpiráciu africkými maskami</b>?</p> 
          <p>Diskutujte o fenoméne kolonializmu, ktorý ako systém nadvlády a kontroly jedného štátu nad iným, nemal len ekonomické a politické motivácie, ale aj kultúrny rozmer.</p>
        </div>
      </div>

    </section>

    <section class="container">
      <div class="row">
        <div class="col-sm-12 col-lg-6 text-left">
          <h4>Aktivity</h4>
          <p class="with-circle">
            Narysujte na výkres rozloženú <b>sieť kocky</b> tak, aby sa dala zlepiť (napríklad vo veľkosti 5 x 5 cm, na okrajoch nechajte malé výbežky, aby sa kocka dala dobre skladať). Vyberte pre žiakov fotky predmetov, ktoré nepoznajú. Ich úlohou bude nakresliť na jednotlivé políčka predmet postupne z každej strany: zhora, zdola, z ľavej strany, z pravej strany, spredu a zozadu. Ak sa niektorý predmet nedá nakresliť zo všetkých strán, vyberte si viac predmetov.</p> 
          <p>Kocku si vystrihnite a zložte. Postavte spoločné zátišie, ktoré sa mení otáčaním strán.</p>	
		      </p>
        </div>
        <div class="col-sm-12 col-lg-6">
          <img class="framed" src="/img/picasso/picasso_kocka.jpg" />
        </div>
      </div>
    </section>

    <section class="container">
      <div class="row">
        <div class="col-sm-10 offset-sm-1  col-md-10 offset-md-1 col-lg-8 offset-lg-2">
          <h4>
            Externé odkazy
          </h4>
          <ul class="text-left">
						<li>
              <dl> 
                <dt>Pablo Picasso – Francov sen a lož:</dt><dd>
              <a v-bind:href="kiosk?null:'https://www.webumenia.sk/clanok/pablo-picasso-francov-sen'" target="_blank">
                https://www.webumenia.sk/clanok/pablo-picasso-francov-sen
              </a>
              </dd></dl>
            </li>
            <li>
              <dl> 
                <dt>Múzeum Pabla Picassa v Barcelone:</dt><dd>
              <a v-bind:href="kiosk?null:'http://www.museupicasso.bcn.cat'" target="_blank">
                http://www.museupicasso.bcn.cat/
              </a>
              </dd></dl>
            </li>
            <li>
              <dl> 
                <dt>Múzeum Pabla Picassa v Malage:</dt><dd>
              <a v-bind:href="kiosk?null:'https://www.museopicassomalaga.org'" target="_blank">
                https://www.museopicassomalaga.org/
              </a>
              </dd></dl>
            </li>
            <li>
              <dl> 
                <dt>Múzeum Pabla Picassa v Paríži:</dt><dd>
              <a v-bind:href="kiosk?null:'http://www.museepicassoparis.fr'" target="_blank">
                http://www.museepicassoparis.fr/
              </a>
              </dd></dl>
            </li>
            <li>
              <dl> 
                <dt>Ako porozumieť Picassovi? (video v anglickom jazyku):</dt><dd>
              <a v-bind:href="kiosk?null:'https://www.youtube.com/watch?v=_HGW1DQO1xQ'" target="_blank">
                https://www.youtube.com/watch?v=_HGW1DQO1xQ
              </a>
              </dd></dl>
            </li>
          </ul>
        </div>
      </div>
    </section>

    <div class="text-center">
      <a v-bind:href="kiosk?null:'../pdfs/Pablo_Picasso.pdf'"  class="pdf-link mt-5 mb-3">
        <img
          src="/img/news.png"
          class="d-inline-block"
        />
        <span>{{ downloadPdf }}</span>
      </a>
      <Button v-bind:text="backHome" v-bind:href="'/'"  class="mt-5" />
    </div>

    <footer class="container space">&nbsp;</footer>
    <div class="bg-dots-fadedown flip-vertical bottom-0"></div>
    
  </div>
</template> 

<script>
import index from "./index";
import ArtistProfile from "../components/ArtistProfile";
import BasicPage from "../components/BasicPage.vue";

export default {
  mixins: [BasicPage],
  components: {
    ArtistProfile
  },
  computed: {
    profile() {
      return { ...this.profiles["Pablo Picasso"] };
    }
  }
};
</script>