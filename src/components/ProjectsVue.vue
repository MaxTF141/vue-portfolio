<template>
    <section id="projects">
        <h5 class="display-5 text-success text-center">PROJECTS</h5>
        <div class="container-fluid">
            <div class="row">
                <div class="col-lg-4 col-12 mt-2 py-lg-5 py-0" v-for="project in projects" :key="project.id" >
                    <div class="card mx-auto w-100">
                        <img :src="project.image" class="card-img-top" alt="...">
                        <div class="card-body">
                            <h4 class="card-text">{{ project.name }}</h4>
                            <div class="icons d-flex gap-2">
                                <a :href="project.githubLink" target="blank"><i class="bi bi-github"></i></a>
                                <a :href="project.netlifyLink" target="blank"><i class="bi bi-globe"></i></a>
                            </div>
                        </div>
                    </div>                    
                </div>
                <div class="col-lg-4 col-12 py-2 py-lg-5 py-5"  v-for="project in projects2" :key="project.id">
                    <div class="card mx-auto w-100">
                        <img :src="project.image" class="card-img-top" alt="...">
                        <div class="card-body d-flex flex-column justify-content-space-between">
                            <h4 class="card-text">{{ project.name }}</h4>
                            <div class="icons d-flex gap-2">
                                <a :href="project.githubLink" target="blank"><i class="bi bi-github"></i></a>
                                <a :href="project.netlifyLink" target="blank"><i class="bi bi-globe"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>
<script>
export default {
    data() {
        return {
            projects: [
                {
                    id: 1,
                    name: 'Javascript calculator',
                    image: 'https://i.postimg.cc/9QBP2Zy1/js-calculator.png',
                    githubLink: 'https://github.com/MaxTF141/JSCalculator.git',
                    netlifyLink: 'https://maxwill-jscalculator.netlify.app/'
                },
                {
                    id: 2,
                    name: 'E-commerce CRUD system',
                    image: 'https://i.postimg.cc/26wQm028/e-commerce-crud.png',
                    githubLink: 'https://github.com/MaxTF141/JSCalculator.git',
                    netlifyLink: 'https://maxwill-jscalculator.netlify.app/'
                },
                {
                    id: 3,
                    name: 'Todo App',
                    image: 'https://i.postimg.cc/tgw6bY0J/Todo-App-Google-Chrome-1-10-2023-3-01-45-PM.png',
                    githubLink: 'https://github.com/MaxTF141/Todo-App.git',
                    netlifyLink: 'https://maxwill-todo-app.netlify.app/'
                },
            ],
            projects2: [
                {
                    id: 4,
                    name: 'Vue Exercise E-commerce',
                    image: 'https://i.postimg.cc/N0tc08JF/vue-exercise1-Google-Chrome-1-11-2023-9-52-10-AM.png',
                    githubLink: 'https://github.com/MaxTF141/vue-exercise-ecommerce.git',
                    netlifyLink: 'https://hoodies-ecommerce.netlify.app/',
                },
                {
                    id: 5,
                    name: 'HMTL5 And CSS3 Portfolio',
                    image: 'https://i.postimg.cc/Vk5Zrbjq/first-project.png',
                    githubLink: 'https://github.com/MaxTF141/Portfolio',
                    netlifyLink: 'http://maxwill-firstportfolio.netlify.app',
                },
                {
                    id: 6,
                    name: '',
                    image: '',
                    githubLink: '',
                    netlifyLink: '',
                }

            ]
        }
    }
}
</script>

<style scoped>
#projects {
    background-color: #0c3047;
    padding-top: 20px;
    min-height: 100vh;
    overflow-x: none;
    margin-left: 50px;
}

i {
    font-size: 27px;
    color: #198754;
}

.card {
    background-color: #11405e
}
</style>