<template>
    <div>
        <div class="footer-container">
            <div class="footer-infos">
                <img class="guiga-banner" src="~assets/images/banner-guiga.png" alt="Guiga Modas logo" width=15% height=10%>
                <p class="store-name">GUIGA MODAS</p>
                <p>Rua Ramiro Barcelos, 841 - Próximo ao clube Sócrates</p>
                <p>São José do Norte, RS</p>
            </div>
            <p class="social-title">Acompanhe-nos nas redes sociais:</p>
            <div class="social">
                <a href="https://www.facebook.com/ingridguigamodas" target="_blank"><img src="~assets/images/icons/facebook-icon.png" alt="Ícone Facebook" width=35 height=35></a>
                <a href="http://m.me/ingridguigamodas" target="_blank"><img src="~assets/images/icons/messanger-icon.png" alt="Ícone Messanger" width=35 height=35></a>
                <a href="https://www.instagram.com/guigamodassjn/" target="_blank"><img src="~assets/images/icons/instagram-icon.png" alt="Ícone Instagram" width=35 height=35></a>
                <a href="https://api.whatsapp.com/send?phone=+555399550692&text=Oi%20Guiga,%20tudo%20bem?%20=)" target="_blank"><img src="~assets/images/icons/whatsapp-icon.png" alt="Ícone Whatsapp" width=35 height=35></a>
            </div>
        </div>
        <div class="developer">
            <p class="developed-by">Developed by: Robby Amaral</p>
            <img src="~assets/images/icons/linkedin-icon.png" alt="Developer Linkedin" width=18 height=18>
            <img src="~assets/images/icons/whatsapp-white-icon.png" alt="developer Whatsapp" width=18 height=18>
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
    padding: 2rem 0;
    text-align: center;
    font-size: 1.25rem;
    background-color: black;
    .footer-infos {
        p { padding-bottom: .5rem; }
        img { padding-bottom: 1rem; }
    }
    .social-title { padding: 1rem 0; }
    .social {
        display: flex;
        justify-content: center;
        img {
            padding: 0 .75rem;
        }
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
        .social {
            img {
                width: 25px;
                height: 25px;
            }
        }
    }
}
</style>