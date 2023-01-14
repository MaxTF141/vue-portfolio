<template>
    <section id="testimonials">
        <h5 class="display-5 text-success text-center py-4">TESTIMONIALS</h5>
        <div class="carousel mt-5 pt-5 mx-auto" id="carousel">
            <div id="carouselExampleDark" class="carousel carousel-dark slide mt-5" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div class="container-fluid">
                        <div class="carousel-item active" data-bs-interval="1000000"
                            v-for="testimonies in testimonialsActiveCarousel" :key="testimonies.id">
                            <div class="container-fluid text-center">
                                <div class="row justify-content-center">
                                    <div class="col-12 col-lg-6 my-3 d-flex justify-content-around g-3 pb-4">
                                        <div class="card" style="width: 30rem; height: fit-content;">
                                            <div class="card-body">
                                                <i class="bi bi-quote text-center"></i>
                                                <p class="testimony text-center">{{ testimonies.testimony }}</p>
                                                <div class="content">
                                                    <img class="image mx-auto" :src="testimonies.image">
                                                    <h4 class="text-center">{{ testimonies.personName }}</h4>
                                                    <h5 class="text-muted text-center">{{ testimonies.relation }}</h5>
                                                </div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="carousel-item" data-bs-interval="1000000" v-for="testimonies in testimonials"
                        :key="testimonies.id">
                        <div class="container-fluid text-center">
                            <div class="row justify-content-center">
                                <div class="col-12 col-lg-6 my-3 d-flex justify-content-around g-3 pb-4">
                                    <div class="card" style="width: 30rem; height: fit-content;">
                                        <div class="card-body">
                                            <i class="bi bi-quote text-center"></i>
                                            <p class="testimony text-center">{{ testimonies.testimony }}</p>
                                            <div class="content">
                                                <img class="image mx-auto" :src="testimonies.image">
                                                <h4 class="text-center">{{ testimonies.personName }}</h4>
                                                <h5 class="text-muted text-center">{{ testimonies.relation }}</h5>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleDark"
                    data-bs-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Previous</span>
                </button>
                <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleDark"
                    data-bs-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="visually-hidden">Next</span>
                </button>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data() {
        return {
            testimonialsActiveCarousel: [
                {
                    id: 1,
                    personName: 'Timothy Jennike',
                    image: 'https://i.postimg.cc/tT4PKdwm/C11-4.png',
                    testimony: 'Maxwill is a guy who becomes very passionate towards something when he becomes interested in it. He is very friendly and open to help anyone that has difficulty with any topic. He shows amazing creativity and problem-solving skills already. I recommend him to any company.',
                    relation: 'PEER'
                }
            ],
            testimonials: [
                {
                    id: 2,
                    personName: 'Brandon Swinton',
                    image: 'https://i.postimg.cc/XJMJtLb4/C11_Brandon_Swinton_(4).png',
                    testimony: 'Maxwill is very committed in his work. He loves learning. An incredible problem solver. His very discipline worker. Always willing to assist those in need. I enjoyed having Maxwill as a fellow developer.',
                    relation: 'PEER'
                },
                {
                    id: 3,
                    personName: 'Reece Simon',
                    image: 'https://i.postimg.cc/Y9t3Mrpn/Reece-Profile.png',
                    testimony: 'Maxwill is an exceptionally hard worker and always making time to assist anyone who is in need. Also goes the extra-mile when doing anything that has to be done. He is also very confident in his capabilities and never fails to get the Job done.',
                    relation: 'PEER'
                },
                {
                    id: 4,
                    personName: 'Joel Mukanya',
                    image: 'https://i.postimg.cc/wBp5Qqsq/Joel-Profile.png',
                    testimony: 'Maxwill is a very creative, goal-getter, and well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I am very delighted to see him build more awesome projects, and most importantly, companies will love to hire such a developer.',
                    relation: 'LECTURER'
                },
                {
                    id: 5,
                    personName: 'Javier Goodall',
                    image: 'https://i.postimg.cc/1RCH11bB/Javier-Profile.png',
                    testimony: 'Maxwill seems to be very passionate in web development because he puts in 100% in every project does. He is always willing to help and goes the extra mile for students who are struggling on their projects.',
                    relation: 'PEER'
                },
                {
                    id: 6,
                    personName: 'Deno Rautenbach',
                    image: 'https://i.postimg.cc/Qd4KYcCd/DSC_3597.png',
                    testimony: "Maxwill is a hardworking, results orientated team player. He has a keen eye for detail and always does the utmost to achieve a goal. I respect and admire this approach to problem solving as he has shown it's useful for technical as well as everyday problems. He's an inexpensive asset to any company out there looking to hire!",
                    relation: 'PEER'
                }
            ]
        }
    }
}
</script>
<style scoped>
*,
*::before,
*::after {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

#testimonials {
    background-color: #0c3047;
    min-height: 93vh;
    margin-left: 50px;
    overflow-x: hidden;
}

.carousel-control-prev-icon,
.carousel-control-next {
    color: #198754;
}

/* .carousel-item img{
    width: auto;
    height: 75vh;
    object-position: center;
    object-fit: cover;
} */

.cards {
    background-color: white;
    /* width: 50%;
    height: 30%; */
    border-radius: 10px;
}

i {
    display: block;
    color: #198754;
    font-size: 60px;
}

.testimony {
    margin: 0px auto;
}

h4 {
    color: #198754;
}

.image {
    width: 6rem;
    display: block;
    border-radius: 50px;
    border: 3px solid #198754;
}

/* .carousel {
    overflow: hidden;
} */
</style>