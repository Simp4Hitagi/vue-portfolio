<template>
    <div>
        <div class="container">
            <div class="row justify-content-around">
                <div class="col-8">
                    <h1 class="display-1 fw-bold animate__animated animate__fadeInDown">Testimonials</h1>
                </div>
            </div>
        </div>
        <div class="container">
            <div class="row justify-content-around">
                <div v-for="testimonial in testimonials" :key="testimonial">
                    <div class="card mb-3 m-auto" style="max-width: 540px;">
                        <div class="row g-0 m-auto">
                          <div class="col-md-4">
                            <img :src=testimonial.image alt="..." class="img-fluid rounded-start card-img-top img-fluid m-auto " style="width: 100%; height: 100%">
                          </div>
                          <div class="col-md-8">
                            <div class="card-body">
                              <h5 class="card-title">{{testimonial.name}}</h5>
                              <p class="card-text">{{testimonial.title}}</p>
                              <p class="card-text">{{testimonial.testimonial}}</p>
                            </div>
                          </div>
                        </div>
                      </div>
                </div>
    
            </div>
        </div>
    </div>
    <Footer/>
</template>
<script>
import Footer from '@/components/Footer.vue';
export default {
    name: 'testimonials',
    components: {
        Footer
    },
    data(){
        return{
            testimonials: [
                {
                    name: "Joel Mukanya",
                    title: "LC Lecturer",
                    testimonial: "Deno is a very creative, go-getter, and well-behaved student. He does enjoy working with his classmates and works well on his project. He has gained knowledge of web development, including Bootstrap 5. I will be very delighted to see him get hired as a developer.",
                    image: "https://i.postimg.cc/Ghbvn8KL/Joel-Profile.jpg"
                },
                {
                    name: "Umayr Nordien",
                    title: "Student",
                    testimonial: "I know I can depend on Deno to collaborate with on both large scale projects and smaller casual ones. He is steadfast in his ethical behavior and does not budge from these values according from what I've learned from a professional capacity. In a casual manner he's a friendly person and considerate of others and has a good mentality and outlook on life.",
                    image: "https://i.postimg.cc/bY15qwDC/Umayar.jpg"
                },
                {
                    name: "Uzukhanye Dywili",
                    title: "Student",
                    testimonial: "Thoughtful, hardworker, caring, smart, and confident are words that best describe Deno. A person who willingly goes an extra mile to get things done.",
                    image: "https://i.postimg.cc/g0CwdWnp/Uzukhanye.jpg"
                },
                {
                    name: "John-Bruce Noad",
                    title: "Student",
                    testimonial: "Deno is a self-confident and determined individual. Once he sets his mind to something, it is near impossible to shift his course.  Deno is not easily bothered by what others think or say about him, and is therefore easy to get along with. When it comes to his work, he is not afraid in the slightest to put his hard-working nature, and his amazing intellect on full display. I have enjoyed working alongside Deno, and can say with absolute confidence that he will be a great asset to any company that affords him the opportunity to present his value.",
                    image: "https://i.postimg.cc/9fWZj8Gg/John.jpg"
                },
                {
                    name: "Luntu ",
                    title: "Student",
                    testimonial: "Deno is a reliable person who is not turn down a fellow coder's cry for help when they need it. His determination to never turn down a challenge, work ethic, and intellect makes him a great asset to have in a team and said team is bound to be successful in whichever task if he is involved in it.",
                    image: "https://i.postimg.cc/4yL9TCRv/DSC-3496.jpg"
                },
                {
                    name: "KonkeJeff RicardoMalindi",
                    title: "Student",
                    testimonial: "Deno is like a sponge, constantly absorbing knowledge and has a very keen interest in finding out the salution to a problem he has no idea how to solve,that is why in work space he would be a very resourceful asset",
                    image: "https://i.postimg.cc/Gm9nTXgJ/DSC-3528.jpg"
                }, 
                {
                    name: "Cassidy Manuel",
                    title: "LC Studio Intern",
                    testimonial: "Deno is respectful, dedicated and a driven individual. He thrives in a team work environment and I would highly recommend him.",
                    image: "https://i.postimg.cc/RFPQjTnH/Cassidy.jpg"
                }
            ]
        }
    }
}
</script>
<style scoped>

</style>