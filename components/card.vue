<template>
        <div class="row1">
                            <h5 class="card-title text-center" style="font-size: 26px;">{{btnText}}</h5>
                            <br />
                            <p class="card-text">{{pText}}
                            </p>
                        </div>
</template>
<script>

export default{
    props: {
        btnText:{
            type:String,
            default:""
        },
        pText:{
            type:String,
            default:""
        },
    },
};
</script>
<style scoped>
    
</style>