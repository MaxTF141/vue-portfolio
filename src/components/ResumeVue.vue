<template>
    <section id="resume">
        <h5 class="display-5 text-center text-success">RESUME</h5>
        <div class="timeline">
            <div v-for="school in education" :key="school.id">
                <div class="timeline-badge" :class="school.class">
                    <div class="content px-2">
                        <h4 class="text-white">{{ school.name }}</h4>
                        <p class="text-white">{{ school.description }}</p>
                        <h5 class="text-white">{{ school.timePeriod }}</h5>
                    </div>
                </div>
            </div>
        </div>

    </section>
    <section id="skills">
            <h5 class="display-5 text-center text-success pt-lg-4">Skills</h5>
            <div class="container-fluid">
                <div class="row pt-5 gap-5">
                    <div class="col-lg-12 d-flex justify-content-center gap-4 pb-5">
                        <img class="img-fluid" src="https://i.postimg.cc/X7N1TkNX/html-5.png" alt="">
                        <img class="img-fluid" src="https://i.postimg.cc/sgqnGFYZ/css-3.png" alt="">
                        <img class="img-fluid" src="https://i.postimg.cc/jjfMz8c3/bootstrap.png" alt="">
                        <img class="img-fluid" src="https://i.postimg.cc/HsSvH8jz/js.png" alt="">
                        <img class="img-fluid" src="https://i.postimg.cc/NMwpb1Ps/pngwing.com_(5).png" alt="">
                    </div>
                </div>
            </div>
    </section>



</template>
<script>
export default {
    data() {
        return {
            education: [
                {
                    name: 'KUILS RIVER TECHNICAL HIGH SCHOOL',
                    image: 'https://i.postimg.cc/RhK674kH/My_project.png',
                    description: 'I graduated from high school with a diploma.',
                    timePeriod: '2015 - 2019',
                    class: 'right',
                },
                {
                    name: 'DE JAGERS UITRUSTERS',
                    description: 'De Jagers is a retail store. I worked there for about two years as a temporary worker since I finished high school.',
                    image: 'https://i.postimg.cc/52091fsS/De-Jagers-Logo-Master-Revised-Mrt-2015-copy.png',
                    timePeriod: 'MAR 2020 - DEC 2022',
                    class: 'left'
                },
                {
                    name: 'iCollege (Bellville Campus)',
                    description: 'I attended this college after I took a gap year after school. I studied IT Tech Support NQF4 during that year.',
                    image: 'https://i.postimg.cc/VLrQF4km/i-COLLEGE-White-Logo.gif',
                    timePeriod: 'FEB - DEC 2021',
                    class: 'right',
                },    
                {
                    name: 'LIFE CHOICES CODING ACADEMY',
                    description: "So far it's been a great experience here at Life Choices. I began to love coding more and more. And I have learnt a lot and It's just not coding.I love how they implement everything that you'll need after you done with the Course",
                    image: 'https://i.postimg.cc/0jnPmNkj/logo_429x99.png',
                    timePeriod: 'SEP 2022 - PRESENT',
                    class: 'left'
                },
            ],
            workExperience: [
            ]
        }
    }
}
</script>
<style>
#resume {
    background-color: #0c3047;
    padding-top: 20px;
    min-height: 100vh;
    margin-left: 50px;
}

#resume .card {
    background-color: #198754;
}

#skills {
    background-color: #0c3047;
    padding-top: 20px;
    min-height: 40vh;
    margin-left: 50px;
}

#skills h6 {
    color: white;
    padding-left: 10px;
}

.timeline {
    position: relative;
    max-width: 1200px;
    margin: 0 auto;
}

.timeline::after {
    content: '';
    position: absolute;
    width: 6px;
    background-color: #198754;
    top: 0;
    bottom: 0;
    left: 50%;
    margin-left: -3px;
}

.timeline-badge {
    padding: 10px 40px;
    position: relative;
    background-color: inherit;
    width: 50%;
}

.timeline-badge::after {
    content: '';
    position: absolute;
    width: 25px;
    height: 25px;
    right: -13px;
    background-color: #0c3047;
    border: 4px solid #198754;
    top: 15px;
    border-radius: 50%;
    z-index: 1;
}

.left {
    left: 0;
}

.right {
    left: 50%;
}

.left::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    right: 30px;
    border: medium solid #198754;
    border-width: 10px 0 10px 10px;
    border-color: transparent transparent transparent #198754;
}

.right::before {
    content: " ";
    height: 0;
    position: absolute;
    top: 22px;
    width: 0;
    z-index: 1;
    left: 30px;
    border: medium solid #198754;
    border-width: 10px 10px 10px 0;
    border-color: transparent #198754 transparent transparent;
}

.right::after {
    left: -12px;
}

.content {
    padding: 20px 30px;
    position: relative;
    border-radius: 6px;
}

#skills img {
    width: 12%;
}

@media screen and (max-width: 600px) {
    .timeline::after {
        left: 38px;
    }

    .timeline-badge {
        width: 100%;
        padding-left: 70px;
        padding-right: 25px;
    }

    .left::after,
    .right::after {
        left: 25px;
    }

    .right {
        left: 0%;
    }
}
</style>