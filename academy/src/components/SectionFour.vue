<script>
import CardThree from "./CardThree.vue"

 export default {
        data() {
            return {
                cardArr: [{
                    icon: "public/img/news-3-2.jpg",
                    category:"Admin University",
                    title: "Peer pressure changes how teens tackle inequality",
                    description: "____",
                    readmore: "Read more >",
                },
                {
                    icon: "public/img/news-2-2.jpg",
                    category:"Admin Education",
                    title: "Lewisham Live Mixtape celebrates borough's",
                    description: "____",
                    readmore: "Read more >",
                },
                {
                    icon: "public/img/news-1-2.jpg",
                    category:"Admin Education",
                    title: "Turner Prize winnner's work to open Gold on Film festival",
                    description: "____",
                    readmore: "Read more >",
                },
            ]
            };
        },
        components: {
            CardThree,
        }
    }</script>

<template>
<section>
    <h1>Latest From Our Blogs</h1>
    <p>Wheter you're a foundation course or an undergraduate degree master's <hr> or a PhD, academics is a place where students thrive.</p>

   

        <div class="container">
            <CardThree class="card" v-for="card in cardArr"
            :key="card.key"
            :icon="card.icon"
            :category="card.category"
            :title="card.title"
            :description="card.description"
            :readmore="card.readmore"
            />
        </div>
</section>

</template>
<style scoped>
section{
    text-align: center;
    font-size: 25px;
    

}

hr {
  height: 1px;
  margin: 0;
  border: none;
  background-color: transparent;
}

img{
    width: 356px;
}

ul li{
    list-style:none;
}

.container{
    margin-top: 4rem;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    
    
    
}

.card{
    background-color:whitesmoke;
    padding: 2rem;
    margin:3rem;
    width: 300px;
    height: 460px;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    align-items: center;
    justify-content: center;
}

.readmore{
    margin-right: 7rem;
}

.description{
    color: red;
    margin-right: 12rem;
}

.title{
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}


</style>