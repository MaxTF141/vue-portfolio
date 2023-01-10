<template>
    <section id="projects">
        <h5 class="display-5 text-success text-center py-4">PROJECTS</h5>
        <div class="container-fluid d-lg-flex justify-content-center">
            <div class="row gap-5 mx-5 px-5 justify-content-center">
                <Div v-for="project in projects" :key="project.id" class="card px-0" style="width: 18rem;">
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
    </section>

</template>
<script>
export default {
    data(){
        return {
            projects:[
                {
                    name: 'Javascript calculator',
                    image: 'https://i.postimg.cc/9QBP2Zy1/js-calculator.png',
                    githubLink: 'https://github.com/MaxTF141/JSCalculator.git',
                    netlifyLink: 'https://maxwill-jscalculator.netlify.app/'
                },
                {
                    name: 'E-commerce CRUD system',
                    image: 'https://i.postimg.cc/26wQm028/e-commerce-crud.png',
                    githubLink: 'https://github.com/MaxTF141/JSCalculator.git',
                    netlifyLink: 'https://maxwill-jscalculator.netlify.app/'
                },
                {
                    name: 'Todo App',
                    image: 'https://i.postimg.cc/tgw6bY0J/Todo-App-Google-Chrome-1-10-2023-3-01-45-PM.png',
                    githubLink: 'https://github.com/MaxTF141/Todo-App.git',
                    netlifyLink: 'https://maxwill-todo-app.netlify.app/'
                },
                {
                    name:'',
                    image:'',
                    githubLink:'',
                    netlifyLink:'',
                },
                {
                    name:'',
                    image:'',
                    githubLink:'',
                    netlifyLink:'',
                },
                {
                    name:'',
                    image:'',
                    githubLink:'',
                    netlifyLink:'',
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
    margin-left: 70px;
}
i{
  font-size: 27px;
  color: #198754;
}
.card {
    background-color:#11405e
}

</style>