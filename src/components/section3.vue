<template>
    <div class="s3">
        <div class="container">
            <div class="hc">
                <h4><i>Courses</i></h4>
            </div>
            <div class="ho">
                <h2>Our Most Popular Courses</h2>
            </div>
            <div class="courses-list">
                <div v-for="course in courses" :key="course.id" class="course-card">
                    <div class="course-image">
                        <img v-bind:src="course.image" alt="Course Image">
                    </div>
                    <div class="course-details">
                        <div class="course-title">{{ course.title }}</div>
                        <div class="course-students"><b>{{ course.students }}</b> <i>Students</i></div>
                        <div class="course-box">
                            <div class="c-b">
                                <div><img src="../assets/imgs/time.png" alt=""></div>
                                <div class="course-time">{{ course.time }}</div>
                            </div>
                            <div class="c-b">
                                <div><img src="../assets/imgs/date.png" alt=""></div>
                                <div class="course-lectures">{{ course.lectures }} Lectures</div>
                            </div>
                        </div>
                        <div class="course-box">
                            <div class="c-b">
                                <div><img src="../assets/imgs/octac.png" alt=""></div>
                                <div class="course-instructor">{{ course.instructor }}</div>
                            </div>
                            <div class="c-b">
                                <div class="course-price">{{ course.price }} <span
                                        style="text-decoration: line-through; color: black; font-size: 14px; font-weight: 400;">
                                        {{ course.price }}</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'SecTre',
    data() {
        return {
            courses: [
                {
                    id: 1,
                    title: "Ultimate Business Intelligence Analyst A to Z Course 2021",
                    students: 46995,
                    time: "11 hr 20 mins",
                    lectures: 44,
                    instructor: "Albert Hitler",
                    price: "₹2000",
                    image: require("@/assets/imgs/c1.png")
                },
                {
                    id: 2,
                    title: "Adobe Photoshop Training: From Beginner to Pro",
                    students: 6995,
                    time: "6 hr 20 mins",
                    lectures: 24,
                    instructor: "Wanda Willson",
                    price: "₹3000",
                    image: require("@/assets/imgs/c2.png")
                },
                {
                    id: 3,
                    title: "Social Media Marketing - A to Z Content Marketing class 2021",
                    students: 46995,
                    time: "11 hr 20 mins",
                    lectures: 44,
                    instructor: "Albert Hitler",
                    price: "₹2000",
                    image: require("@/assets/imgs/c3.png")
                }
            ]
        };
    }
};
</script>
  
<style scoped>
.s3 {
    background-color: #FFFFFF;
    padding: 10px;
    margin-left: 8%;
    margin-right: 8%;
}

.hc h4 {
    color: #01CB63;
    margin-bottom: 0%;

}

.ho h2 {
    color: #1F2532;
    text-transform: capitalize;
    margin-top: 1.5%;
}

.courses-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    grid-gap: 20px;
    margin-top: 4%;
}

.course-card {
    background-color: #fff;
    border-radius: 5px;
    overflow: hidden;
    box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.course-card:hover {
    transform: translateY(-5px);
}

.course-image img {
    width: 100%;
    height: auto;
}

.course-details {
    padding: 20px;
}

.course-title {
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 10px;
    text-align: left;
}

.course-instructor {
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    color: #1F2532;
    margin-bottom: 10px;
    padding-top: 6%;
}

.course-time {
    font-size: 15px;
    color: #1F2532;
    margin-bottom: 10px;
    padding-top: 5%
}

.course-lectures {
    font-size: 15px;
    color: #1F2532;
    margin-bottom: 10px;
    padding-top: 5%
}

.course-box {
    display: flex;
    justify-content: space-between;
    margin-top: 10%;
    font-style: italic;
}

.c-b {
    display: flex;
}

.course-students {
    font-size: 15px;
    color: #1F2532;
    margin-bottom: 10px;
    text-align: left;
    margin-top: 8%;

}

.course-price {
    font-size: 22px;
    font-weight: bold;
    color: #01CB63;
    margin-bottom: 10px;
    padding-top: 6%;

}

@media only screen and (max-width: 525px) {
    .ho h2 {
        width: 100%;
    }

    .courses-list {
        margin-left: 10%;
        margin-right: 10%;
        margin-top: 10%;
    }
}

@media only screen and (max-width: 450px) {

    .courses-list {
        margin-left: 0%;
        margin-right: 0%;
        margin-top: 10%;
    }
}
</style>  