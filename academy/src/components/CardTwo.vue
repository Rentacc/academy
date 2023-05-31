<script>
    export default{
        props:{
            icon: String,
            price: String,
            title: String,
            description: String,
            courseby: String
        }
    }
    
    
    </script>
    <template>
                <ul>
                    <li>
                    <div class="icon"><img :src="icon" alt=""></div>
                    </li>
                    <li>
                        <div class="price">{{ price }}</div>
                    </li>
                    
                    <li>
                        <div class="title">{{ title }}</div>
                    </li>
                    <li>
                        <div class="description">{{ description }}</div>
                    </li>
                    <li>
                        <div class="courseby">{{ courseby }}</div>
                    </li>
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