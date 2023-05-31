<script>
    export default{
        props:{
            icon: String,
            category: String,
            title: String,
            description: String,
            readmore: String
        }
    }
    
    
    </script>
    <template>
                <ul>
                    <li>
                    <div class="icon"><img :src="icon" alt=""></div>
                    </li>
                    <li>
                        <div class="category">{{ category }}</div>
                    </li>
                    
                    <li>
                        <div class="title">{{ title }}</div>
                    </li>
                    <li>
                        <div class="description">{{ description }}</div>
                    </li>
                    <li>
                        <div class="readmore">{{ readmore }}</div>
                    </li>
                </ul>
    
    
    
    
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