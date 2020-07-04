<template>
    <div>
        <section class="section" id="main">
            <div class="container-fliud">
                <h1>John Gill</h1>
                <img alt="Vue logo" id="main-picture" class="rounded-circle" src="https://johnrgill.github.io/photo2.jpg">
                <h1>Software Developer</h1>
                <h4>and learning enthusiast</h4>
                <button type="button" class="btn btn-dark btn-lg" data-toggle="modal" data-target=".bd-example-modal-lg" data-aos="flip-up">Contact</button>
            </div>
        </section>
        <div class="container-fluid">
            <div class="row facts">
                <div class="col-md-4">
                        <div class="card" data-aos="fade-up">
                            <div class="card-head">
                                <h2>About me</h2>
                            </div>
                            <ul>
                                <li>Interested in computers since childhood</li>
                                <li>NSCC Web Dev Grad</li>
                                <li>Constantly learning new technologies</li>
                                <li>Windows/Unix and web/desktop</li>
                            </ul> 
                        </div>
                </div>

                <div class="col-md-4">
                        <div class="card" data-aos="fade-up">
                            <div class="card-head">
                                <h2>Technologies</h2>
                            </div>
                            <ul>
                                <li>JavaScript/Vue/Node</li>
                                <li>Python/Django</li>
                                <li>PHP</li>
                                <li>Java</li>
                            </ul> 
                        </div>
                </div>

                <div class="col-md-4">
                        <div class="card" data-aos="fade-up">
                            <div class="card-head">
                                <h2>Experience</h2>
                            </div>
                            <ul>
                                <li>Some freelance web experience</li>
                                <li>Personal projects for productivity</li>
                                <li>VBA Developer work term</li>
                                <li>Light 2D Game Development</li>
                            </ul> 
                        </div>
                </div>
            </div>
        </div>
        <section class="protfolio">
            <h1>Portfolio</h1>
            <p>Here are a few of my personal projects</p>
            <div class="container">
                <div class="row">
                    <div class="col-md-4">
                            <div class="card" data-aos="zoom-in-up">
                                <div class="card-head">
                                    <img alt="Vue logo" class="rounded-circle img-custom" src="https://johnrgill.github.io/johngillmusic/homepage.PNG">
                                    <h3>Personal music page</h3>
                                </div>
                                <hr>
                                <div class="card-body">
                                    <p>
                                        This is a personal website I created for myself and my music to get a better understanding of HTML,CSS, and jQuery.
                                    </p>
                          <button type="button" class="btn btn-outline-secondary">
                            <a href="http://andrewmac.ca/jungle/johngillmusic/" target="_blank">More</a>
                            </button>
                                </div>
                            </div>
                            <br>
                    </div>
                    <div class="col-md-4">
                            <div class="card" data-aos="zoom-in-down">
                                <div class="card-head">
                                    <img alt="Vue logo" class="rounded-circle img-custom" src="https://johnrgill.github.io/nicolemac/mainpage.png">
                                    <h3>Artist page/store front (frontend only)</h3>
                                </div>
                                <hr>
                                <div class="card-body">
                                    <p>
                                        Artist's store front/personal website I made for a project in school. This was useful in getting to know the grid system in Bootstrap.
                                    </p>
                                    <button type="button" class="btn btn-outline-secondary"><a href="http://andrewmac.ca/jungle/nicolemac/boot.html " target="_blank" >More</a></button>
                                </div>
                            </div>
                        <br>
                    </div>  
                    <div class="col-md-4">
                        <div class="card" data-aos="zoom-in-up">
                            <div class="card-head">
                                <img alt="Vue logo" class="rounded-circle img-custom" src="../assets/pword.png">
                                <h3>Python password generator</h3>
                            </div>
                            <hr>
                            <div class="card-body">
                                <p>
                                    This is a quick little password generator I spun up using python and tkinter. 
                                </p>
                                <button type="button" class="btn btn-outline-secondary"><a href="https://github.com/johnrgill/pword/blob/master/pword.py" target="_blank">More</a> </button>
                            </div>
                        </div>
                        <br>
                    </div>
                </div>
            </div>
        </section>
        <!-- modal for contact -->
        <section class="">
            <div class="modal fade bd-example-modal-lg" tabindex="-1" 
                role="dialog" aria-labelledby="myLargeModalLabel" aria-hidden="true">
                    <div class="modal-dialog modal-lg">
                            <div class="modal-content">
                                <contact/>
                            </div>
                    </div>
                </div>
        </section>
        <footer><small>&copy; John Gill 2020</small></footer>
    </div>
    
    
</template>
<script lang="ts">
import contact from './contact.vue'
export default {
    name:'Lander',
    components:{
        contact
    }  
}
</script>

<style lang="css" scoped>
    .section{
        padding-top: 10%;
        padding-bottom: 10%;
        font-family: Roboto;
        color: white;
    }
    .protfolio{
        background-color: #343a40;
        padding-top: 8%;
        padding-bottom: 15%;
        /* padding:15% */
        background-image: url("../assets/bg2.jpg");
        font-family: Roboto;
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
    }
    .img-custom{
        width: 140px;
        height: 140px;
        margin-top: 15px;
        transition: transform .2s; 
    }
    .img-custom:hover{
        transform: scale(1.5);
    }
    #main-picture{
        width: 50%;
       
    }
    #main{
        background-image: url("../assets/bg4.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
    }
    footer{
        float: right;
        font-family: Roboto;
    }
    a{
        text-decoration: none;
        color: black;
    }
    li{
        list-style-position: inside;
        list-style-type: square;
        margin: 2%;
        color: #343a40;
        text-align: left;
    }
    .facts{
        background-color: #343a40;
        font-family: Roboto; 
    }
    
    
</style>