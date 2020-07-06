<template>
    <div>
        <div class="container" style="padding:10%">
            <h2>Contact Me</h2>
            <br>
            <input type="text" value="john.gill.cb@gmail.com" id="my_email">
            
               
        </div>
    </div>
</template>
<script lang="ts">
export default {
    data(){
        return {
            contact:{
                email:'',
                message:''
            }
        }
    },

}

</script>


<style lang="css" scoped>
    div{
        font-family: Roboto;
    }
</style>