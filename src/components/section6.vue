<template>
    <div class="s6">
        <div class="sidehead">
            <h4><i>Testimonials</i></h4>
        </div>
        <div class="headdesc">
            <h2>Check out What Our Students Think About Us</h2>
        </div>
        <div class="cards">
            <div class="ind-card">
                <div class="card-desc">
                    <p>It's a comprehensive online learning platform for everyone looking to learn and course pro.
                        provinding this platform which is very beneficial for practicals. Students can revise everything at
                        home like dissection and slides</p>
                </div>
                <div class="card-footer">
                    <div class="cardf-left">
                        <div class="card-dp">
                            <img src="../assets/imgs/octac.png" alt="image_anshul">
                        </div>
                        <div class="carddp-desc">
                            <div class="card-name">
                                <h4 style="margin: 0%;">Anshul Jain</h4>
                            </div>
                            <div class="card-name-desc">
                                <p style="margin: 0%;">Yesterday</p>
                            </div>
                        </div>
                    </div>
                    <div class="cardf-right">
                        <div class="card-img">
                            <img src="../assets/imgs/rquote.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
            <div class="ind-card">
                <div class="card-desc">
                    <p>It's a comprehensive online learning platform for everyone looking to learn and course pro.
                        provinding this platform which is very beneficial for practicals. Students can revise everything at
                        home like dissection and slides</p>
                </div>
                <div class="card-footer">
                    <div class="cardf-left">
                        <div class="card-dp">
                            <img src="../assets/imgs/octac.png" alt="image_anshul">
                        </div>
                        <div class="carddp-desc">
                            <div class="card-name">
                                <h4 style="margin: 0%;">Rajkumar Jain</h4>
                            </div>
                            <div class="card-name-desc">
                                <p style="margin: 0%;">Yesterday</p>
                            </div>
                        </div>
                    </div>
                    <div class="cardf-right">
                        <div class="card-img">
                            <img src="../assets/imgs/rquote.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecSix'
}
</script>

<style scoped>
.s6 {
    margin-top: 5%;
    margin-left: 8%;
    margin-right: 8%;
    margin-bottom: 10%;
}

.sidehead {
    color: #01CB63;
    text-align: left;
    margin-bottom: 0%;
}

.headdesc {
    color: #1F2532;
    text-transform: capitalize;
    opacity: 1;
    text-align: left;
    width: 40%;
    margin-top: 1%;
}

.cards {
    display: flex;
    justify-content: space-evenly;
}

.ind-card {
    width: 40%;
    background: #FFFFFF 0% 0% no-repeat padding-box;
    box-shadow: 0px 20px 30px #1F25321A;
    border-radius: 15px;
    opacity: 1;
    padding: 2%;
    text-align: left;
    display: flex;
    flex-direction: column;
}

.card-desc {
    height: 70%;
    width: 85%;
    font-style: italic;
}

.card-footer {
    height: 30%;
    padding-bottom: 2%;
    margin-top: 5%;
    display: flex;
}

.cardf-left {
    display: flex;
    width: 85%;
    margin-top: 5%;
}

.card-dp img {
    padding-top: 5%;
    align-items: center;
}

.carddp-desc {
    margin-left: 2%;
    display: flex;
    flex-direction: column;
}

.card-name {
    font-size: small;
}

.cardf-right {
    float: right;
    margin-top: 5%;
}

.card-img {
    padding-top: 3%;
}

@media only screen and (max-width: 600px) {
    .headdesc {
        color: #1F2532;
        text-transform: capitalize;
        opacity: 1;
        text-align: left;
        width: 50%;
        margin-top: 1%;
    }

    .cards {
        display: flex;
        flex-direction: column;
        margin-top: -5%;
    }

    .ind-card {
        width: 100%;
        margin-top: 5%;
    }
}

@media only screen and (max-width: 525px) {
    .headdesc {
        width: 100%;
    }
}
</style>