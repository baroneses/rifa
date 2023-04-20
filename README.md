# Como configurar o site com a roleta

* Adicionar o arquivo roletaScript.js dentro da pasta `/assets/js`
* Adicionar o arquivo roleta.css e formulario.css dentro da pasta `/assets/css`


* Inserir o seguinte codigo dentro das tags < head >
```
<!-- FORMULARIO CSS FORMULARIO CSS FORMULARIO CSS -->
    <link rel="stylesheet" type="text/css" href="./assets/css/formulario.css"/>
    <link rel="stylesheet" type="text/css" href="./assets/css/roleta.css">
<!-- FORMULARIO CSS FORMULARIO CSS FORMULARIO CSS -->
```
* Inserir o seguinte codigo abaixo das tags < body> ou junto dos outros scripts no HTML
```
<!-- FORMULARIO SCRIPT FORMULARIO SCRIPT FORMULARIO SCRIPT -->
    <script src="./assets/js/jquery.js"></script>
    <script src="./assets/js/roletaScript.js"></script>
<!-- FORMULARIO SCRIPT FORMULARIO SCRIPT FORMULARIO SCRIPT -->
```
* Inserir a imagem da roleta dentro da pasta `/assets/images/roleta` com os nomes roleta001.png e seta2.png
* Inserir o seguinte código HTML logo abaixo do </ header>

```
<!-- FORMULARIO ROLETA -->
    <div class="spin-wrapper container">
        <p>
            <b style="color: red; font-size: 30px"> AVISO! </b><br>Apenas para os visitantes do nosso site, o o remedio aqui da prostata será vendido com desconto!
            Clique no botão para girar a roleta e
            garanta o seu desconto! Boa sorte!
        </p>
        <div class="wheel-wrapper">
            <div class="wheel">
                <img alt="" class="wheel-img b-lazy b-error" src="./assets/images/roleta/roleta001.png">
                <div class="wheel-cursor">
                    <img alt="" src="./assets/images/roleta/seta2.png" class="b-lazy b-error">
                    <span class="cursor-text"> GIRA!!</span>
                </div>
            </div>
        </div>
    </div>




    <div class="order-block" id="bottom_form" style="display: none">
        <img
                src="./assets/images/bottles/ps3.png"
                class="order-block-img not-lazy" />
        <div class="order-block-text">
            <div class="checkmark">
                <a class="link-rd link2" target="_blank">Experimente agora PROSTASLIM!</a>
            </div>

            <p>
                Últimos frascos disponíveis:
                <b>
                    <script type="text/javascript">
                        var options = {
                            weekday: "long",
                            year: "numeric",
                            month: "long",
                            day: "numeric",
                        };
                        var today = new Date();
                        document.write(today.toLocaleDateString("pt-BR", options));

                    </script>
                </b>
            </p>
            <p class="note">
                Garanta a sua <a target="_blank" class="link-rd link2">OFERTA EXCLUSIVA</a> e aproveite os 50% de
                desconto + frete grátis!

            </p>
            <section class="u-clearfix u-grey-10 u-section-3 show-on-call-action-form" >
                <div style="box-shadow: 1px 1px 7px 3px #d7d7d7"  class="u-clearfix u-grey-10 u-section-3 container">
                    <form id='form_id'>
                        <div class="row">
                            <h4 class="mb-4">Insira suas informações, <strong>FACA ALGO AGORA </strong> para ver o preço!</h4>
                            <div class="input-group input-group-icon">
                                <input id="user_name" type="text" placeholder="Nome completo"/>
                                <div class="input-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24px" height="24px" viewBox="0 0 24 24" version="1.1">
                                        <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                                            <polygon points="0 0 24 0 24 24 0 24"/>
                                            <path d="M12,11 C9.790861,11 8,9.209139 8,7 C8,4.790861 9.790861,3 12,3 C14.209139,3 16,4.790861 16,7 C16,9.209139 14.209139,11 12,11 Z" fill="#000000" fill-rule="nonzero" opacity="0.3"/>
                                            <path d="M3.00065168,20.1992055 C3.38825852,15.4265159 7.26191235,13 11.9833413,13 C16.7712164,13 20.7048837,15.2931929 20.9979143,20.2 C21.0095879,20.3954741 20.9979143,21 20.2466999,21 C16.541124,21 11.0347247,21 3.72750223,21 C3.47671215,21 2.97953825,20.45918 3.00065168,20.1992055 Z" fill="#000000" fill-rule="nonzero"/>
                                        </g>
                                    </svg>
                                </div>
                            </div>
                            <div class="input-group input-group-icon">
                                <input id="user_phone" onkeypress="mask(this, mphone);" onblur="mask(this, mphone);" type="text" placeholder="Telefone"/>
                                <div class="input-icon">
                                    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24px" height="24px" viewBox="0 0 24 24" version="1.1">
                                        <g stroke="none" stroke-width="1" fill="#0000" fill-rule="evenodd">
                                            <rect x="0" y="0" width="24" height="24"/>
                                            <path d="M7.13888889,4 L7.13888889,19 L16.8611111,19 L16.8611111,4 L7.13888889,4 Z M7.83333333,1 L16.1666667,1 C17.5729473,1 18.25,1.98121694 18.25,3.5 L18.25,20.5 C18.25,22.0187831 17.5729473,23 16.1666667,23 L7.83333333,23 C6.42705272,23 5.75,22.0187831 5.75,20.5 L5.75,3.5 C5.75,1.98121694 6.42705272,1 7.83333333,1 Z" fill="#000000" fill-rule="nonzero"/>
                                            <polygon fill="#0000" opacity="0.3" points="7 4 7 19 17 19 17 4"/>
                                            <circle fill="#0000" cx="12" cy="21" r="1"/>
                                        </g>
                                    </svg>
                                </div>
                            </div>

                        </div>
                        <div class="action">
                            <button type="submit" class="action-button">VER PREÇOS E OFERTAS</button>
                        </div>
                        <div class="footer_call mt-5">
                            <h6>Frete gratis para todo Brasil </h6>
                        </div>
                    </form>

                </div>
            </section>
        </div>
    </div>

    <div class="spin-result-wrapper" style="display: none">
        <div class="pop-up-window">
            <span class="pop-up-heading lt71">Parabéns!</span>
            <p class="ruletka-p pop-up-text lt72">
                Você ganhou 50% de desconto +<br />frete grátis na compra do seu ProstaSlim!
            </p>
            <a class="pop-up-button-roleta lt73"> OK</a>
        </div>
    </div>
    <!-- FORMULARIO ROLETA -->
```
* Trocar a classe da variavel `CLASS_TO_DISPLAY` no .html para ".spin-wrapper", da maneira abaixo
```
var CLASS_TO_DISPLAY = ".spin-wrapper";
```

# Como configurar o site com apena o formulário

* Adicionar o arquivo formularioOnlyScript.js dentro da pasta `/assets/js`
* Adicionar o arquivo formulario.css dentro da pasta `/assets/css`


* Inserir o seguinte codigo dentro das tags < head >
```
<!-- FORMULARIO CSS FORMULARIO CSS FORMULARIO CSS -->
    <link rel="stylesheet" type="text/css" href="./assets/css/formulario.css"/>
<!-- FORMULARIO CSS FORMULARIO CSS FORMULARIO CSS -->
```
* Inserir o seguinte codigo abaixo das tags < body> ou junto dos outros scripts no HTML
```
<!-- FORMULARIO SCRIPT FORMULARIO SCRIPT FORMULARIO SCRIPT -->
    <script src="./assets/js/formularioOnlyScript.js"></script>
<!-- FORMULARIO SCRIPT FORMULARIO SCRIPT FORMULARIO SCRIPT -->
```

* Inserir o seguinte código HTML logo abaixo do </ header>

```
    <!-- FORMULARIO FORMULARIO FORMULARIO -->
    <section class="u-clearfix u-grey-10 u-section-3 show-on-call-action-form" >
        <div class="header_call">
            <h4>SUA CHANCE ... LOREM IPSUM</h4>
        </div>
        <div  class="u-clearfix u-grey-10 u-section-3 container">
            <form id='form_id'>
                <div class="row">
                    <h4 class="mb-4">Insira suas informações, <strong>FACA ALGO AGORA </strong> para ver o preço!</h4>
                    <div class="input-group input-group-icon">
                        <input id="user_name" type="text" placeholder="Nome completo"/>
                        <div class="input-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24px" height="24px" viewBox="0 0 24 24" version="1.1">
                                <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                                    <polygon points="0 0 24 0 24 24 0 24"/>
                                    <path d="M12,11 C9.790861,11 8,9.209139 8,7 C8,4.790861 9.790861,3 12,3 C14.209139,3 16,4.790861 16,7 C16,9.209139 14.209139,11 12,11 Z" fill="#000000" fill-rule="nonzero" opacity="0.3"/>
                                    <path d="M3.00065168,20.1992055 C3.38825852,15.4265159 7.26191235,13 11.9833413,13 C16.7712164,13 20.7048837,15.2931929 20.9979143,20.2 C21.0095879,20.3954741 20.9979143,21 20.2466999,21 C16.541124,21 11.0347247,21 3.72750223,21 C3.47671215,21 2.97953825,20.45918 3.00065168,20.1992055 Z" fill="#000000" fill-rule="nonzero"/>
                                </g>
                            </svg>
                        </div>
                    </div>
                    <div class="input-group input-group-icon">
                        <input id="user_phone" onkeypress="mask(this, mphone);" onblur="mask(this, mphone);" type="text" placeholder="Telefone"/>
                        <div class="input-icon">
                            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="24px" height="24px" viewBox="0 0 24 24" version="1.1">
                                <g stroke="none" stroke-width="1" fill="#0000" fill-rule="evenodd">
                                    <rect x="0" y="0" width="24" height="24"/>
                                    <path d="M7.13888889,4 L7.13888889,19 L16.8611111,19 L16.8611111,4 L7.13888889,4 Z M7.83333333,1 L16.1666667,1 C17.5729473,1 18.25,1.98121694 18.25,3.5 L18.25,20.5 C18.25,22.0187831 17.5729473,23 16.1666667,23 L7.83333333,23 C6.42705272,23 5.75,22.0187831 5.75,20.5 L5.75,3.5 C5.75,1.98121694 6.42705272,1 7.83333333,1 Z" fill="#000000" fill-rule="nonzero"/>
                                    <polygon fill="#0000" opacity="0.3" points="7 4 7 19 17 19 17 4"/>
                                    <circle fill="#0000" cx="12" cy="21" r="1"/>
                                </g>
                            </svg>
                        </div>
                    </div>

                </div>
                <div class="action">
                    <button type="submit" class="action-button">VER PREÇOS E OFERTAS</button>
                </div>
                <div class="footer_call mt-5">
                    <h6>Frete gratis para todo Brasil </h6>
                </div>
            </form>

        </div>
        <div class="header_call">
            <h4>SUA CHANCE ... LOREM IPSUM</h4>
        </div>

    </section>
    <!-- FORMULARIO FORMULARIO FORMULARIO -->
```
