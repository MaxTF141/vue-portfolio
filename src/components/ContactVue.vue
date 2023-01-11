<template>
    <section id="contact">
        <h5 class="display-5 text-center text-success py-4">CONTACT ME</h5>
        <div class="container-fluid my-auto">
            <div class="row">
                <div class="col-12 col-lg-6 ps-lg-5">
                    <h6 class="display-6 text-lg-start text-center text-success">GET IN TOUCH</h6>
                    <p class="lead text-lg-start text-center text-light w-lg-50 w-100 mx-auto ms-lg-1 pb-3">You can
                        contact me by filling in the form on this page or via the contact information.</p>
                    <div class="contact-icons d-flex justify-content-lg-start py-2 justify-content-center">
                        <i class="bi bi-phone-fill text-success pt-1"></i>
                        <p class="lead text-light ps-3">+27 67 274 6346</p>
                    </div>
                    <div class="contact-icons d-flex justify-content-lg-start py-2 justify-content-center">
                        <i class="bi bi-envelope-open-fill text-success pt-1"></i>
                        <p class="lead text-light ps-3">isaacsmaxwill22@gmail.com</p>
                    </div>
                    <div class="contact-icons d-flex justify-content-lg-start py-2 justify-content-center">
                        <a href="https://www.facebook.com/maxwill.isaacs.9"><i
                                class="bi bi-facebook text-success pt-1"></i>
                        </a>
                        <p class="lead text-light ps-3">My FACEBOOK</p>
                    </div>
                    <div class="contact-icons d-flex justify-content-lg-start py-2 justify-content-center">
                        <a href="https://www.instagram.com/maxisaacs_22/"><i
                                class="bi bi-instagram text-success pt-1"></i></a>
                        <p class="lead text-light ps-3">My INSTAGRAM</p>
                    </div>
                    <div class="contact-icons d-flex justify-content-lg-start py-2 justify-content-center">
                        <a href="https://github.com/MaxTF141"><i class="bi bi-github text-success pt-1"></i></a>
                        <p class="lead text-light ps-3">My GitHub</p>
                    </div>
                </div>
                <div class="col-12 col-lg-6 pt-lg-5 mt-lg-5 text-center">
                    <h6 class="display-6 text-success">CONTACT FORM</h6>
                    <form action="https://formspree.io/f/xlevokwe" method="post">
                        <!-- 2 column grid layout with text inputs for the first and last names -->
                        <div class="row mb-4">
                            <div class="col">
                                <div class="form-outline">
                                    <input type="text" id="form3Example1" class="form-control" name="firstname"
                                        placeholder="First Name" required />
                                </div>
                            </div>
                            <div class="col">
                                <div class="form-outline">
                                    <input type="text" id="form3Example2" class="form-control" name="surname"
                                        placeholder="Last Name" required />
                                </div>
                            </div>
                        </div>

                        <!-- Email input -->
                        <div class="form-outline mb-4">
                            <input type="email" id="form3Example3" class="form-control" name="email"
                                placeholder="Email Address" required />
                        </div>
                        <!-- Message input -->
                        <div class="form-outline mb-4">
                            <textarea class="form-control" id="form4Example3" name="message" rows="4"
                                placeholder="Message" required></textarea>
                        </div>

                        <!-- Submit button -->
                        <button type="submit" class="btn btn-success btn-block d-block mx-auto">Contact Me</button>
                    </form>
                </div>
            </div>
        </div>
    </section>


</template>
<script>
export default {

}
</script>
<style scoped>
#contact {
    background-color:#0c3047;
    min-height: 100vh;
    overflow: hidden;
    margin-left: 50px;
}
#contact i {
    display: block;
    scale: 2;
    font-size: 1rem;
    color: #198754;

}

</style>