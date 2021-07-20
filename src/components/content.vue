<template>
    <div class="maincontent">
        
        <ul class="ul" id="ul">
            <img id="img"  v-bind:src="srcimg" alt="">
            <li><h5 >Name</h5></li>
            <li>{{name}}</li>
            <li><h5>Position</h5></li>
            <li>{{position}}</li>
            <li><h5 >Company</h5></li>
            <li>{{company}}</li>
            <li id="btnli"><button class="btn" v-on:click="shank">Shashank</button>
            <button class="btn" v-on:click="utk">Utkarsh</button>
            <button class="btn" v-on:click="pinky">Pinky</button></li>
        </ul>
    </div>
</template>
<script>

export default {
    
    name:"maincontent",
    data(){
        return{
            name:"",
            position:"",
            company:"",
            srcimg:"",
         
             
        }
    },
    methods:{
        shank:function(){
            this.name="Shashank Kulkarni",
            this.position="JavaScript Developer",
            this.company="HotWax Systems"
            this.srcimg="https://media-exp1.licdn.com/dms/image/C5603AQErCBWwuSx9_A/profile-displayphoto-shrink_800_800/0/1594899337905?e=1632355200&v=beta&t=w1YAp81sGhzzpGrvxb5qvWyP_5Y8C2cEQ3jMRP48lNQ"
            
        },
                utk:function(){
            this.name="Utkarsh Khedekar",
              this.position="Java Developer",
            this.company="Infosys"
            this.srcimg="https://media-exp1.licdn.com/dms/image/C4E03AQGVxWUMTqyOeQ/profile-displayphoto-shrink_800_800/0/1599810830159?e=1632355200&v=beta&t=DJUh9NDqVYznjdozJgshrW0v9dY79r1HKaFrKgvR-9A"

          
        },
                pinky:function(){
            this.name="Pinky Jagwani",
            this.position="customer service",
            this.company="HP"
            this.srcimg="https://media-exp1.licdn.com/dms/image/C4D03AQHxSSvcbmg6hw/profile-displayphoto-shrink_800_800/0/1618506381364?e=1632355200&v=beta&t=0goYTosuGjCW4m3cTNNYNo5L8G8sJ64oVGzfSkm0Bwo"
        }
    }
}
</script>
<style>
.maincontent{
}
.ul{
    list-style-type: none;
 
}
#btnli{
    margin-top: 30px;
}
.btn{
    margin-left: 10px;
    margin-right: 10px;
}
#img{

    border: 2px green solid;
    border-radius: 1000px;
    width: 150px;
    height: 150px;
}

</style>