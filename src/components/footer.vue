<template>
    <div class="footer">
        <b-row id="back" >
            <b-col >
            <b-row id="first">
                <div class="bottom-left">เลขทะเบียนแนะนำ</div>
                </b-row>
            <b-row id="second">
                <div class="sub1">เลขทะเบียนมงคล</div>
            </b-row>
            <b-row id="third">
                    <div class="sub2"> ที่รอให้ท่านได้จับจองเป็นเจ้าของ</div>
                </b-row>
            </b-col>

            <b-col >
                <b-row class="slidetabien">
                    <b-col style="display:flex;height:0em">
                        <Tabien></Tabien>
                    </b-col>
                </b-row>
                     <b-row class="secondcoltext">
                        <div class="secondtext1"> ระดับความมงคล  : <span class="grade">A+</span></div>
                </b-row>
                  <b-row class="secondcoltext" >
                        <div class="secondtext2"> ระดับความแท้  : <span class="grade">A+</span></div>
                </b-row>
            </b-col>
        </b-row>

    </div>
</template>

<script>
import Tabien from './tabien'
import Vue from 'vue'
Vue.component('Tabien')
export default {
    name:'footer',
    components:{
        Tabien
    }
}
</script>
<style scoped>
#back{
    background-image :url('../assets/tbm_ui_under.png');
     background-repeat:no-repeat;
   background-size:contain;
  height: -webkit-fill-available;
}
#first{
height: 7em;
    padding-left: 5em;
    padding-top: 2em;

}
#second{
    padding-top: 2em;
    height: 4em;
    padding-left: 5em;
}
#third{
    padding-top: 2em;
    height: 4em;
    padding-left: 5em;
}

.bottom-left {

    font-size: 4vw;
    color :white;
    font-weight :700
}
.sub1 {
    font-size: 2vw;
    color :white;

}
.sub2 {

    font-size: 2vw;
    color :white;
}
.secondcol{
    display: flex;
    justify-content: center;
}
.slidetabien{
    padding-top: 5em;
        height: 30%;
    position: relative;

}
.level1{
position: relative;
    align-content: center;
}
.level2{
position: relative;
    align-content: center;
}
.secondcoltext{
    justify-content: center;
        position: relative;

}
.secondtext1{
        font-size: 1.5vw;
    color :white;
    margin-left: 1em;
}
.secondtext2{
        font-size: 1.5vw;
    color :white;
}
.grade{
    color: rgb(68, 255, 68);
    font-size: 1.5vw;
}

</style>
