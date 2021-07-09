<template>

    <div class="card">
        <img src="/assets/logo/logo.png" alt="Denim Jeans" style="width:100%">
        <h1 class="text-sm">{{ title }}</h1>
        <p class="price">{{ price }}</p>
        <p>Some text about the jeans..</p>
        <p>
            <button>Add to Cart</button>
        </p>
    </div>


</template>

<script>
export default {
    name: "ArticlesTinker",
    props: {
        title: String,
        brand: String,
        user_pseudo: String,
        nb_photo: Number,
        price: Number,
    }

}
</script>

<style lang="scss" scoped>

.card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    max-width: 300px;
    height: 400px;
    margin: auto;
    text-align: center;
    font-family: arial;

}

.price {
    color: grey;
    font-size: 22px;
}

.card button {
    border: none;
    outline: 0;
    padding: 12px;
    color: white;
    background-color: #000;
    text-align: center;
    cursor: pointer;
    width: 100%;
    font-size: 18px;
}

.card button:hover {
    opacity: 0.7;
}


</style>
