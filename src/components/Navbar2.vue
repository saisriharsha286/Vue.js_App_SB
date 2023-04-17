<template>
    <div class="header">
        <div class="nav">
            <img class="image" src="../assets/imgs/coursepro.png" alt="cplogo">
        </div>
        <button class="login">
            <div>Login</div>
        </button>
        <button class="register">
            <div>Register</div>
        </button>
    </div>
</template>
  
<script>
export default {
    name: 'NavBar',
    props: {
    }
}
</script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav {
    margin: 0px;
    width: 100%;
    text-align: left;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

.image {
    margin-top: 10px;
    margin-left: 10%;
}

.header {
    display: flex;
    position: fixed;
    background-color: #FFFFFF;

}

.login {
    background-color: #FFFFFF;
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 0px;
    padding-top: 0px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
    border: 0px;
    letter-spacing: 0px;
    color: #1F2532;
    opacity: 1;
    cursor: pointer;
}

.register {
    color: #FFFFFF;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
    margin: 15px;
    padding-left: 15px;
    padding-right: 15px;
    padding-top: 10px;
    padding-bottom: 10px;
    background: #01CB63 0% 0% no-repeat padding-box;
    box-shadow: 0px 5px 15px #01CB6359;
    border-radius: 10px;
    opacity: 1;
    border: 0px;
    border-color: #01CB6359;
    cursor: pointer;
    margin-right: 8%;
}
</style>
  