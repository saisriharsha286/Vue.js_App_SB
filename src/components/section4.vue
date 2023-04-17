<template>
    <div class="s4">
        <div class="container">
            <div class="hc">
                <h4><i>Top Earners</i></h4>
            </div>
            <div class="ho">
                <h2>Transforming your ideas into reality</h2>
            </div>
            <div class="names-list">
                <div v-for="name in names" :key="name.id" class="names-card">
                    <div class="names-image">
                        <img v-bind:src="name.image" alt="">
                    </div>
                    <div class="names-details">
                        <div><img src="../assets/imgs/rec.png" alt=""></div>
                        <div class="names-title">{{ name.title }}</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'SecFour',
    data() {
        return {
            names: [
                {
                    id: 1,
                    title: "₹8,00,000",
                    image: require("@/assets/imgs/luis.png")
                },
                {
                    id: 2,
                    title: "₹6,00,000",
                    image: require("@/assets/imgs/craig.png")
                },
                {
                    id: 3,
                    title: "₹5,00,000",
                    image: require("@/assets/imgs/christopher.png")
                },
                {
                    id: 4,
                    title: "₹4,50,000",
                    image: require("@/assets/imgs/jonas.png")
                }
            ]
        };
    }
};
</script>
  
<style scoped>
.s4 {
    background-color: #FFFFFF;
    padding: 10px;
    margin-left: 8%;
    margin-right: 8%;
    margin-top: 10%;
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

.names-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    grid-gap: 20px;
    margin-top: 4%;

}

.names-card {
    background-color: #fff;
    border-radius: 5px;
    overflow: hidden;
    box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.names-image img {
    width: 100%;
    height: auto;
}

.names-details {
    padding: 0px;
    display: flex;
    vertical-align: middle;
}

.names-title {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 10px;
    text-align: left;
    padding-top: 6%;
    padding-left: 5%;

}

@media only screen and (max-width: 525px) {
    .ho h2 {
        width: 100%;
    }

    .names-list {
        margin-left: 15%;
        margin-right: 15%;
        margin-top: 10%;

    }
}
</style>  