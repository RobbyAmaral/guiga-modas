<template>
    <div class="container-product-card">
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
        <div class="card-product">
            <img class="product-pic" src="~/assets/images/blusao.jpg" width="100%" height="300">
            <div class="product-info">
                <p class="description">Blusão 100% lã</p>
                <div class="price">
                    <div class="forward-price">Em até 6X <span class="focus-price">38,30</span></div>
                    <div class="spot-price">À vista <span class="focus-price">R$189,90</span></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: "ProductCard",
  components: {

  }
};
</script>

<style lang="scss" scoped>
.container-product-card {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    .card-product {
        margin: 3rem 0;
        width: 320px;
        height: 390px;
        border: 1px solid #E9E9E9;
        border-radius: 5px;
        box-shadow: 5px 5px 15px 0px rgba(0, 0, 0, 0.5);
        .product-pic {
            border-top-left-radius: 5px;
            border-top-right-radius: 5px;
        }
        .product-info {
            text-align: center;
            .description {
                font-size: 1.2rem;
                color: #e6207e;
            }
            .price {
                line-height: 1.4;
                .forward-price, .spot-price {
                    font-size: .875rem;
                    color: black;
                }
                .focus-price {
                    font-size: 1.2rem;
                    color: #e6207e;
                }
        } 
        }
    }   
}
</style>