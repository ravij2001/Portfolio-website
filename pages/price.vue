<template>
<main>
    <div class="col opacity:0 bg-gray-700 text-white mx-5 my-5">
        <ul>
            <li class="text-4xl">{{basic}}</li>
            <li class="text-4xl">{{rupee}}</li>
            <li>5gb storage ram</li>
            <li>20GB Monthly Bandwidth</li>
            <li>Basic</li>
            <li>My SQL Databases</li>
            <li>10 Free Domain Names</li>
            <br>
            <button class="btn text-white"><strong>Purchase</strong></button>
        </ul>
    </div>
</main>
</template>
<script>
export default {
    props: {
            basic: {
                  type: String,
                default: "",
    },
           rupee: {
                  type: String,
                default: "",
    },
   },
};
</script>
<style scoped>
.col{
    /* border: 2px solid red; */
    text-align: center;
    width: 97.3%;
    height: 550px;
    border-radius: 10px;
    padding: 18px;
}
li{
    padding: 15px;
    /* border-bottom: 1px solid white; */
}
.btn {
  border: 2px solid red;
  border-radius: 25px;
  width: 50%;
  padding: 15px;
}
#a{
  background-color: red;
}

.btn:hover {
  background-color: red;
}
</style>