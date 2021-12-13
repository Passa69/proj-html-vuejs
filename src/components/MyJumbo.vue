<template>
    <div id="jumbo_comp"> 
        <div id="jumbo_text">
            <h1 class="jumbo_elem">Complete your dreams in JavaS Programming</h1>

            <p class="jumbo_elem">Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestiae corporis similique, sapiente ipsum assumenda, doloremque a possimus in porro eius ipsam cum iusto, rerum quam at nemo dolore minus. Impedit.</p>

            <button class="jumbo_elem">Download free E-book</button>
        </div>

        <img src="@/assets/home-5-hero-image.png" alt="">
    </div>
</template>

<script>
export default {
  name: 'MyJumbo',

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#jumbo_comp {
    display: flex;
    flex-direction: row;
    padding: 50px;

    #jumbo_text {
        margin-top: 100px;
        margin-right: 20px;
        text-align: left;

        .jumbo_elem {
            margin: 30px 0;
        }
    }
}

h1 {
    font-size: 50px;
    color: #3f3a64;
}

p {
    font-size: 20px;
    color: #928fa5;
}

button {
    font-size: 15px;
    padding: 15px 40px;
    background-color: #20ad96;
    color: white;
    border: 1px solid #20ad96;
    border-radius: 5px;
}
</style>