<template>
    <div class="s1b">
        <div class="matter">
            <div class="texth">
                <h1 style="margin: 1px;">Anytime, Anywhere </h1>
                <h1 style="margin: 1px;">Learn on your schedule </h1>
                <h1 style="margin: 1px;">From any device</h1>
            </div>
            <div class="para">
                <b>
                    <p><i>We Believe everyone has the capcity to be creative <span
                                style="color: aliceblue; font-style:normal ;">Course Pro</span> is a place where people
                            develop their own potential</i></p>
                </b>
            </div>
            <div>
                <button class="btn">Lets get started</button>
            </div>
        </div>
        <div class="image">
            <img class="rec25" alt="" src="../assets/imgs/rec25.png">
        </div>
    </div>
</template>

<script>
export default {
    name: 'SecOne'
}
</script>

<style scoped>
.s1b {
    background-color: #01CB63;
    display: flex;
    flex-direction: row;
}

.matter {
    margin: 0px;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 5%;
    padding-bottom: 5%;
    width: 60%;
}

.texth {
    color: aliceblue;
    margin: 0px;
    width: 70%;
    text-align: left;
    font-size: 130%;
}

.para {
    width: 70%;
    overflow-wrap: normal;
    text-align: left;
    font-size: medium;
    line-height: 160%;
}

.btn {
    text-align: left;
    margin-top: 5%;
    border: 0px;
    background-color: #000000;
    border-radius: 10px;
    opacity: 1;
    color: #FFFFFF;
    padding: 10px;
    width: 130px;
    text-align: center;
    cursor: pointer;
    font-style: italic;
    transition: background-color 0.3s ease;

}

.btn:hover {
    background-color: #444;
}

.rec25 {
    text-align: right;
    width: 100%;
    height: 100%;
}

@media only screen and (max-width: 780px) {
    h1 {
        font-size: 1.6em;
    }
}

@media only screen and (max-width: 675px) {
    h1 {
        font-size: 1.4em;
    }

    p {
        font-size: 0.8em;
    }
}

@media only screen and (max-width: 600px) {

    .s1b {
        background-color: #01cb6370;
    }

    .matter {
        background-image: url('../assets/imgs/rec25`.png');
        width: 100%;
    }

    .image {
        width: 0%;
    }
}
</style>