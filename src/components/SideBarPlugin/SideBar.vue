<template>
    <div id="side">
        {{title}}
    </div>
</template>


<style>
#side  { 
    background-color : #44475c;
    width : 80px;
    height : 100%;
    float : left;
    color : #fff;
    top : 0;
    bottom : 0;
    position: absolute;
    width: 15%;

 }

</style>

<script>
export default {
    name: "SideBar",
    props: {
        title : {
            type : String,
            default : "Stock Agence"
        }
    }

}


</script>