<script>

    export default {
        data() {
            return {
                cardOne: [{
                    icon:"public/svg/svg-0.svg",
                    title: "Online Coaching",
                    description: "Lorem ipsum is simply dummy text to printing and typesetting has been the industrys",
                },
                {
                    icon: "public/svg/svg-1.svg",
                    title: "Consultation",
                    description: "Lorem ipsum is simply dummy text to printing and typesetting has been the industrys",
                },
                {
                    icon: "public/svg/svg-2.svg",
                    title: "Life Programs",
                    description: "Lorem ipsum is simply dummy text to printing and typesetting has been the industrys",
                },
            ]
            };
        },
    }

</script>

<template>

    <section>
        <h1>
            Since 2000, weve been partnering with education leaders to <hr> <span class="red">increase equity and achievements</span> for all students.
        </h1>


        <ul class="none">
            <li v-for="card in cardOne">
                
                <div class="icon"><img :src="card.icon" alt=""></div>
                <div class="title">{{ card.title }}</div>
                <div class="description">{{ card.description }}</div>
            
            </li>
        </ul>

        <div class="flex">

        <div class="numbers">
            <span class="orangebg">6500</span><span class="orange">+</span><span>Students</span>
        </div>
        <div class="numbers">
            <span class="redbg">200</span><span class="red">+</span><span>Online Courses</span>
        </div>
        <div class="numbers">
            <span class="greenbg">100</span><span class="green">%</span><span>Happy Clients</span>
        </div>
    </div>
    </section>
    
</template>

<style scoped>
hr {
  height: 1px;
  margin: 0;
  border: none;
  background-color: transparent;
}

h1{
    text-align: center;
    font-size: 30px;
}

.red{
    color: red;
}

.flex{
    display: flex;
     justify-content: center;
     align-items: center;
}

.numbers{
    font-size: 40px;
    margin: 3rem;
   
}

.orangebg{
    background-image: url("../assets/img/counter-shape-1-1-1.png");
    color: orange;
    margin-right: .5rem;
    
}

.orange{
    color: orange;
    margin-right: .5rem;
}

.redbg{
    background-image: url("../assets/img/counter-shape-2-1-1.png");
    color: red;
    margin-right: .5rem;
    
}

.red{
    color: red;
    margin-right: .5rem;
}

.greenbg{
    background-image: url("../assets/img/counter-shape-3-1-1.png");
    color: green;
    margin-right: .5rem;
    
}

.green{
    color: green;
    margin-right: .5rem;
}

.icon{
    width: 70px;
}

.title{
    font-size: 25px;
   
}

ul li{
    list-style: none;
}



</style>