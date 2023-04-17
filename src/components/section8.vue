<template>
    <footer class="footer">
        <div class="footer-head">
            <div class="heading">
                <h5>Contact Us</h5>
            </div>
            <div class="sidehed">
                Reach Out with any question you have
            </div>
        </div>
        <div class="container">
            <div class="row">
                <div class="col-md-6">
                    <h3>Get in Touch</h3>
                    <p>Fill out the form below and we'll get back to you as soon as possible.</p>
                    <form @submit.prevent="submitForm">
                        <div class="form-group">
                            <label for="name">Name</label>
                            <input type="text" id="name" v-model="name" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <input type="email" id="email" v-model="email" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="number">Phone</label>
                            <input type="number" id="number" v-model="number" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <input type="text" id="text" v-model="subject" class="form-control" required>
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" v-model="message" class="form-control" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary">Submit</button>
                    </form>
                </div>
                <div class="col-md-6">
                    <h3>Contact Us</h3>
                    <p>123 Main St.<br>Anytown, USA 12345</p>
                    <p>Email: info@example.com<br>Phone: 555-1234</p>
                </div>
            </div>
            <div class="row">
                <div class="col-md-12">
                    <hr>
                    <p>&copy; 2023 MyWebsite. All rights reserved.</p>
                </div>
            </div>
        </div>
    </footer>
</template>
  
<script>
export default {
    name: 'SecEight',
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
            // handle form submission here
            console.log(this.name, this.email, this.number, this.subject, this.message);
            // reset form fields
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
.sidehed {
    text-align: center;
    font: normal normal bold 40px/54px;
    letter-spacing: 0px;
    color: #1F2532;
    text-transform: capitalize;
    opacity: 1;
}

.footer {
    background-color: #f8f8f8;
    padding: 60px 0;
    margin-top: 50px;
}

.form-control {
    height: 40px;
    border-radius: 0;
}

.btn-primary {
    border-radius: 0;
}

hr {
    border: none;
    border-top: 1px solid #ccc;
    margin-top: 30px;
    margin-bottom: 30px;
}
</style>
  