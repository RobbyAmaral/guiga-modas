<template>
    <div class="container-master">
        <div class="header-section">
            <img src="~/assets/images/fashion.jpg" alt="Woman header" width="100%" height="450">
            <div class="page-section-title">
                <p class="title-section">Feminino</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.container-master {
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
}
.header-section {
    text-align: center;
    position: relative;
    .page-section-title {
        width: 100%;
        background-color: rgba(0,0,0,.6);;
        top: 70%;
        left: 50%;
        position: absolute;
        transform: translate(-50%, -50%);
        .title-section {
            padding: 8px;
            color: white;
            font-size: 2.5rem;
        }
    }
}

@media (max-width: 525px) {
    .header-section {
        img {
            height: auto;
            max-height: 250px;
        }
        .page-section-title{
            .title-section {
                font-size: 1.8rem;
            }
        }
    }
}
</style>