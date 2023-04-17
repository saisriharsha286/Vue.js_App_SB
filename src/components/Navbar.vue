<template>
    <nav class="navbar">
        <div class="navbar-container">
            <div class="navbar-brand">
                <router-link to="/" class="navbar-logo">
                    <img src="../assets/imgs/coursepro.png" alt="Logo" />
                </router-link>
            </div>
            <div class="navbar-toggle" :class="{ 'is-active': isNavOpen }" @click="isNavOpen = !isNavOpen">
                <span></span>
                <span></span>
                <span></span>
            </div>
            <div class="navbar-links" :class="{ 'is-active': isNavOpen }">
                <div class="navbar-buttons">
                    <router-link to="/login" class="navbar-buttonl">Login</router-link>
                    <router-link to="/register" class="navbar-buttonr">Register</router-link>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'NavBar',
    data() {
        return {
            isNavOpen: false,
        };
    },
};
</script>

<style scoped>
.navbar {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #fff;
    position: sticky;
    top: 0;
    z-index: 999;
    padding-left: 6%;
    padding-right: 4%;
}

.navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    max-width: 1200px;
    padding: 0 20px;
}

.navbar-brand {
    display: flex;
    align-items: center;
}

.navbar-logo {
    font-size: 2rem;
    color: #333;
    text-decoration: none;
}

.navbar-logo img {
    height: 40px;
    margin-right: 10px;
}

.navbar-toggle {
    display: none;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 21px;
    cursor: pointer;
}

.navbar-toggle span {
    display: block;
    width: 100%;
    height: 3px;
    background-color: #333;
    border-radius: 3px;
    transition: all 0.3s ease;
}

.navbar-toggle.is-active span:nth-child(2) {
    opacity: 0;
}

.navbar-links {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.navbar-links ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
}

.navbar-links li {
    margin: 0 10px;
}

.navbar-links a {
    font-size: 1.2rem;
    color: #333;
    text-decoration: none;
    transition: all 0.3s ease;
}

.navbar-links a:hover {
    color: #01CB63;
}

.navbar-buttons {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.navbar-buttonr {
    color: #FFFFFF;
    font-style: italic;
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
    transition: all 0.3s ease;
}
.navbar-buttonl
{
    background-color: #FFFFFF;
    margin-left: 10px;
    margin-right: 10px;
    margin-top: 0px;
    padding-left: 15px;
    padding-right: 15px;
    padding-top: 10px;
    padding-bottom: 10px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
    border-radius: 10px;
    border: 0px;
    letter-spacing: 0px;
    color: #1F2532;
    opacity: 1;
    cursor: pointer;
    transition: all 0.3s ease;

}
.navbar-buttonr:hover {
    background-color: #fff;
    color: #01CB63;
    border: 1px solid #01CB63;
}
.navbar-buttonl:hover {
    background-color: #fff;
    color: #01CB63;
    border: 1px solid #01CB63;
}

@media (max-width: 768px) {
    .navbar-brand {
        margin-right: auto;
    }

    .navbar-toggle {
        display: flex;
    }

    .navbar-links {
        display: none;
        position: absolute;
        top: 80px;
        left: 0;
        width: 100%;
        background-color: #fff;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
    }

    .navbar-links.is-active {
        display: flex;
        flex-direction: column;
    }

    .navbar-links ul {
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100%;
    }

    .navbar-links li {
        margin: 10px 0;
    }
}
</style>  