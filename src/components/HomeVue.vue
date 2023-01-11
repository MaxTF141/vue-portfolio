<template>
  <section id="landing">
    <div class="container-fluid">
      <div class="row pt-5">
        <div class="col-12 col-lg-6 d-flex d-lg-flex mt-lg-5 justify-content-center">
          <img class="img-fluid showcase" src="../assets/undraw_code_thinking_re_gka2.svg" alt="laptop-coding"
            loading="lazy">
        </div>
        <div class="col-12 col-lg-6 text-light text-center m-auto name-animation">
          <p class="lead py-3">hi, WELCOME!</p>
          <h3 class="display-3">I'm <span class="text-success">Maxwill Isaacs</span></h3>
          <p class="lead pb-3">And I'm an Aspired Developer</p>
          <div class="icons d-flex justify-content-center gap-3">
            <a href="https://www.linkedin.com/in/maxwill-isaacs-88a1a2212/" target="_blank"><i
                class="bi bi-linkedin text-success mx-2"></i></a>
            <a href="https://www.instagram.com/maxisaacs_22/" target="_blank"><i
                class="bi bi-instagram text-success mx-2"></i></a>
            <a href="https://www.facebook.com/maxwill.isaacs.9" target="_blank"><i
                class="bi bi-facebook text-success mx-2"></i></a>
          </div>
        </div>
        <router-link class="text-decoration-none" to="./about"><button type="button"
            class="btn btn-success d-block mt-4 mx-auto mt-5">View more...</button></router-link>
      </div>
    </div>
  </section>
</template>
<script>
export default {

}
</script >
<style scoped>
#landing {
    background-color: #0c3047;
    padding-top: 20px;
    min-height: 100vh;
    margin-left: 50px;
}

i{
  font-size: 2rem;
  color: white;
}

#landing .name-animation {
    animation: name-breathing 10s  infinite normal;
}
#landing button {
    animation: nav-hover 10s  infinite normal;
}


@keyframes name-breathing {
    0% {
        transform: scale(1);
    }
    16% {
        transform: scale(1.1);
    }
    32% {
        transform: scale(1);
    }
    48% {
        transform: scale(1.1);
    }
    64% {
        transform: scale(1);
    }
    80% {
        transform: scale(1.1);
    }
    100% {
        transform: scale(1);
    }
}

</style>