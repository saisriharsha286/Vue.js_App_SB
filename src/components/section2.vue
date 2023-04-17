<template>
    <div class="s2">
        <div class="part">
            <div class="head">
                <p>Total Students</p>
            </div>
            <div class="body">
                <p class="num">5140</p>
            </div>
        </div>
        <div class="part">
            <div class="head">
                <p>Partners</p>
            </div>
            <div class="body">
                <p class="num">4123</p>
            </div>
        </div>
        <div class="part">
            <div class="head">
                <p>Affiliate Distribution</p>
            </div>
            <div class="body">
                <p class="num">4.18 Lac</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecTwo'
}
</script>

<style scoped>
.s2 {
    background-image: url(../assets/imgs/Group12141.png);
    display: flex;
    padding-top: 5%;
    padding-bottom: 5%;
    margin-bottom: 8%;


}

.part {
    width: 33%;
    font-weight: 600;
    color: #86919D;
    display: flex;
    flex-direction: column;
}

.head {
    font-size: large;
}

.body {
    text-decoration: underline;
    text-decoration-color: #01CB63;
    text-underline-offset: 5px;
}

.num {
    color: #1F2532;
    font-weight: 900;
    font-size: xx-large;
    margin: 0px;
    margin-left: 2%;

}

@media only screen and (max-width: 675px) {
    p {
        font-size: 0.8em;
    }

    .num {
        font-size: x-large;
    }
}

@media only screen and (max-width: 505px) {
    p {
        font-size: 0.6em;
    }

    .num {
        font-size: x-large;
    }
}
</style>