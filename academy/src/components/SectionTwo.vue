<script>
 export default {
        data() {
            return {
                cardTwo: [{
                    icon:"public/img/bruce-mars-FWVMhUa_wbY-unsplash.jpg",
                    price: "Free",
                    title: "UI Animation using Sketch 3, Principle App, and Flinto",
                    description: "This online photography course will teach you how to take amazing images and even sell..",
                    courseby: "Course by: University"
                },
                {
                    icon: "public/img/course-1-2.jpg",
                    price: "Free",
                    title: "The Ultimate Drawing Course - Beginner to Advanced ",
                    description: "This online photography course will teach you how to take amazing images and even sell..",
                    courseby: "Course by: University"
                },
                {
                    icon: "public/img/william-thomas-ny6tO4ItOEY-unsplash.jpg",
                    price: "Free",
                    title: "Your Complete Guide to Photography",
                    description: "This online photography course will teach you how to take amazing images and even sell..",
                    courseby: "Course by: University"
                },
            ]
            };
        },
    }
</script>

<template>
    <section>
    <h1>Recent Courses</h1>
    <p>Wheter you're considering a foundation course or an undergraduate degree master's <hr> or a PhD, academics is a place where students thrive</p>
</section>

<ul>
    <div class="container">
            <li class="card" v-for="card in cardTwo">
                <div class="icon"><img :src="card.icon" alt=""></div>
                <div class="price">{{ card.price }}</div>
                <div class="title">{{ card.title }}</div>
                <div>{{ card.description }}</div>
                <div class="red">{{ card.courseby }}</div>
            </li>
        </div>
        </ul>
</template>


<style scoped>
 section{
    text-align: center;
    font-size: 30px;
 }
 hr {
  height: 1px;
  margin: 0;
  border: none;
  background-color: transparent;
}

img{
   width: 300px;
   height: auto;
}

.price{
    background-image: url("../assets/img/counter-shape-2-1-1.png");
    background-repeat: no-repeat;
    font-weight: bold;
    margin-right: 16.5rem;
    
}

.title{
    font-weight: bold;
}

.red{
    color: red;
    margin-right: 8.9rem;
    
}

ul li{
    list-style: none;
}

.container{
    margin-top: 6rem;
    display: flex;
    justify-content: center;
    align-items: center;
}

.card{
    background-color: whitesmoke;
    padding: 2rem;
    margin:3rem;
    width: 300px;
    height: 400px;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    align-items: center;
    justify-content: center;


}
</style>