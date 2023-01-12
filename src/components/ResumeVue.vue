<template>
    <section id="resume">
        <h5 class="display-5 text-center text-success">RESUME</h5>
        <h6 class="display-6 text-center text-success">EDUCATION</h6>
        <div class="container-fluid text-center">
            <div class="row">
                <div class="col-12 col-lg-6 my-3 d-flex justify-content-around g-3 pb-4">
                    <div class="card" style="width: 30rem; height: fit-content;">
                        <div class="card-body">
                            <h5 class="display-5 card-title text-light">KUILS RIVER TECHNICAL HIGH SCHOOL</h5>
                            <p class="lead card-text text-light">I graduated from high school with a diploma.</p>
                            <h6 class="card-subtitle mb-2 text-dark">2015 - 2019</h6>
                        </div>
                    </div>
                </div>
                <div class="col-12 col-lg-6 my-3 d-flex justify-content-center g-3">
                    <div class="card" style="width: 30rem; height: fit-content;">
                        <div class="card-body">
                            <h5 class="display-5 card-title text-light">iCollege (Bellville Campus)</h5>
                            <p class="lead card-text text-light">I attended this college after I took a gap year after
                                school. I studied IT Tech Support NQF4 during that year.</p>
                            <h6 class="card-subtitle mb-2 text-dark">FEB - DEC 2021</h6>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="cards d-flex justify-content-center py-5 mx-2">
            <div class="card" style="width: 30rem; height:fit-content;">
                <div class="card-body">
                    <h5 class="display-5 card-title text-light">LIFE CHOICES CODING ACADEMY</h5>
                    <p class="lead card-text text-light text-light">So far it's been a great experience here at Life
                        Choices. I began to love coding more and more. And I have learnt a lot and It's just not
                        coding.I love how they implement everything that you'll need after you done with the Course.</p>
                    <h6 class="card-subtitle mb-2 text-dark">SEP 2022 - PRESENT</h6>
                </div>
            </div>
        </div>
        <h6 class="display-6 text-center text-success mt-4">WORK AND EXPERIENCE</h6>
        <div class="cards d-flex justify-content-center py-4 mx-2">
            <div class="card" style="width: 30rem; height:fit-content;">
                <div class="card-body">
                    <h5 class="display-5 card-title text-light">DE JAGERS UITRUSTERS</h5>
                    <p class="lead card-text text-light">De Jagers is a retail store. I worked there for about two years
                        as a temporary worker since I finished high school.</p>
                    <h6 class="card-subtitle mb-2 text-dark">MAR 2020 - PRESENT</h6>
                </div>
            </div>
        </div>
        <a class="text-decoration-none pb-4" href="/files"><button type="button"
                class="btn btn-success btn-lg d-block mx-auto">Download My CV</button></a>
    </section>
    <section id="skills">
        <div class="container-fluid pt-5">
            <div class="row pt-5">
                <h5 class="display-5 text-center text-success pt-lg-4">Skills</h5>
            </div>
            <div class="row pt-lg-4">
                <div class="col-2"></div>
                <div class="col-8">
                    <h6>HMTL5</h6>
                    <div class="progress">
                        <div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar"
                            aria-label="Default striped example" style="width: 85% " aria-valuenow="10"
                            aria-valuemin="0" aria-valuemax="100">85%</div>
                    </div>
                    <h6>CSS3</h6>
                    <div class="progress">
                        <div class="progress-bar progress-bar-striped bg-success progress-bar-animated"
                            role="progressbar" aria-label="Success striped example" style="width: 80%"
                            aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">80%</div>
                    </div>
                    <h6>Bootstrap5</h6>
                    <div class="progress">
                        <div class="progress-bar progress-bar-striped bg-info progress-bar-animated" role="progressbar"
                            aria-label="Info striped example" style="width: 70%" aria-valuenow="50" aria-valuemin="0"
                            aria-valuemax="100">70%</div>
                    </div>
                </div>
                <div class="col-2"></div>
            </div>
        </div>
    </section>
    


</template>
<script>
export default {
    data(){
        return{
           education: [
            {
                schoolName: 'KUILS RIVER TECHNICAL HIGH SCHOOL',
                description: 'I graduated from high school with a diploma.',
                timePeriod: '2015 - 2019'
            },
            {
                schoolName: 'iCollege (Bellville Campus)',
                description: 'I attended this college after I took a gap year after school. I studied IT Tech Support NQF4 during that year.',
                timePeriod: 'FEB - DEC 2021'
            },
            {
                schoolName: 'LIFE CHOICES CODING ACADEMY',
                description: "So far it's been a great experience here at Life Choices. I began to love coding more and more. And I have learnt a lot and It's just not coding.I love how they implement everything that you'll need after you done with the Course",
                timePeriod: 'SEP 2022 - PRESENT'
            },
           ],
           workExperience: [
            {
                companyName:'DE JAGERS UITRUSTERS',
                description:'De Jagers is a retail store. I worked there for about two years as a temporary worker since I finished high school.',
                timePeriod:'MAR 2020 - DEC 2022'
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

</style>