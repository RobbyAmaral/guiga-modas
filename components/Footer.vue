<template>
    <div>
        <div class="footer-container">
            <div class="footer-infos">
                <!-- <img class="guiga-banner" src="~assets/images/banner-guiga.png" alt="Guiga Modas logo" width=15% height=10%> -->
                <nuxt-link to="/"><img src="~assets/images/guiga-logo.png" alt="Guiga Modas logo" width=110 height=55></nuxt-link>
                <p class="store-name">GUIGA MODAS</p>
                <p>Rua Ramiro Barcelos, 841 - Próximo ao clube Sócrates</p>
                <p>São José do Norte, RS</p>
            </div>
            <p class="social-title">Acompanhe-nos nas redes sociais:</p>
            <div class="social">
                <a href="https://www.facebook.com/ingridguigamodas" target="_blank"><img src="~assets/images/icons/icon-facebook.png" alt="Ícone Facebook" width=35 height=35></a>
                <a href="http://m.me/ingridguigamodas" target="_blank"><img src="~assets/images/icons/messanger-icon.png" alt="Ícone Messanger" width=35 height=35></a>
                <a href="https://www.instagram.com/guigamodassjn/" target="_blank"><img src="~assets/images/icons/instagram-icon.png" alt="Ícone Instagram" width=35 height=35></a>
                <a href="https://api.whatsapp.com/send?phone=+555399550692&text=Oi%20Guiga,%20tudo%20bem?%20acabei%20de%20ver%20a%20sua%20loja%20online%20=)" target="_blank"><img src="~assets/images/icons/whatsapp-icon.png" alt="Ícone Whatsapp" width=35 height=35></a>
            </div>
            <div class="ways-to-pay">
                <p class="ways-to-pay-title">Formas de Pagamento</p>
                <p class="ways-to-pay-subtitle">em até 6 vezes nos cartões:</p>
                <ul class="ways-to-pay-cards">
                    <img src="~assets/images/icons/icon-visa.png" alt="Ícone Visa" width="35" height="30">
                    <img src="~assets/images/icons/icon-master.png" alt="Ícone Mastercard" width="35" height="30">
                    <img src="~assets/images/icons/icon-hiper.png" alt="Ícone Hipercard" width="35" height="30">
                    <img src="~assets/images/icons/icon-banri.png" alt="Ícone Banri Compras" width="35" height="30">
                    <img src="~assets/images/icons/icon-elo.png" alt="Ícone elo" width="35" height="30">
                    <img src="~assets/images/icons/icon-senff.png" alt="Ícone Senff" width="35" height="30">
                </ul>
            </div>
        </div>
        <div class="developer">
            <p class="developed-by">Developed by: Robby Amaral</p>
            <a href="https://www.linkedin.com/in/robby-amaral-388910139/" target="_blank"><img src="~assets/images/icons/linkedin-icon.png" alt="Developer Linkedin" width=18 height=18></a>
            <a href="https://api.whatsapp.com/send?phone=+5511972725601&text=Olá,%20vi%20o%20seu%20site!%20tem%20como%20me%20informar??%20=)" target="_blank"><img src="~assets/images/icons/whatsapp-white-icon.png" alt="developer Whatsapp" width=18 height=18></a>
        </div>
    </div>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
.footer-container {
    width: 100%;
    color: white;
    margin: 4rem 0 2rem 0;
    padding: 1.5rem 0 3rem 0;
    text-align: center;
    font-size: 1.25rem;
    background-color: black;
    .footer-infos, .ways-to-pay {
        p { padding-bottom: .5rem; }
        .store-name { padding-bottom: 1.5rem; }
    }
    .social-title, .ways-to-pay { padding: 1rem 0; }
    .social { padding-bottom: 1.5rem; }
    .social, .ways-to-pay-cards {
        display: flex;
        justify-content: center;
        img { padding: 0 .75rem; }
    }
    .ways-to-pay {
        color: black;
        background-color: white;
        img { padding: .5rem; }
    }
}
.developer {
    display: flex;
    color: black;
    font-size: 1rem;
    padding-bottom: 3rem;
    justify-content: center;
    .developed-by, img { padding-right: .5rem;}
}

@media (max-width: 525px) {
    .footer-container {
        font-size: 1rem;
        .guiga-banner {
            width: 30%;
            height: 20%;
        }
        .social, .ways-to-pay {
            img {
                width: 25px;
                height: 25px;
            }
        }
    }
}
</style>