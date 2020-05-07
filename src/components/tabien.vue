<template>
<div class="containtabien">

<carousel-3d>

<!-- v-for -->
 <slide v-for="(data,index) in tabiendata" v-bind:key="index" :index='index'>
     <img class="image" src="../assets/tbm_tabien .png" alt="" />
<h2 class="uprow">
<span class="num" >{{data.No}}</span>
</h2>
<div class="word1">
        <div >ระดับความมงคล : <span class="grade">{{data.grade1}}</span></div>
        </div>
    <div class="word2">
        <div >ระดับความแท้ : <span class="grade">{{data.grade2}}</span></div>
    </div>
  </slide>

</carousel-3d>



</div>

</template>

<script>
import Vue from 'vue';
import Carousel3d from 'vue-carousel-3d';

Vue.use(Carousel3d);
export default {
    name:'tabien',
    data(){
        return{
         tabiendata:[{
            No:'กก 1234',
            grade1:'A+',
            grade2:'A+'
        },{
            No:'กข 7777',
            grade1:'A+',
            grade2:'ฺB+'
        },{
            No:'ทม 8888',
            grade1:'A+',
            grade2:'C+'
        },{
            No:'นน 8899',
            grade1:'A+',
            grade2:'C+'
        },{
            No:'พพ 0108',
            grade1:'A+',
            grade2:'C+'
        },{
            No:'พพ 0108',
            grade1:'A+',
            grade2:'C+'
        },{
            No:'พพ 0108',
            grade1:'A+',
            grade2:'C+'
        },{
            No:'พพ 0108',
            grade1:'A+',
            grade2:'C+'
        },
        ]}

    },

}
</script>
<style  scoped>
.containtabien{
        width: 50em;
        display: contents;
}
 .tabien{
height: 10em;
     background-image: url('../assets/tbm_tabien .png');
     background-repeat:no-repeat;
   background-size:contain;
   /* width: 20em */
   width: 50%
 }

 .rownum{
     height: 2em;
    padding-top: 0.5em;
    padding-left: 2vw;
    font-size: 2vw;
    color :white
 }

 .word1{
   position: absolute;
    top: 34%;
    left: 22%;
    width: 50%;
    color: white;
    font-size: 1vw;
 }
 .word2{
   position: absolute;
    top: 42%;
    left: 22%;
    width: 50%;
    color: white;
    font-size: 1vw;
 }
 .num{
     font-size: 2vw
 }
 /* .underdetail{
     padding-top: 1em;
 } */
 .image{
position: absolute;
width: 100%;
}
.uprow{
position: absolute;
top: 14%;
left: 22%;
width: 50%;
color: white;
}
.carousel-3d-slide{
    background: transparent;
    border: transparent;
}
/* .carousel-3d-container{
    max-height: 220px;
} */
.grade{
    color: rgb(68, 255, 68);
    font-size: 1vw;
}
</style>