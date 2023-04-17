<template>
    <div class="s5">
        <div class="ctnr">
            <div class="hc">
                <h4><i>Refer</i></h4>
            </div>
            <div class="ho">
                <h2>How it works</h2>
            </div>
            <div class="pic">
                <img style="width: 100%; margin: 0%;" src="../assets/imgs/s5.png" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecFive'
}
</script>

<style scoped>
.s5 {
    background-color: #FFFFFF;
    padding: 10px;
    margin-left: 8%;
    margin-right: 8%;
    margin-top: 10%;
}

.ctnr {
    text-align: left;
}
.hc h4 {
    color: #01CB63;
    text-align: left;
    margin-bottom: 0%;
}

.ho h2 {
    color: #1F2532;
    text-transform: capitalize;
    opacity: 1;
    text-align: left;
    width: 35%;
    margin-top: 1.5%;
}

@media only screen and (max-width: 600px)
{
    .ho h2 {
    width: 50%;
}
}
@media only screen and (max-width: 525px)
{
    .ho h2 {
    width: 100%;
}
}


</style>