<template>
    <section id="resume">
        <h5 class="display-5 text-center text-success">RESUME</h5>
        <h6 class="display-6 text-center text-success">EDUCATION</h6>
        <div class="container text-center" v-for="school in education" :key="school.id">
            <div class="timeline timeline_area">
                <div class="row py-5" >
                    <div class=" timeline-badge"></div>
                    <div class="col-12">
                        <!-- <img :src="school.image" alt="png" style="width: 10rem;"> -->
                        <div class="info px-2">
                            <h4 class="text-white">{{ school.schoolName }}</h4>
                            <p class="text-white">{{ school.description }}</p>
                            <h5 class="text-white">{{ school.timePeriod }}</h5>
                        </div>
                    </div>
            </div>
            </div>
        </div>

    </section>
    <section id="skills">
        <div class="container-fluid pt-5">
            <div class="row pt-5">
                <h5 class="display-5 text-center text-success pt-lg-4">Skills</h5>
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
                    schoolName: 'KUILS RIVER TECHNICAL HIGH SCHOOL',
                    image: 'https://i.postimg.cc/RhK674kH/My_project.png',
                    description: 'I graduated from high school with a diploma.',
                    timePeriod: '2015 - 2019'
                },
                {
                    schoolName: 'iCollege (Bellville Campus)',
                    description: 'I attended this college after I took a gap year after school. I studied IT Tech Support NQF4 during that year.',
                    image: 'https://i.postimg.cc/VLrQF4km/i-COLLEGE-White-Logo.gif',
                    timePeriod: 'FEB - DEC 2021'
                },
                {
                    schoolName: 'LIFE CHOICES CODING ACADEMY',
                    description: "So far it's been a great experience here at Life Choices. I began to love coding more and more. And I have learnt a lot and It's just not coding.I love how they implement everything that you'll need after you done with the Course",
                    image: 'https://i.postimg.cc/0jnPmNkj/logo_429x99.png',
                    timePeriod: 'SEP 2022 - PRESENT'
                },
            ],
            workExperience: [
                {
                    companyName: 'DE JAGERS UITRUSTERS',
                    description: 'De Jagers is a retail store. I worked there for about two years as a temporary worker since I finished high school.',
                    image:'https://i.postimg.cc/52091fsS/De-Jagers-Logo-Master-Revised-Mrt-2015-copy.png',
                    timePeriod: 'MAR 2020 - DEC 2022'
                }
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
.timeline_area{
    /* border-left: 2px solid #198754; */
    margin-left: 30%;
    
}
.row {
    position: relative;

}



.timeline:before {
  top: 0;
  bottom: 0;
  margin-top: 20px;
  position:absolute;
  content: " ";
  width: 3px;
  background-color:#198754;
  left: 30%;

}

.timeline-badge {
  color: rgb(0, 0, 0);
  width: 50px;
  height: 50px;
  line-height: 50px;
  font-size: 1.4em;
  text-align: center;
  position: relative;
  top: 16px;
  left: -10%;
  z-index: 100;
  border-top-right-radius: 50%;
  border-top-left-radius: 50%;
  border-bottom-right-radius: 50%;
  border-bottom-left-radius: 50%;
}

.timeline-badge {
  background-color: #198754 !important;
}
</style>