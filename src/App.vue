<template>
    <div>
        <div id="loading-screen" v-bind:loaded="loaded">
            <div id="loading" class="loading__container">
                <div class="loading__circle">
                    <div class="loading__circle__inside">
                    </div>
                    <div class="loading__rectangle1">
                    </div>
                    <div class="loading__rectangle2">
                    </div>
                    <div class="loading__shadow">
                    </div>
                </div>
                <div class="loading__weights__container">
                    <div class="loading__weights">
                        <div class="w1 wl">
                        </div>
                        <div class="w2">
                        </div>
                        <div class="w3">
                        </div>
                        <div class="w4">
                        </div>
                        <div class="w5">
                        </div>
                        <div class="w6">
                        </div>
                        <div class="w5">
                        </div>
                        <div class="w4">
                        </div>
                        <div class="w3">
                        </div>
                        <div class="w2">
                        </div>
                        <div class="w1 wr">
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div>
            <div id="top">
                <div id="header">
                    <div class="logo">
                        <div class="pz-logo">
                            PZ
                        </div>
                        <div class="pz-logo-caption">
                            Paweł Zych
                        </div>
                    </div>
                    <div class="header-title">
                        <div>
                            TRENER
                        </div>
                        <div>
                            PERSONALNY
                        </div>
                    </div>
                    <div class="header-place">
                        <svg class="icon-place" viewBox="0 0 20 20">
                            <path d="M10,1.375c-3.17,0-5.75,2.548-5.75,5.682c0,6.685,5.259,11.276,5.483,11.469c0.152,
                            0.132,0.382,0.132,0.534,0c0.224-0.193,5.481-4.784,5.483-11.469C15.75,3.923,13.171,1.375,10,
                            1.375 M10,17.653c-1.064-1.024-4.929-5.127-4.929-10.596c0-2.68,2.212-4.861,4.929-4.861s4.929,
                            2.181,4.929,4.861C14.927,12.518,11.063,16.627,10,17.653 M10,3.839c-1.815,0-3.286,1.47-3.286,
                            3.286s1.47,3.286,3.286,3.286s3.286-1.47,3.286-3.286S11.815,3.839,10,3.839 M10,9.589c-1.359,
                            0-2.464-1.105-2.464-2.464S8.641,4.661,10,4.661s2.464,1.105,2.464,2.464S11.359,9.589,10,
                            9.589"></path>
                        </svg>
                        Kalisz
                    </div>
                    <div id="hamburger">
                        <div></div>
                        <div></div>
                        <div></div>
                    </div>
                </div>
                <ul id="menu">
                    <li data-menuanchor="page1" class="active"><a href="#page1">Start</a></li>
                    <li data-menuanchor="page2"><a href="#page2">Treningi</a></li>
                    <li data-menuanchor="page3"><a href="#page3">Etapy</a></li>
                    <li data-menuanchor="page4"><a href="#page4">Opinie</a></li>
                    <li data-menuanchor="page5"><a href="#page5">Cennik</a></li>
                    <li data-menuanchor="page6"><a href="#page6">Kontakt</a></li>
                    <li>
                        <a href="http://www.facebook.com/trenerpersonalnykalisz" target="_blank" title="Facebook">
                            <svg class="icon-facebook" viewBox="0 0 512 512">
                                <path d="M211.9 197.4h-36.7v59.9h36.7V433.1h70.5V256.5h49.2l5.2-59.1h-54.4c0 0 0-22.1
                                0-33.7 0-13.9 2.8-19.5 16.3-19.5 10.9 0 38.2 0 38.2 0V82.9c0 0-40.2 0-48.8 0 -52.5
                                0-76.1 23.1-76.1 67.3C211.9 188.8 211.9 197.4 211.9 197.4z"></path>
                            </svg>
                        </a>
                    </li>
                </ul>
            </div>

            <full-page :options="options" @after-load="afterLoad" id="fullpage">
                <div class="section section-1">
                    <div class="section__content">
                        <div>
                            <img class="section__image section__image-left" src="./assets/zych1.jpg">
                        </div>
                        <div class="section__content__text">
                            <div class="section__header">Twój sukces to mój sukces!</div>
                            <p>
                                Sport i&nbsp;aktywność fizyczna to mój styl życia. Trenując siebie i&nbsp;innych
                                spełniam
                                swoje marzenia. Po latach wyrzeczeń i&nbsp;podróży związanych z&nbsp;karierą siatkarską
                                zamieszkałem na stałe w&nbsp;Kaliszu. Prowadzę treningi personalne wykorzystując wiedzę
                                zdobytą podczas studiów na Akademii Wychowania Fizycznego i&nbsp;Sportu w&nbsp;Gdańsku
                                oraz na Państwowej Wyższej Szkole Zawodowej w&nbsp;Kaliszu uzupełniając ją o&nbsp;szkolenia,
                                kursy oraz fachową literaturę. Korzystam również z&nbsp;bogatych doświadczeń, które
                                zyskałem jako zawodnik i&nbsp;trener wielu polskich zespołów siatkarskich.
                            </p>
                            <p>
                                Do każdego podopiecznego podchodzę indywidualnie, ponieważ każda osoba ma inne problemy
                                i&nbsp;nawyki, nad którymi razem pracujemy. Pomagam ludziom w&nbsp;realizacji ich celów
                                związanych z&nbsp;budowaniem masy mięśniowej, redukcją tkanki tłuszczowej i&nbsp;pozbyciem
                                się
                                wad postawy.
                            </p>
                            <p>
                                Zapewniam świetną atmosferę na treningach. Przyjdź i&nbsp;przekonaj się :)
                            </p>
                        </div>
                    </div>
                </div>
                <div class="section section-2">
                    <div class="section__header section__header-center">Dopasowuję treningi odpowiednio do Twoich
                        potrzeb
                    </div>
                    <div class="section__content">
                        <div class="section__content__text">
                            <div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-stationary-bike"></i>
                                    <div>Redukcja tkanki tłuszczowej</div>
                                </div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-dumbbell"></i>
                                    <div>Budowa tkanki mięśniowej</div>
                                </div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-treadmill"></i>
                                    <div>Trening motoryczny</div>
                                </div>
                            </div>
                            <div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-isotonic"></i>
                                    <div>Trening wytrzymałościowy</div>
                                </div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-kettlebell"></i>
                                    <div>Trening korekcyjny (wady postawy)</div>
                                </div>
                                <div class="section__content__element">
                                    <i class="iconflat icon-stopwatch"></i>
                                    <div>Przygotowanie do rożnego typu zawodów sportowych</div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="section section-3">
                    <div class="section__header section__header-center">Poprowadzę Cię do wymarzonej sylwetki i doskonałej
                        formy
                    </div>
                    <div class="section__content">
                        <div class="section__content__element">
                            <div class="section__content__element__header">
                                <div class="number" number="1">1</div>
                                <div>Plan żywieniowy</div>
                            </div>
                            <div>
                                Na tym etapie analizuję Twój tryb życia, a w szczególności sposób odżywiania.
                                Identyfikuję elementy mające negatywne skutki na Twój organizm i zastępuję je
                                odpowiednimi, dbając o prawidłowe zapotrzebowanie kaloryczne i wartości odżywcze.
                            </div>
                        </div>
                        <div class="section__content__element">
                            <div class="section__content__element__header">
                                <div class="number" number="2">2</div>
                                <div>Plan treningowy</div>
                            </div>
                            <div>
                                Biorąc pod uwagę Twoje możliwości czasowe układam odpowiedni rozkład treningów. W
                                zależności od celów, jakie chcesz osiągnąć dobieram odpowiednie metody treningowe,
                                pamiętając o stopniowaniu trudności i obciążeń.
                            </div>
                        </div>
                        <div class="section__content__element">
                            <div class="section__content__element__header">
                                <div class="number" number="3">3</div>
                                <div>Treningi</div>
                            </div>
                            <div>
                                Podczas treningów dbam o poprawne wykonywanie ćwiczeń i aktywnie motywuję Cię dopóki
                                założenia dnia nie zostaną zrealizowane. Analizuję Twoje postępy na bieżąco i w razie
                                potrzeby koryguję lub rozwijam Twój plan treningowy.
                            </div>
                        </div>
                    </div>
                </div>
                <div class="section section-4">
                    <div class="section__content">
                        <div class="section__header section__header-center">Moją wizytówką są zadowoleni klienci</div>
                        <div class="section__slider">
                            <div class="section__slider__button section__slider__button-left" v-on:click="moveSlider('left')"></div>
                            <div class="section__slider__content__box">
                                    <div class="section__slider__content">
                                        <div class="section__slider__content__quotes">
                                            <span></span>
                                            <span>
                                                &bdquo;
                                            </span>
                                        </div>
                                        <div class="section__slider__content__text">
                                            Treningi z Pawłem to zawsze świetna zabawa. Są ciężkie, ale on umie mnie odpowiednio
                                            zmotywować. Pierwsze efekty były widoczne bardzo szybko.
                                        </div>
                                        <div class="section__slider__content__quotes">
                                            &ldquo;
                                        </div>
                                    </div>
                                    <div class="section__slider__content">
                                        <div class="section__slider__content__quotes">
                                            <span></span>
                                            <span>
                                                &bdquo;
                                            </span>
                                        </div>
                                        <div class="section__slider__content__text">
                                            Obawiałam się treningu na siłowni ze względu na moją nadwagę. Jednak przy Pawle wszystkie moje kompleksy zniknęły. Jego podejście pozwala mi skupić się na treningu i wykonywać go z pełną satysfakcją.
                                        </div>
                                        <div class="section__slider__content__quotes">
                                            &ldquo;
                                        </div>
                                    </div>
                                    <div class="section__slider__content">
                                        <div class="section__slider__content__quotes">
                                            <span></span>
                                            <span>
                                                &bdquo;

                                            </span>
                                        </div>
                                        <div class="section__slider__content__text">
                                            Na treningu personalnym z Pawłem mogłem się poczuć jak profesjonalny sportowiec. Jego podejście i fachowość pomogły mi poprawić technikę wykonywania ćwiczeń, a co za tym idzie polepszyłem swoje wyniki.
                                        </div>
                                        <div class="section__slider__content__quotes">
                                            &ldquo;
                                        </div>
                                    </div>
                            </div>
                            <div class="section__slider__button section__slider__button-right" v-on:click="moveSlider('right')"></div>
                        </div>
                    </div>
                </div>
                <div class="section section-5">
                    <div class="section__header section__header-center">
                        Dostajesz ode mnie pierwszy trening za darmo
                    </div>
                    <div class="section__content">
                        <div>
                            <div class="section__second-header">
                                A jeśli zdecydujesz się na dalszą współpracę to:
                            </div>
                            <div class="flex-center section__content__box">
                                <div class="flex-center section__content__text">
                                    <div>
                                        <i class="iconflat icon-gym-station"></i>
                                    </div>
                                    <div>
                                        <div class="section__content__element">
                                            <div>1 trening personalny</div>
                                            <div>99,00 zł</div>
                                        </div>
                                        <div class="section__content__element">
                                            <div>5 treningów personalnych</div>
                                            <div>399,00 zł</div>
                                        </div>
                                        <div class="section__content__element">
                                            <div>10 treningów personalnych</div>
                                            <div>699,00 zł</div>
                                        </div>
                                    </div>
                                </div>
                                <div class="flex-center section__content__text">
                                    <div>
                                        <i class="iconflat icon-workout"></i>
                                    </div>
                                    <div>
                                        <div class="section__content__element">
                                            <div>Konsultacja żywieniowa</div>
                                            <div>49,00 zł</div>
                                        </div>
                                        <div class="section__content__element">
                                            <div>Ułożenie diety</div>
                                            <div>149,00 zł</div>
                                        </div>
                                        <div class="section__content__element">
                                            <div>Ułożenie planu treningowego</div>
                                            <div>149,00 zł</div>
                                        </div>
                                        <div class="section__content__element">
                                            <div>Ułożenie diety + planu treningowego</div>
                                            <div>249,00 zł</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="section section-6">
                    <div class="section__content">
                        <div class="flex-center">
                            <div class="section__content__box">
                                <div class="section__header">Czekam na wszystkie Twoje pytania</div>
                                <div class="section__content__box__elements">
                                    <div>
                                        <div class="section__content__element">
                                            <svg class="svg-icon" viewBox="0 0 20 20">
                                                <path d="M12.075,10.812c1.358-0.853,2.242-2.507,2.242-4.037c0-2.181-1.795-4.618-4.198-4.618S5.921,4.594,5.921,6.775c0,1.53,0.884,3.185,2.242,4.037c-3.222,0.865-5.6,3.807-5.6,7.298c0,0.23,0.189,0.42,0.42,0.42h14.273c0.23,0,0.42-0.189,0.42-0.42C17.676,14.619,15.297,11.677,12.075,10.812 M6.761,6.775c0-2.162,1.773-3.778,3.358-3.778s3.359,1.616,3.359,3.778c0,2.162-1.774,3.778-3.359,3.778S6.761,8.937,6.761,6.775 M3.415,17.69c0.218-3.51,3.142-6.297,6.704-6.297c3.562,0,6.486,2.787,6.705,6.297H3.415z"></path>
                                            </svg>
                                            <div>Paweł Zych</div>
                                        </div>
                                        <div class="section__content__element">
                                            <svg class="svg-icon" viewBox="0 0 20 20">
                                                <path d="M17.659,3.681H8.468c-0.211,0-0.383,0.172-0.383,0.383v2.681H2.341c-0.21,0-0.383,0.172-0.383,0.383v6.126c0,0.211,0.172,0.383,0.383,0.383h1.532v2.298c0,0.566,0.554,0.368,0.653,0.27l2.569-2.567h4.437c0.21,0,0.383-0.172,0.383-0.383v-2.681h1.013l2.546,2.567c0.242,0.249,0.652,0.065,0.652-0.27v-2.298h1.533c0.211,0,0.383-0.172,0.383-0.382V4.063C18.042,3.853,17.87,3.681,17.659,3.681 M11.148,12.87H6.937c-0.102,0-0.199,0.04-0.27,0.113l-2.028,2.025v-1.756c0-0.211-0.172-0.383-0.383-0.383H2.724V7.51h5.361v2.68c0,0.21,0.172,0.382,0.383,0.382h2.68V12.87z M17.276,9.807h-1.533c-0.211,0-0.383,0.172-0.383,0.383v1.755L13.356,9.92c-0.07-0.073-0.169-0.113-0.27-0.113H8.851v-5.36h8.425V9.807z"></path>
                                            </svg>
                                            <div>+48 515 123 834</div>
                                        </div>
                                        <div class="section__content__element">
                                            <svg class="svg-icon" viewBox="0 0 20 20">
                                                <path d="M8.749,9.934c0,0.247-0.202,0.449-0.449,0.449H4.257c-0.247,0-0.449-0.202-0.449-0.449S4.01,9.484,4.257,9.484H8.3C8.547,9.484,8.749,9.687,8.749,9.934 M7.402,12.627H4.257c-0.247,0-0.449,0.202-0.449,0.449s0.202,0.449,0.449,0.449h3.145c0.247,0,0.449-0.202,0.449-0.449S7.648,12.627,7.402,12.627 M8.3,6.339H4.257c-0.247,0-0.449,0.202-0.449,0.449c0,0.247,0.202,0.449,0.449,0.449H8.3c0.247,0,0.449-0.202,0.449-0.449C8.749,6.541,8.547,6.339,8.3,6.339 M18.631,4.543v10.78c0,0.248-0.202,0.45-0.449,0.45H2.011c-0.247,0-0.449-0.202-0.449-0.45V4.543c0-0.247,0.202-0.449,0.449-0.449h16.17C18.429,4.094,18.631,4.296,18.631,4.543 M17.732,4.993H2.46v9.882h15.272V4.993z M16.371,13.078c0,0.247-0.202,0.449-0.449,0.449H9.646c-0.247,0-0.449-0.202-0.449-0.449c0-1.479,0.883-2.747,2.162-3.299c-0.434-0.418-0.714-1.008-0.714-1.642c0-1.197,0.997-2.246,2.133-2.246s2.134,1.049,2.134,2.246c0,0.634-0.28,1.224-0.714,1.642C15.475,10.331,16.371,11.6,16.371,13.078M11.542,8.137c0,0.622,0.539,1.348,1.235,1.348s1.235-0.726,1.235-1.348c0-0.622-0.539-1.348-1.235-1.348S11.542,7.515,11.542,8.137 M15.435,12.629c-0.214-1.273-1.323-2.246-2.657-2.246s-2.431,0.973-2.644,2.246H15.435z"></path>
                                            </svg>
                                            <div>NIP 555-209-70-23</div>
                                        </div>
                                        <div class="section__content__element">
                                            <svg class="svg-icon" viewBox="0 0 20 20">
                                                <path d="M17.388,4.751H2.613c-0.213,0-0.389,0.175-0.389,0.389v9.72c0,0.216,0.175,0.389,0.389,0.389h14.775c0.214,0,0.389-0.173,0.389-0.389v-9.72C17.776,4.926,17.602,4.751,17.388,4.751 M16.448,5.53L10,11.984L3.552,5.53H16.448zM3.002,6.081l3.921,3.925l-3.921,3.925V6.081z M3.56,14.471l3.914-3.916l2.253,2.253c0.153,0.153,0.395,0.153,0.548,0l2.253-2.253l3.913,3.916H3.56z M16.999,13.931l-3.921-3.925l3.921-3.925V13.931z"></path>
                                            </svg>
                                            <div>kontakt@pawelzych.pl</div>
                                        </div>
                                    </div>
                                    <div>
                                        <div>
                                            <textarea placeholder="Twoje pytanie" maxlength="2500" class="form message" v-model="formMessage"></textarea>
                                        </div>
                                        <div>
                                            <input type="email" placeholder="Twój e-mail" maxlength="45" class="form mail" v-model="formMail" v-on:keyup.enter="sendMessage">
                                        </div>
                                        <div class="button-div">
                                            <div class="form-status">
                                                {{formStatus}}
                                                <div class="form-loader">
                                                        <div class="loading__weights">
                                                            <div class="w1 wl">
                                                            </div>
                                                            <div class="w2">
                                                            </div>
                                                            <div class="w3">
                                                            </div>
                                                            <div class="w4">
                                                            </div>
                                                            <div class="w5">
                                                            </div>
                                                            <div class="w6">
                                                            </div>
                                                            <div class="w5">
                                                            </div>
                                                            <div class="w4">
                                                            </div>
                                                            <div class="w3">
                                                            </div>
                                                            <div class="w2">
                                                            </div>
                                                            <div class="w1 wr">
                                                            </div>
                                                        </div>
                                                </div>
                                            </div>
                                            <input type="button" value="WYŚLIJ" class="form button" v-on:click="sendMessage">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div>
                                <img class="section__image section__image-right" src="./assets/zych2.jpg">
                            </div>
                        </div>
                    </div>
                </div>
            </full-page>
        </div>
    </div>
</template>

<script>
    import FullPage from './assets/FullPage.vue'
    import fullPageMixin from './assets/fullPageMixin'

    export default {
        name: 'app',
        mixins: [fullPageMixin],
        components: {
            FullPage
        },
        data() {
            return {
                loaded: false,
                options: {
                    afterLoad: this.afterLoad,
                    scrollBar: false,
                    menu: '#menu',
                    navigation: true,
                    anchors: ['page1', 'page2', 'page3', 'page4', 'page5', 'page6']
                },
                slides: [],
                activeSlideIndex: 0,
                disableSlider: false,
                formMessage: '',
                formMail: '',
                formStatus: '',
                formStatusColor: 'white'
            }
        },
        methods: {
            afterLoad() {
                setTimeout(() => {
                    this.loaded = true;
                    this.loaded = true;
                }, 2000);
                this.slides = document.querySelectorAll('.section__slider__content');
                this.slides[this.activeSlideIndex].style.left = '0';
                this.slides[this.activeSlideIndex].style.transitionDuration = '1000ms';
                this.slides[this.getSlideProperIndex(this.activeSlideIndex + 1)].style.left = '100%';
                this.slides[this.getSlideProperIndex(this.activeSlideIndex - 1)].style.left = '-100%';
            },

            toggleNavigation: function () {
                this.options.navigation = !this.options.navigation;
            },

            moveSlider: function (direction) {
                if (this.disableSlider === false) {
                    this.disableSlider = true;

                    if (direction === 'right') {
                        this.slides[this.activeSlideIndex].style.left = '-100%';
                        this.slides[this.getSlideProperIndex(this.activeSlideIndex + 1)].style.transitionDuration = '1000ms';
                        this.slides[this.getSlideProperIndex(this.activeSlideIndex + 1)].style.left = '0';

                        setTimeout(() => {
                            this.slides[this.activeSlideIndex].style.transitionDuration = '0ms';
                            this.activeSlideIndex = this.getSlideProperIndex(this.activeSlideIndex + 1);
                            this.slides[this.getSlideProperIndex(this.activeSlideIndex + 1)].style.left = '100%';
                            this.slides[this.getSlideProperIndex(this.activeSlideIndex - 1)].style.left = '-100%';
                            this.disableSlider = false;
                        }, 1000);
                    } else if (direction === 'left') {
                        this.slides[this.activeSlideIndex].style.left = '100%';
                        this.slides[this.getSlideProperIndex(this.activeSlideIndex - 1)].style.transitionDuration = '1000ms';
                        this.slides[this.getSlideProperIndex(this.activeSlideIndex - 1)].style.left = '0';

                        setTimeout(() => {
                            this.slides[this.activeSlideIndex].style.transitionDuration = '0ms';
                            this.activeSlideIndex = this.getSlideProperIndex(this.activeSlideIndex - 1);
                            this.slides[this.getSlideProperIndex(this.activeSlideIndex + 1)].style.left = '100%';
                            this.slides[this.getSlideProperIndex(this.activeSlideIndex - 1)].style.left = '-100%';
                            this.disableSlider = false;
                        }, 1000);
                    }
                }
            },

            getSlideProperIndex: function (index) {
                if (index < 0) {
                    return this.slides.length - 1;
                } else if (index >= this.slides.length) {
                    return 0;
                } else {
                    return index;
                }
            },

            sendMessage: function () {
                if (this.formMessage === '') {
                    this.formStatus = 'Nie wpisano wiadomości';
                } else if (this.formMail === '') {
                    this.formStatus = 'Nie podano adresu e-mail';
                } else if (!this.isEmailCorrect(this.formMail)) {
                    this.formStatus = 'Niepoprawny adres e-mail';
                } else {
                    this.formStatus = 'Wysyłanie wiadomości';
                    document.querySelector('.form-loader').style.visibility = 'visible';
                    setTimeout(() => {
                        const success = false;

                        if (success) {
                            this.formStatus = 'Wysłano pomyślnie';
                            this.formMessage = '';
                            this.formMail = '';
                        } else {
                            this.formStatus = 'Błąd - Spróbuj ponownie';
                        }

                        document.querySelector('.form-loader').style.visibility = 'hidden';
                    }, 3000);
                }
            },

            isEmailCorrect: function (address) {
                return true;
            }
        }
    }
</script>

<style type="text/css">
    @font-face {
        font-family: roboto;
        src: url(assets/fonts/Roboto-Regular.ttf);
    }

    @font-face {
        font-family: pz;
        src: url(assets/fonts/ftb.ttf);
    }

    @font-face {
        font-family: iconflat;
        src: url(assets/fonts/iconflat.ttf);
    }

    .iconflat {
        font-family: iconflat;
        font-style: normal;
    }

    .icon-dumbbell:before {
        content: "\f100";
        position: relative;
        top: 8px;
    }

    .icon-stationary-bike:before {
        content: "\f101";
        position: relative;
        top: 0px;
    }

    .icon-isotonic:before {
        content: "\f102";
        position: relative;
        top: 1px;
        left: 6px;
    }

    .icon-workout:before {
        content: "\f103";
        font-size: 40px;
        margin-right: 24px;
        position: relative;
        left: 4px;
    }

    .icon-stopwatch:before {
        content: "\f104";
        position: relative;
        top: 1px;
        left: 2px;
    }

    .icon-kettlebell:before {
        content: "\f105";
        position: relative;
        top: 1px;
        left: 4px;
    }

    .icon-sport-wear:before {
        content: "\f106";
    }

    .icon-chest-expander:before {
        content: "\f107";
    }

    .icon-treadmill:before {
        content: "\f108";
        position: relative;
        top: 3px;
    }

    .icon-gym-station:before {
        content: "\f109";
        font-size: 40px;
        margin-right: 24px;
    }

    .icon-kettlebell-1:before {
        content: "\f10a";
    }

    .icon-pulsometer:before {
        content: "\f10b";
    }

    a {
        text-decoration: none
    }

    * {
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box
    }

    body {
        font-family: roboto;
    }

    #top {
        position: fixed;
        top: 0;
        width: 100%;
        display: flex;
        justify-content: space-between;
        z-index: 100;
        padding: 10px 35px;
    }

    #header {
        width: 100%;
        color: #fff;
        display: flex;
        align-items: center;
    }

    .pz-logo {
        font-family: pz;
        font-size: 93px;
        padding: 0;
        line-height: 0.6;
    }

    .pz-logo-caption {
        text-align: center;
        font-size: 16px;
        letter-spacing: 3px;
        position: relative;
        right: 4px;
        text-transform: uppercase;
    }

    .header-title {
        font-size: 28px;
        font-weight: 800;
        margin: 0 28px;
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: space-between;
        line-height: 1;
        height: 100%;
        padding-top: 6px;
    }

    .header-place {
        display: flex;
        align-items: center;
        font-size: 22px;
    }

    .icon-place {
        width: 32px;
        color: #fff;
        fill: #fff;
    }

    #hamburger {
        display: none;
        flex-direction: column;
        justify-content: space-between;
        width: 34px;
        height: 34px;
        icon: pointer;
    }

    #hamburger > div {
        background-color: #ffffff;
        height: 20%;
        border-radius: 2px;
    }

    #menu {
        z-index: 70;
        -webkit-font-smoothing: antialiased;
        -moz-font-smoothing: antialiased;
        letter-spacing: 1px;
        font-size: 17px;
        display: flex;
        align-items: center;

        list-style: none;
        margin: 0;
        padding: 0;
    }

    #menu li {
        display: inline-block;
        margin: 10px 0;
        position: relative
    }

    #menu a {
        color: #fff;
        padding: 0 0.8em 1.1em 0.8em
    }

    #menu li.active a:after {
        content: '';
        margin: 0 0.8em 0 0.8em;
        height: 2px;
        background: #fff;
        display: block;
        position: absolute;
        bottom: -6px;
        left: 0;
        right: 0;
    }

    .icon-facebook {
        width: 32px;
        color: #fff;
        fill: #fff;
        border-color: #fff;
        border-width: 2px;
        border-style: solid;
        border-radius: 10px;
        position: relative;
        top: 3px;
    }

    .section {
        position: relative;
        background-size: cover;
        background-position: center center;
    }

    .section > div {
        padding-top: 70px;
    }

    #loading-screen {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #000000;
        margin: 0;
        position: fixed;
        top: 0;
        left: 0;
        height: 100%;
        width: 100%;
        z-index: 300;
        transition-property: opacity;
        transition-duration: 800ms;
        transition-timing-function: ease-in;
        opacity: 1;
    }

    #loading-screen[loaded] {
        opacity: 0;
        pointer-events: none;
    }

    .loading__container {
        height: 200px;
        width: 200px;
        background-color: #000000;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .loading__circle {
        width: 100%;
        height: 100%;
        background-color: #ffffff;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        animation-name: loading;
        animation-duration: 1s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
    }

    .loading__circle__inside {
        background-color: #000000;
        width: 90%;
        height: 90%;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .loading__rectangle1 {
        background-color: #000000;
        width: 60%;
        height: 50%;
        position: absolute;
        top: 0;
        left: 0;
    }

    .loading__rectangle2 {
        background-color: #000000;
        width: 100%;
        height: 10%;
        position: absolute;
        top: 0;
    }

    .loading__shadow {
        background: linear-gradient(to bottom, black, rgba(0, 0, 0, 0));
        width: 40%;
        height: 40%;
        position: absolute;
        top: 10%;
        right: 0;
    }

    .loading__weights__container {
        position: absolute;
        top: 0;
        width: 100%;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .loading__weights {
        width: 70%;
        height: 70%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .loading__weights > div {
        background-color: #ffffff;
        z-index: 1;
    }

    .loading__weights > .w1 {
        width: 5%;
        height: 6%;
    }

    .loading__weights > .w2 {
        width: 3%;
        height: 9%;
        border-radius: 1px;
    }

    .loading__weights > .w3 {
        width: 7%;
        height: 30%;
        border-radius: 3px;
    }

    .loading__weights > .w4 {
        width: 8%;
        height: 40%;
        border-radius: 3px;
    }

    .loading__weights > .w5 {
        width: 3%;
        height: 9%;
        border-radius: 1px;
    }

    .loading__weights > .w6 {
        width: 40%;
        height: 6%;
    }

    .loading__weights > .wl {
        border-top-left-radius: 2px;
        border-bottom-left-radius: 2px;
    }

    .loading__weights > .wr {
        border-top-right-radius: 2px;
        border-bottom-right-radius: 2px;
    }

    @keyframes loading {
        from {
            transform: rotate(0deg);
        }
        to {
            transform: rotate(360deg);
        }
    }

    .section-1 {
        background-image: url('assets/background3.jpg');
    }

    .section-2 {
        background-image: url('assets/background2.jpg');
    }

    .section-3 {
        background-image: url('assets/background1.jpg');
    }

    .section-4 {
        background-image: url('assets/background5.jpg');
    }

    .section-5 {
        background-image: url('assets/background0.jpg');
    }

    .section-6 {
        background-image: url('assets/background6.jpg');
    }

    #fp-nav {
        padding-top: 35px;
    }

    #fp-nav > ul > li > a > span {
        background-color: #a5a5a5;
    }

    .section__header {
        color: #ffffff;
        font-weight: 800;
        margin-bottom: 24px;
        text-align: center;
    }

    .section__content {
        display: flex;
        align-items: center;
        justify-content: center;
        color: #ffffff;
    }

    .section-1 .section__header {
        text-align: left;
        font-size: 45px;
    }

    .section-1 .section__content__text {
        width: 50%;
        font-size: 16px;
        text-align: justify;
    }

    .section-1 .section__content__text > p {
        margin: 15px 0;
    }

    .section-2 .section__header {
        font-size: 36px;
    }

    .section-2 .section__content {
        font-size: 19px;
        flex-direction: column;
        align-items: flex-start;
    }

    .section-2 .iconflat {
        font-size: 28px;
        margin-right: 16px;
    }

    .section-2 .section__content__text {
        margin: 24px auto;
        display: flex;
    }

    .section-2 .section__content__text > div:nth-child(1) {
        margin-right: 32px;
    }

    .section-2 .section__content__element {
        display: flex;
        align-items: center;
        height: 40px;
        margin-bottom: 10px;
    }

    .section-3 .section__header {
        font-size: 36px;
    }

    .section-3 .section__content__element {
        margin: 24px;
        font-size: 16px;
        width: 24%;
        align-self: flex-start;
    }

    .section-3 .section__content__element__header {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        font-size: 26px;
        margin-bottom: 12px;
    }

    .section-4 .section__content {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .section-4 .section__header {
        font-size: 36px;
    }

    .section-4 .section__slider__content__box {
        overflow: hidden;
        position: relative;
        width: 100%;
        height: 150px;
    }

    .section-4 .section__slider {
        width: 80%;
        color: #ffffff;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .section-4 .section__slider__button {
        width: 0;
        height: 0;
        border-top: 40px solid transparent;
        border-bottom: 40px solid transparent;
        cursor: pointer;
    }

    .section-4 .section__slider__button-left {
        border-right: 40px solid #ffffff;
    }

    .section-4 .section__slider__button-right {
        border-left: 40px solid #ffffff;
    }

    .section-4 .section__slider__content {
        display: flex;
        margin: 0 72px;
        position: absolute;
        left: 100%;
        width: calc(100% - 144px);
        transition-property: left;
        transition-duration: 0ms;
        transition-timing-function: ease-in-out;
    }

    .section-4 .section__slider__content__quotes {
        font-size: 100px;
        display: flex;
        flex-direction: column;
    }

    .section-4 .section__slider__content__text {
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: justify;
        padding: 24px;
        font-size: 20px;
    }

    .section-4 .section__slider__content__quotes > span:nth-child(1) {
        flex: 1;
    }

    .section-5 .section__header {
        font-size: 36px;
    }

    .section-5 .section__second-header {
        text-align: center;
        font-size: 21px;
        margin-bottom: 16px;
    }

    .section-5 .section__content__element {
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin: 6px;
    }

    .section-5 .section__content__element > div:nth-child(2) {
        padding-left: 16px;
    }

    .section-5 .section__content__box > div:nth-child(1) {
        margin-right: 48px;
    }

    .section-6 .section__header {
        font-size: 35px;
        margin-bottom: 42px;
    }

    .section-6 .section__content__box {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .section-6 .section__content__element {
        display: flex;
        align-items: center;
        margin: 0 16px 16px 0;
    }

    .section-6 .section__content__box__elements {
        display: flex;
        justify-content: space-between;
    }

    .section-6 .svg-icon {
        width: 30px;
        height: 30px;
        fill: #ffffff;
        margin-right: 16px;
    }

    .section-6 .form {
        border-radius: 6px;
        background-color: rgb(255,255,255,0.2);
        border: 0;
        color: #ffffff;
        padding: 8px;
        font-family: roboto;
    }

    .section-6 .message {
        width: 300px;
        height: 85px;
    }

    .section-6 .mail {
        width: 300px;
        margin-top: 4px;
    }

    .section-6 .button {
        padding: 8px 16px;
        cursor: pointer;
    }

    .section-6 .form-status {
        display: flex;
        align-items: center;
        justify-content: flex-start;
        font-size: 14px;
        padding-left: 8px;
    }

    .section-6 .loading__weights {
        width: 100%;
        height: 100%;

        animation-name: loading;
        animation-duration: 1s;
        animation-iteration-count: infinite;
        animation-timing-function: linear;
    }

    .section-6 .button-div {
        display: flex;
        justify-content: space-between;
        margin-top: 8px;
    }

    .section-6 .form-loader {
        visibility: hidden;

        position: relative;
        width: 30px;
        height: 30px;
        margin-left: 8px;

        display: flex;
        align-items: center;
        justify-content: center;

    }

    .number {
        width: 34px;
        height: 34px;
        color: #000000;
        background-color: #ffffff;
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-size: 30px;
        font-weight: 800;
        font-family: pz;
        margin-right: 12px;
    }

    .number[number="1"] {
        padding-left: 1px;
    }

    .number[number="2"] {
        padding-left: 1px;
    }

    .number[number="3"] {
        padding-left: 2px;
    }

    .section__image {
        max-height: 50vh;
        border-radius: 5px;
    }

    .section__image-right {
        margin-left: 48px;
    }

    .section__image-left {
        margin-right: 48px;
    }

    ::-webkit-input-placeholder { /* Chrome/Opera/Safari */
        color: #ffffff;
    }

    ::-moz-placeholder { /* Firefox 19+ */
        color: #ffffff;
    }

    :-ms-input-placeholder { /* IE 10+ */
        color: #ffffff;
    }

    :-moz-placeholder { /* Firefox 18- */
        color: #ffffff;
    }

    .flex-center {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    @media only screen and (max-width: 1100px) {
        #top {
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        #header {
            width: unset;
        }

        .section > div {
            padding-top: 140px;
        }

        .section-1 .section__header {
            font-size: 34px;
        }

        @media only screen and (max-width: 620px) {
            #menu {
                display: none;
            }

            #header {
                width: 100%;
                justify-content: space-between;
            }

            #hamburger {
                display: flex;
            }

            .header-place {
                display: none;
            }

            .header-title {
                margin: 0;
            }

            @media only screen and (max-width: 500px) {
                .pz-logo {
                    font-size: 60px;
                    text-align: center;
                }

                .pz-logo-caption {
                    font-size: 12px;
                    right: 0;
                }

                .header-title {
                    font-size: 20px;
                }

                @media only screen and (max-width: 400px) {
                    .pz-logo {
                        font-size: 50px;
                    }

                    .pz-logo-caption {
                        font-size: 10px;
                    }

                    .header-title {
                        font-size: 14px;
                    }

                    #hamburger {
                        width: 28px;
                        height: 28px;
                    }

                    #top {
                        padding: 8px 15px;
                    }
                }
            }
        }
    }
    @media only screen and (max-width: 1024px) {
        .section-1 .section__content__text > p {
            font-size: 15px;
        }

        @media only screen and (max-width: 940px) {
            .section-1 .section__content__text > p {
                margin: 6px 0;
                font-size: 14px;
            }

            .section-1 .section__header {
                margin-bottom: 8px;
                font-size: 30px;
            }

            .section-2 .section__header {
                font-size: 31px;
            }

            .section-3 .section__header {
                font-size: 28px;
            }

            .section-4 .section__header {
                font-size: 29px;
            }

            .section-5 .section__header {
                font-size: 30px;
            }

            .section-6 .section__header {
                font-size: 31px;
            }

            @media only screen and (max-width: 860px) {
                .section-1 .section__content__text > p {
                    font-size: 13px;
                }

                .section-1 .section__header {
                    font-size: 26px;
                    margin-bottom: 0;
                }

                .section-2 .section__header {
                    font-size: 23px;
                    margin-bottom: 0;
                }

                .section-2 .section__content {
                    font-size: 17px;
                }

                .section-2 .section__content__text {
                    flex-direction: column;
                }

                .section-2 .section__content__element {
                    margin-bottom: 5px;
                }

                .section-3 .section__header {
                    font-size: 22px;
                    margin-bottom: 0;
                }

                .section-3 .section__content__element {
                    width: 26%;
                }

                .section-3 .section__content__element__header {
                    font-size: 22px;
                }

                .section-4 .section__slider__content__text {
                    font-size: 19px;
                }

                .section-4 .section__slider__content {
                    width: calc(100% - 70px);
                    margin: 0 35px;
                }

                .section-4 .section__slider__content__box {
                    height: 160px;
                }

                .section-5 .section__content__box {
                    flex-direction: column;
                }

                .section-5 .section__content__box > div:nth-child(1) {
                    margin-right: 0;
                }

                .section-5 .section__content__text:nth-child(1) .section__content__element > div:nth-child(2) {
                    padding-left: 90px;
                }

                @media only screen and (max-width: 820px) {
                    .section-4 .section__slider {
                        width: 90%;
                    }

                    .section-4 .section__slider__content__text {
                        font-size: 18px;
                    }

                    .section-6 .section__image-right {
                        display: none;
                    }
                }
            }
        }
    }
</style>
