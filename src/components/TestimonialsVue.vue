<template>
    <section id="testimonials">
        <h5 class="display-5 text-success text-center py-4">TESTIMONIALS</h5>
        <div class="container-fluid" id="carousel">
            <div id="carouselExampleDark" class="carousel carousel-dark slide" data-bs-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active" data-bs-interval="10000" v-for="testimonies in testimonialsActiveCarousel" :key="testimonies.id">
                        <img :src="testimonies.image" class="img-fluid d-block w-25 mx-auto" alt="testimony"
                            loading="lazy">
                        <p class="lead text-center font-italic text-muted"> {{testimonies.relation}}</p>
                        <h5 class="display-5 text-white text-center mx-auto my-0 pt-1"> {{testimonies.personName}}</h5>
                        <p class="lead text-center text-light w-75 mx-auto px-0 px-md-5">{{testimonies.testimony}}</p>
                    </div>
                    <div class="carousel-item" data-bs-interval="10000"  v-for="testimonies in testimonials" :key="testimonies.id">
                        <img :src="testimonies.image"
                            class="img-fluid d-block w-25 mx-auto" alt="testimony" loading="lazy">
                        <p class="lead text-center font-italic text-muted">{{ testimonies.relation }}</p>
                        <h5 class="display-5  text-white text-center mx-auto pt-1">{{ testimonies.personName }}</h5>
                        <p class="lead text-center text-light mx-auto my-0 w-75 px-lg-5">{{ testimonies.testimony }}
                        </p>
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
                    image: 'https://i.postimg.cc/BQzGqxD9/C11-4.jpg',
                    testimony: 'Maxwill is a guy who becomes very passionate towards something when he becomes interested in it. He is very friendly and open to help anyone that has difficulty with any topic. He shows amazing creativity and problem-solving skills already. I recommend him to any company.',
                    relation: 'PEER'
                }
            ],
            testimonials:[
                {
                    id: 2,
                    personName: 'Brandon Swinton',
                    image: 'https://i.postimg.cc/8cDzmL4n/C11-Brandon-Swinton-4.jpg',
                    testimony: 'Maxwill is very committed in his work. He loves learning. An incredible problem solver. His very discipline worker. Always willing to assist those in need. I enjoyed having Maxwill as a fellow developer.',
                    relation: 'PEER'
                },
                {
                    id: 3,
                    personName: 'Reece Simon',
                    image: 'https://i.postimg.cc/TPMrLBGG/Reece-Profile.jpg',
                    testimony: 'Maxwill is an exceptionally hard worker and always making time to assist anyone who is in need. Also goes the extra-mile when doing anything that has to be done. He is also very confident in his capabilities and never fails to get the Job done.',
                    relation: 'PEER'
                },
                {
                    id: 4,
                    personName: 'Joel Mukanya',
                    image: 'https://i.postimg.cc/yYLQR1rK/Joel-Profile.jpg',
                    testimony: 'Maxwill is a very creative, goal-getter, and well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I am very delighted to see him build more awesome projects, and most importantly, companies will love to hire such a developer.',
                    relation: 'LECTURER'
                },
                {
                    id: 5,
                    personName: 'Javier Goodall',
                    image: 'https://i.postimg.cc/YSmjxr6Z/Javier-Profile.jpg',
                    testimony: 'Maxwill seems to be very passionate in web development because he puts in 100% in every project does. He is always willing to help and goes the extra mile for students who are struggling on their projects.',
                    relation: 'PEER'
                },
                {
                    id: 6,
                    personName: 'Deno Rautenbach',
                    image: 'https://i.postimg.cc/Hxfd6X2C/IMG-20221205-WA0042.jpg',
                    testimony: "Maxwill is a hardworking, results orientated team player. He has a keen eye for detail and always does the utmost to achieve a goal. I respect and admire this approach to problem solving as he has shown it's useful for technical as well as everyday problems. He's an inexpensive asset to any company out there looking to hire!",
                    relation: 'PEER'
                }
            ]
        }
    }
}
</script>
<style scoped>
#testimonials {
    background-color: #0c3047;
    /* min-height: 100vh; */
    margin-left: 50px;
    overflow-x: none;
}
#carousel {
    height: 100vh;
    width: 100vw;
}
.carousel-control-prev, .carousel-control-next {
    width: 50px;
}

</style>