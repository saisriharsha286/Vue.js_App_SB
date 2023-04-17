<template>
    <footer class="footer">
        <div class="footer-head">
            <div class="heading">
                <h4><i>Contact Us</i></h4>
            </div>
            <div class="sidehed">
                <h2>Reach Out with any question you have</h2>
            </div>
            <div class="footer-main">
                <div class="footer-left">
                    <div class="footer-smedia">
                        <div class="sm-head">
                            <h3>Contact Information</h3>
                        </div>
                        <div class="all-cinfos">
                            <div class="cinfo">
                                <div class="infoimg">
                                    <img src="../assets/imgs/gmail.jpg" alt="">
                                </div>
                                <div class="infoid">
                                    <a style="color: #2c3e50;" href="mailto:">
                                        <h4>contact@coursepro.com</h4>
                                    </a>
                                </div>
                            </div>
                            <div class="cinfo">
                                <div class="infoimg">
                                    <img src="../assets/imgs/phone.jpg" alt="">
                                </div>
                                <div class="infoid">
                                    <h4>1800-562-895, 1800-869-877</h4>
                                </div>
                            </div>
                            <div class="cinfo">
                                <div class="infoimg">
                                    <img src="../assets/imgs/add.jpg" alt="">
                                </div>
                                <div class="infoid">
                                    <h4>102 Street, India</h4>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="footer-smedia">
                        <div class="sm-head">
                            <h3>Social Media Channel</h3>
                        </div>
                        <div class="smimgs">
                            <div class="smicon">
                                <a href="http://" target="_blank" rel="noopener noreferrer"><img
                                        src="../assets/imgs/Facebook.png" alt="Facebook Icon"></a>
                            </div>
                            <div class="smicon">
                                <a href="http://" target="_blank" rel="noopener noreferrer"><img
                                        src="../assets/imgs/Twitter.png" alt="Twitter icon"></a>
                            </div>
                            <div class="smicon">
                                <a href="http://" target="_blank" rel="noopener noreferrer"><img
                                        src="../assets/imgs/Github.png" alt="Github icon"></a>
                            </div>
                            <div class="smicon">
                                <a href="http://" target="_blank" rel="noopener noreferrer"><img
                                        src="../assets/imgs/Linkedin.png" alt="Linkedin icon"></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="footer-right">
                    <div class="fr-head">
                        <h3>Fill up the form and our team will get back to you within 24 hours</h3>
                    </div>
                    <div class="fr-form">
                        <form @submit.prevent="submitForm">
                            <div class="fr-top">
                                <div class="form-groupl">
                                    <input placeholder="Name"
                                        style="border: 0px; background-color: #fff; border-bottom: 2px solid #01CB63;"
                                        type="text" id="name" v-model="name" class="form-control" required>
                                </div>
                                <div class="form-groupr">
                                    <input placeholder="Email"
                                        style="border: 0px; background-color: #fff; border-bottom: 2px solid #01CB63;"
                                        type="email" id="email" v-model="email" class="form-control" required>
                                </div>
                            </div>
                            <div class="fr-bottom">
                                <div class="form-groupl">
                                    <input placeholder="Phone"
                                        style="border: 0px; background-color: #fff; border-bottom: 2px solid #01CB63;"
                                        type="number" id="number" v-model="number" class="form-control" required>
                                </div>
                                <div class="form-groupr">
                                    <input placeholder="Subject"
                                        style="border: 0px;background-color: #fff; border-bottom: 2px solid #01CB63;"
                                        type="text" id="text" v-model="subject" class="form-control" required>
                                </div>
                            </div>
                            <div class="form-group">
                                <textarea placeholder="Message"
                                    style="height: 150px; width: 100%; border: 2px solid #01CB63;border-radius: 2px;opacity: 1;"
                                    id="message" v-model="message" class="form-control" required></textarea>
                            </div>
                            <button
                                style="background: #000000 0% 0% no-repeat padding-box; border-radius: 10px; opacity: 1; color: #fff; padding-top: 2%; padding-bottom: 2%; padding-left: 4%; padding-right: 4%; font-style: italic;"
                                type="submit" class="btn btn-primary">Submit</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>

        <div class="footer-end">
            <div class="fe-left">
                {{ new Date().getFullYear() }} &copy; Course Pro Private Limited
            </div>
            <div class="fe-right">
                <div class="ferl">Term & Condition <span style="padding-left: 20px;"> </span> Privacy Policy</div>
            </div>
        </div>

    </footer>
</template>

<script>
export default {
    name: 'FooTer',
    data() {
        return {
            name: '',
            email: '',
            number: '',
            subject: '',
            message: ''
        }
    },
    methods: {
        submitForm() {
            console.log(this.name, this.email, this.number, this.subject, this.message);
            this.name = '';
            this.email = '';
            this.number = '';
            this.subject = '';
            this.message = '';
        }
    }
}
</script>

<style scoped>
.footer {
    margin-left: 8%;
    margin-right: 8%;
}

.heading h4 {
    color: #01CB63;
    margin-bottom: 0%;
}

.sidehed h2 {
    text-align: center;
    color: #1F2532;
    text-transform: capitalize;
    opacity: 1;
}

.footer-main {
    display: flex;
    margin-top: 10%;
}

.footer-left {
    width: 40%;
    float: left;
    display: flex;
    flex-direction: column;
    margin-right: 10%;
}

.footer-smedia {
    display: flex;
    flex-direction: column;
    float: left;
}

.footer-smedia h3 {
    float: left;
    margin-left: 20%;
}

.sm-head {
    margin-left: -20%;
    margin-bottom: 5%;
}

.all-cinfos {
    margin-left: -20%;
    margin-top: 10%;
}

.cinfo {
    display: flex;
    margin-left: 18%;
    margin-bottom: 5%;
}

.infoimg img {
    vertical-align: middle;
    padding-top: 8%;
}

.infoid h4 {
    float: right;
}

.smimgs {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

.smicon img {
    width: 60%;
}

.footer-right {
    margin-left: 2%;
}

.fr-form {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-top: 10%;
}

.fr-top {
    display: flex;
    margin-bottom: 10%;
    margin-top: 2%;
}

.form-groupl {
    background-color: #fff;
    margin-right: 2%;
}

.form-groupr {
    background-color: #fff;
    margin-left: auto;
}

.fr-bottom {
    display: flex;
    margin-bottom: 8%;
}

.form-group {
    background-color: #fff;
    margin-bottom: 10%;
}

.footer-end {
    margin-left: -5%;
    margin-right: -5%;
    margin-top: 15%;
    margin-bottom: 3%;
    display: flex;
    justify-content: space-between;
    font-weight: 700;
}

.fe-left {
    text-align: left;
    font-size: 16px;
}

.fe-right {
    display: flex;
    font-size: 15px;
}

textarea:focus,
input:focus {
    outline: none;
}

input[type=number]::-webkit-inner-spin-button,
input[type=number]::-webkit-outer-spin-button {
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    margin: 0;
}


@media only screen and (max-width: 900px) {
    .footer-main {
        display: flex;
        flex-direction: column;
        margin-top: 10%;
    }

    .footer-left {
        width: 100%;
    }

    .footer-smedia h3 {
        float: none;
        margin-left: 20%;
    }

    .footer-smedia {
        float: none;
        justify-content: center;
        align-content: center;
    }

    .all-cinfos {
        align-content: center;
        margin-top: -5%;
        margin-bottom: 5%;
    }

    .cinfo {
        margin-left: 40%;
        margin-bottom: 0%;
    }

    .footer-right {
        margin-top: 15%;
    }

}

@media only screen and (max-width: 600px) {
    .footer-main {
        display: flex;
        flex-direction: column;
        margin-top: 10%;
    }

    .fr-top {
        display: flex;
        flex-direction: column;
        margin-bottom: 0%;
    }

    .fr-bottom {
        display: flex;
        flex-direction: column;
        margin-bottom: 10%;
    }

    .form-groupl {
        background-color: #fff;
        margin-bottom: 10%;
        width: 100%;
    }

    .form-groupr {
        background-color: #fff;
        margin-bottom: 10%;
        width: 100%;
    }

    .cinfo {
        margin-left: 30%;
        margin-bottom: 0%;
    }

}

@media only screen and (max-width: 500px) {
    .cinfo {
        margin-left: 20%;
        margin-bottom: 0%;
    }
}
</style>