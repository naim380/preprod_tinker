<template>
    <div class="home">
        <ArticlesTinker
        v-for="product in products"
        v-bind:user_pseudo="user_pseudo":user_pseudo="user_pseudo"
        v-bind:key="product.id":title="product.title"
        v-bind:brand="product.brand":brand="product.brand"
        v-bind:nb_photo="product.nb_photo":nb_photo="product.nb_photo"
        v-bind:price="product.price":price="product.price"
        ></ArticlesTinker>
    </div>
</template>
<script>
    import ArticlesTinker from "./subComponents/ArticlesTinker";
    export default {
        components: {ArticlesTinker},
        mounted() {
            console.log('Component mounted.')
        },
        data() {
            return {
                products: [
                    {
                        "id":6,
                        "title":"Tournevis",
                        "description":"Soft, knit sweater with a slightly wider neckline. Long sleeves and ribbing at neckline, cuffs, and hem.",
                        "price":"4.99",
                        "specific_price":"35,00",
                        "nb_photo":2,
                        "condition":"New",
                        "brand":"Bosh",
                        "sold":false,
                        "fav":12,
                        "viewed":23,
                        "user_id":7,
                        "user_pseudo":"steph_z2",
                        "user_star":4.5,
                        "user_review":"25",
                        "category_id":11,
                        "category_name":"Clothing"
                    },
                    {
                        "id":7,
                        "title":" Pelle",
                        "description":"lorem ipsum dolor sit amet",
                        "price":"88.30",
                        "specific_price":"185,43",
                        "nb_photo":3,
                        "condition":"New",
                        "brand":"Facom",
                        "sold":false,
                        "fav":78,
                        "viewed":75,
                        "user_id":6,
                        "user_pseudo":"rafael87",
                        "user_star":4,
                        "user_review":"150",
                        "category_id":24,
                        "category_name":"Shoes"
                    },
                    {
                        "id":4,
                        "title":"Scie à ruban",
                        "description":"lorem ipsum dolor sit amet",
                        "price":"138.00",
                        "nb_photo":2,
                        "condition":"New with tags",
                        "brand":"Stainless",
                        "sold":false,
                        "fav":15,
                        "viewed":123,
                        "user_id":12,
                        "user_pseudo":"adamyan",
                        "user_star":4,
                        "user_review":"52",
                        "category_id":13,
                        "category_name":"Bags"
                    },
                    {
                        "id":5,
                        "title":"Marteau",
                        "description":" Lace crop top, Zara",
                        "price":"29.00",
                        "nb_photo":1,
                        "condition":"New",
                        "brand":"Bosh",
                        "sold":false,
                        "fav":2,
                        "viewed":113,
                        "user_id":10,
                        "user_pseudo":"pink_dressing",
                        "user_star":5,
                        "user_review":"252",
                        "category_id":11,
                        "category_name":"Clothing"
                    },
                    {
                        "id":1,
                        "title":"Clé à cliquet",
                        "description":"lorem ipsum dolor sit amet",
                        "price":"12.10",
                        "nb_photo":1,
                        "size":"M",
                        "condition":"Very good",
                        "brand":"Facom",
                        "sold":false,
                        "fav":15,
                        "viewed":123,
                        "user_id":7,
                        "user_pseudo":"steph_z2",
                        "user_star":4.5,
                        "user_review":"25",
                        "category_id":26,
                        "category_name":"Suits & blazers"
                    },

                    {
                        "id":8,
                        "title":"Striped T-shirt",
                        "description":" Longline Striped T-Shirt With Curved Hem",
                        "price":"16.00",
                        "nb_photo":1,
                        "condition":"Very good",
                        "brand":"Bosh",
                        "sold":true,
                        "fav":8,
                        "viewed":233,
                        "user_id":2,
                        "user_pseudo":"lopito43",
                        "user_star":0,
                        "user_review":"0",
                        "category_id":21,
                        "category_name":"Tops & t-shirts"
                    },

                    {
                        "id":2,
                        "title":"Douille",
                        "description":" Lace crop top, Zara",
                        "price":"18.00",
                        "nb_photo":1,
                        "specific_price":"35,00",
                        "size":"L / 40 / 12",
                        "condition":"New with tags",
                        "brand":"Facom",
                        "sold":false,
                        "fav":32,
                        "viewed":153,
                        "user_id":10,
                        "user_pseudo":"pink_dressing",
                        "user_star":5,
                        "user_review":"252",
                        "category_id":11,
                        "category_name":"Clothing"
                    },

                    {
                        "id":3,
                        "title":"Clé dynamométrique",
                        "description":" High heel Cage Effect for Women Sandals Worn only once, very good condition Made in Italy",
                        "price":"120.00",
                        "nb_photo":2,
                        "condition":"Very good",
                        "brand":"Facom",
                        "sold":true,
                        "fav":8,
                        "viewed":233,
                        "user_id":5,
                        "user_pseudo":"maxmoux",
                        "user_star":3.5,
                        "user_review":"122",
                        "category_id":12,
                        "category_name":"Shoes"
                    }

                ]

            }
        }

    }
</script>

<style>
.home{
    display: flex;
    flex-wrap: wrap;
}
</style>
