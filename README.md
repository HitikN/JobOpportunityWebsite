# JobOpportunityWebsite
// This is website is about Japan Job Oppertunity //

-------------------------------------------------------------------------------->> style.css <<--------------------------------------------------------------------------------------------------------

@import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css');

@import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@300;400;500;600;700&display=swap');

:root {
    --main-color: #2980b9;
    --red: red;
    --light-color: #777;
    --light-bg: #eee;
    --black: #2c3e50;
    --white: #fff;
    --box-shadow: 0 .5rem 1rem rgba(0, 0, 0, .1);
    --border: .1rem solid rgba(0, 0, 0, .2);

}

* {
    font-family: 'Comfortaa', cursive;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    outline: none;
    border: none;
}

*::selection {
    background-color: var(--main-color);
    color: var(--white);
}

::-webkit-scrollbar {
    width: 1rem;
    height: .5rem;

}

::-webkit-scrollbar-track {
    background-color: transparent;
}


::-webkit-scrollbar-thumb {
    background-color: var(--main-color);
}

html {
    font-size: 62.5%;
    overflow-x: hidden;
    scroll-padding-top: 7rem;
    scroll-behavior: smooth;
}

body {
    background-color: var(--light-bg);
}

section {
    padding: 2rem;
    margin: 0 auto;
    max-width: 1200px;
}

.heading{
    text-align: center;
    margin-bottom: 2rem;
    font-size: 3rem;
    color: var(--black);
    text-transform: capitalize;
    padding: 1rem 0;
}

.section-title{
    border-top: 1rem solid var(--main-color);
    border-bottom: 1rem solid var(--main-color);
    background-color: var(--black);
    color: var(--white);
    text-align: center;
    padding: 6rem 2rem;
    font-size: 6rem;
    text-transform: capitalize;
}

.btn {
    display: inline-block;
    margin-top: 1rem;
    padding: 1rem 3rem;
    cursor: pointer;
    font-size: 1.8rem;
    color: var(--white);
    background-color: var(--main-color);
    border-radius: .5rem;
    text-transform: capitalize;
    text-align: center;
}

.btn:hover {
    background-color: var(--black);

}

.flex-btn{
    display: flex;
    align-items: center;
    justify-content: space-between;
    column-gap: 1rem;
    flex-wrap: wrap;
}

.header {
    position: sticky;
    top: 0;
    left: 0;
    right: 0;
    background-color: var(--white);
    box-shadow: var(--border);
    z-index: 1000;
}

.header .flex {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

#menu-btn {
    font-size: 2.7rem;
    color: var(--black);
    cursor: pointer;
    display: none;
}

.header .flex .logo {
    font-size: 2.2rem;
    color: var(--black);
}

.header .flex .logo i {
    margin-right: .5rem;
    color: var(--light-color);
}

.header .flex .navbar a {
    display: inline-block;
    padding: 1rem 1.5rem;
    font-size: 1.6rem;
    color: var(--light-color);
    border-radius: .5rem;
    text-transform: capitalize;
}

.header .flex .navbar a:hover {
    background-color: var(--main-color);
    color: var(--white);
}

.home-container{
    background: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTCNUnSe4Wh8Adfb62NYBDI37bhfrBgXwXMfItNvF_i7Q&s'), rgba(0, 0, 0, .7) no-repeat;
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-blend-mode: color;
}

.home-container .home{
    min-height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.home-container .home form{
    background-color: var(--white);
    width: 50rem;
    border-radius: .5rem;
    text-align: center;
}

.home-container .home form h3{
     font-size: 2.5rem;
     color: var(--black);
     margin-bottom: 1rem;
     text-transform: capitalize;

}

.home-container .home form p{
    text-align: left;
    font-size: 1.6rem;
    color: var(--light-color);
    padding-top: 1rem;

}

.home-container .home form p span{
    color: var(--red);
} 

.home-container .home form .input{
    width: 100%;
    border-radius: .5rem;
    margin: 1rem 0;
    background-color: var(--light-bg);
    padding: 1.4rem;
    font-size: 1.8rem;
    color: var(--black);
}

.category .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, 25rem);
    justify-content: center;
    align-items: flex-start;
    gap: 1.5rem;

}

.category .box-container .box{
    border-radius: .5rem;
    box-shadow: var(--box-shadow);
    border: var(--border);
    background: var(--white);
    display: flex;
    align-items: center;
    gap: 2rem;

}

.category .box-container .box i{
    height: 4.5rem;
    width: 5rem;
    line-height: 4.5rem;
    font-size: 1.8rem;
    color: var(--black);
    border-radius: .5rem;
    background-color: var(--light-bg);
    text-align: center;

}

.category .box-container .box h3{
    font-size: 1.8rem;
    text-transform: capitalize;
    color: var(--black);
    padding-bottom: 4rem;
}

.category .box-container .box span{
    color: var(--light-color);
    font-size: 1.6rem;
}

.category .box-container .box:hover{
    background-color: var(--black);
}

.category .box-container .box:hover h3{
    color: var(--white);

}

.category .box-container .box:hover span{
    color: var(--white);
}

.category .box-container .box:hover i{
    color: var(--black);
    background-color: var(--white);
}

.jobs-container .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, 35rem);
    gap: 1.5rem;
    align-items: flex-start;
    justify-content: center;
}

.jobs-container .box-container .box{
    background-color: var(--white);
    border-radius: .5rem;
    border: var(--border);
    padding: 2rem;
    box-shadow: var(--box-shadow);
    overflow-x: hidden;

}

.jobs-container .box-container .box .company{
    display: flex;
    align-items: center;
    gap: 1.5rem;


}

.jobs-container .box-container .box .company img{
    height: 6rem;
    width: 6rem;
    object-fit: contain;
}

.jobs-container .box-container .box .company h3{
    font-size: 1.8rem;
    color: var(--black);
    text-overflow: ellipsis;
    overflow-x: hidden;
    text-transform: capitalize;
    padding-bottom: .5rem;
}

.jobs-container .box-container .box .company p{
    color: var(--light-color);
    font-size: 1.6rem;

}

.jobs-container .box-container .box .job-title{
    font-size: 2rem;
    color: var(--black);
    text-transform: capitalize;
    overflow: hidden;
    text-overflow: ellipsis;
}

.jobs-container .box-container .box .location{
    padding: .7rem 0;
    font-size: 1.6rem;
    color: var(--light-color);

}

.jobs-container .box-container .box .location i{
    margin-right: .3rem;
    color: var(--main-color);
}


.jobs-container .box-container .box .tags{
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    margin: 1.2rem 0;

}

.jobs-container .box-container .box .tags p{
    padding: 1rem 3 rem;
    border-radius: .5rem;
    border-color: var(--light-bg);
    font-size: 1.6rem;
    color: var(--light-color);

}

.jobs-container .box-container .box .tags p i{
    margin-right: .5rem;
    color: var(--black);
}

.jobs-container .box-container .box .fa-heart{
    background-color: var(--light-bg);
    border-radius: .5rem;
    color: var(--light-color);
    font-size: 1.8rem;
    cursor: pointer;
    height: 4rem;
    width: 4.5rem;
    line-height: 4rem;

}

.jobs-container .box-container .box .fa-heart:hover{
    background-color: var(--black);
    color: var(--white);
}

.jobs-container .box-container .box .fa-heart:hover{
    background-color: var(--black);
    color: var(--white);
}

.about img{
    width: 100%;
    margin-bottom: 1.5rem;
}


.about .box{
    background-color: var(--white);
    border-radius: .5rem;
    border: var(--border);
    padding: 2rem;
    box-shadow: var(--box-shadow);
}

.about .box h3{
    font-size: 2.5rem;
    color: var(--black);
    margin-bottom: 1rem;
    text-transform: capitalize;
}

.about .box p{
    padding: 1rem 0;
    line-height: 1.8;
    color: var(--light-color);
    font-size: 1.6rem;
}

.reviews .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, 35rem);
    gap: 1.5rem;
    align-items: flex-start;
    justify-content: center;
}

.reviews .box-container .box{
    background-color: var(--white);
    box-shadow: var(--box-shadow);
    border: var(--border);
    border-radius: .5rem;
    padding: 2rem;
}

.reviews .box-container .box .star{
    margin-bottom: 1.5rem;

}

.reviews .box-container .box .star i{
    color: var(--main-color);
    font-size: 1.8rem;
}

.reviews .box-container .box .title{
    text-transform: capitalize;
    font-size: 2rem;
    color: var(--black);
    text-align: right;

}

.reviews .box-container .box p{
    text-align: right;
    font-size: 1.6rem;
    color: var(--light-color);
    padding: 1rem 0;
    line-height: 1.8;
}

.reviews .box-container .box .user{
    display: flex;
    gap: 1.5rem;
    margin-top: 1rem;
    align-items: center;

}

.reviews .box-container .box .user img{
    height: 6rem;
    width: 6rem;
    border-radius: 50%;
    object-fit: cover;
}

.reviews .box-container .box .user h3{
    font-size: 2rem;
    color: var(--black);
    margin-bottom: .5rem;
    text-transform: capitalize;
}

.reviews .box-container .box .user span{
    color: var(--light-color);
    font-size: 1.6rem;
}

.job-filter form{
    background-color: var(--white);
    box-shadow: var(--box-shadow);
    border: var(--border);
    border-radius: .5rem;
    padding: 2rem;


}


.job-filter form .flex{
    display: flex;
    flex-wrap: wrap;
    column-gap: 1rem;
}

.job-filter form .flex .box{
    flex: 1 1 40rem;
}

.job-filter form .flex .box p{
    font-size: 1.6rem;
    color: var(--light-color);
    
}

.job-filter form .flex .box p span{
     color: var(--red);

}

.job-filter form .flex .box .input{
    width: 100%;
    border-radius: .5rem;
    padding: 1.4rem;
    color: var(--black);
    margin: 1rem 0;
    background-color: var(--light-bg);
    font-size: 1.8rem;
}

.job-filter form .dropdown-container{
    margin-top: 2rem;
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
}

.job-filter form .dropdown-container .dropdown{
    flex: 1 1 20rem;
    position: relative;
}

.job-filter form .dropdown-container .dropdown .output{
    width: 100%;
    background: var(--light-bg);
    border-radius: .5rem;
    padding: 1.4rem;
    font-size: 1.8rem;
    color: var(--black);
    text-align: center;
    user-select: none;
    cursor: pointer;
}

.job-filter form .dropdown-container .dropdown .output:placeholder-shown{
    text-transform: capitalize;
}

.job-filter form .dropdown-container .dropdown .lists{
    position: absolute;
    top: 100%; left: 0; right: 0;
    background-color: var(--white);
    padding: 1rem;
    border-radius: .5rem;
    background-color: var(--white);
    border: var(--border);
    box-shadow: var(--box-shadow);
    z-index: 10;

    transform: scaleY(0);
    transform-origin: top;
}

.job-filter form .dropdown-container .dropdown .lists .items{
    padding: 1.2rem 1.4rem;
    border-radius: .5rem;
    font-size: 1.6rem;
    color: var(--black);
    cursor: pointer;
}

.job-filter form .dropdown-container .dropdown .lists .items:hover{
    background-color: var(--light-color);

}

.job-filter form .dropdown-container .dropdown .lists:hover,
.job-filter form .dropdown-container .dropdown:hover .lists,
.job-filter form .dropdown-container .dropdown .output:focus + .lists,
.job-filter form .dropdown-container .dropdown .output:focus-within + .lists{
    transform: scaleY(1);
    transition: 2s linear;
}

.job-details .detail{
    background-color: var(--white);
    border-radius: .5rem;
    border: var(--border);
    padding: 2rem;
    box-shadow: var(--box-shadow);
}

.job-details .detail h3{
    margin-bottom: 1rem;
    font-size: 2rem;
    color: var(--black);
    text-transform: capitalize;
    overflow-x: hidden;
}

.job-details .detail .job-info a{
    display: block;
    font-size: 1.6rem;
    color: var(--main-color);
}
.job-details .detail .job-info a:hover{
    text-decoration: underline;
}

.job-details .detail .job-info p{
    padding: 1rem 0;
    font-size: 1.6rem;
    color: var(--light-color);
    margin: .5rem 0;
}

.job-details .detail .basic-details{
    background-color: var(--light-bg);
    margin: 1.5rem 0;
    border-radius: .5rem;
    padding: 2rem;
    padding-bottom: 0;
}

.job-details .detail .basic-details p{
    color: var(--light-color);
    padding-bottom: 1.5rem;
}

.job-details .detail ul{
    margin: 1rem 0;
}

.job-details .detail ul li{
     padding: 1rem 0;
     font-size: 1.6rem;
     color: var(--light-color);
     margin-top: 1.5rem;
}

.job-details .detail .description p{
    font-size: 1.6rem;
    color: var(--light-color);
    line-height: 1.8;
    padding: .5rem 0;
}

.job-details .detail .save{
    background-color: var(--light-bg);
    border-radius: .5rem;
    padding: 1rem 1.5rem;
    cursor: pointer;
    font-size: 1.8rem;
    margin-top: 1rem;
}

.job-details .detail .save:hover{
    background-color: var(--black);
}


.job-details .detail .save i{
    margin-right: .5rem;
    color: var(--black);
}

.job-details .detail .save span{
    color: var(--light-color);
}

.job-details .detail .save:hover i{
    color: var(--white);
}

.job-details .detail .save:hover span{
    color: var(--white);
}

.view-company .detail{
    background-color: var(--white);
    box-shadow: var(--box-shadow);
    border: var(--border);
    background-color: var(--white);
    padding: 2rem;
}

.view-company .detail .info{
    max-width: 30rem;
    margin: 0 auto;
    border-radius: .5rem;
    background-color: var(--light-bg);
    padding: 3rem 2rem;
    text-align: center;
}

.view-company .detail .info img{
    height: 10rem;
    width: 10rem;
    object-fit: contain;
    margin-bottom: 1rem;
} 

.view-company .detail .info h3{
    padding: 1.5rem 0;
    font-size: 2rem;
    color: var(--black);
}

.view-company .detail .info p{
     font-size: 1.6rem;
     color: var(--light-color);
}

.view-company .detail .description{
    margin-top: 2rem;
}

.view-company .detail .description h3{
    font-size: 2.5rem;
    color: var(--black);
    padding: 1rem 0;
    text-transform: capitalize;
}

.view-company .detail .description p{
    padding: .5rem 0;
    font-size: 1.6rem;
    color: var(--light-color);
    line-height: 1.8;
}

.view-company .detail ul li{
    margin-left: 3rem;
    font-size: 1.6rem;
    color: var(--light-color);
    padding-top: 1.5rem;
}

.contact .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, 35rem);
    gap: 1.5rem;
    align-items: flex-start;
    justify-self: center;
}

.contact .box-container .box{
    background-color: var(--white);
    border: var(--border);
    border-radius: .5rem;
    box-shadow: var(--box-shadow);
    padding: 3rem 2rem;
    text-align: center;
}

.contact .box-container .box i{
    height: 4.5rem;
    width: 5rem;
    line-height: 4.5rem;
    font-size: 2rem;
    color: var(--white);
    background-color: var(--black);
    border-radius: .5rem;
    margin-bottom: 2rem;
}

.contact .box-container .box a{
    display: block;
    padding-top: .5rem;
    font-size: 1.6rem;
    color: var(--light-color);
    line-height: 1.5rem;
}

.contact form{
    margin-top: 2rem;
    background-color: var(--white);
    border: var(--border);
    border-radius: .5rem;
    box-shadow: var(--box-shadow);
    padding: 2rem;
    text-align: center;
}

.contact form h3{
    font-size: 2.5rem;
    color: var(--black);
    text-transform: capitalize;
    margin-bottom: 1rem;
}

.contact form .flex{
    display: flex;
    flex-wrap: wrap;
    column-gap: 1rem;
}

.contact form .flex .box{
    flex: 1 1 40rem;
}

.contact form .input{
    width: 100%;
    border-radius: .5rem;
    padding: 1.4rem;
    color: var(--black);
    font-size: 1.8rem;
    background-color: var(--light-bg);
    margin: 1rem 0;
}

.contact form p{
    text-align: left;
    font-size: 1.6rem;
    padding-top: 1rem;
    color: var(--light-color);
}

.contact form span{
    color: var(--red);
}

.contact form textarea{
    height: 15rem;
    resize: none;
}

.account-form-container{
    background: url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYJ19gKxubMAIzg9g7M9cqZRean-aIO1z7AQ&s'), rgba(0, 0, 0, .7) no-repeat;
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    background-blend-mode: color;
}

.account-form-container .account-form{
    min-height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
}

.account-form-container .account-form form{
    background-color: var(--white);
    border-radius: .5rem;
    padding: 2rem;
    width: 50rem;
    text-align: center;
}


.account-form-container .account-form form h3{
    font-size: 2.5rem;
    color: var(--black);
    text-transform: capitalize;
    margin-bottom: 1rem;
}

.account-form-container .account-form form .input{
    width: 100%;
    margin: 1rem 0;
    font-size: 1.8rem;
    padding: 1.4rem;
    background-color: var(--light-bg);
    border-radius: .5rem;
}

.account-form-container .account-form form p{
    padding: 1rem 0;
    font-size: 1.6rem;
    color: var(--light-color);
}

.account-form-container .account-form form p a{
    color: var(--main-color);
}

.account-form-container .account-form form p a:hover{
    color: var(--black);
    text-decoration: underline;
}














.footer .grid{
    display: -moz-grid ;
    grid-template-columns: repeat(auto-fit, 30rem);
    gap: 1.5rem;
    justify-content: center;
    align-items: flex-start;
}

.footer .grid .box h3{

     font-size: 2.5rem;
     color: var(--black);
     margin: 1rem 0;
     text-transform: capitalize;

}


.footer .grid .box a{

      display: block;
      padding: 1.5rem 0;
      font-size: 1.6rem;
      color: var(--light-color);

}


.footer .grid .box a i{
    color: var(--main-color);
    margin-right: .8rem;
    transition: 2s linear;
}


.footer .grid .box a:hover i{
    margin-right: 2rem;
}

.footer .credit{
    text-align: center;
    padding: 3rem 2rem;
    border-top: var(--border);
    background-color: var(--white);
    font-family: 2rem;
    color: var(--light-color);
    line-height: 1.5;
}

.footer .credit span{
    color: var(--main-color);
    text-transform: capitalize;
}







@media (max-width:991px){
    html{
        font-size: 55%;
    }

    .section-title{
        font-size: 5rem;

    }
}




@media (max-width:768px){

  #menu-btn{
    display: inline-block;
  }

  .header .flex .navbar{
    position: absolute;
    top: 99%; left: 0; right: 0;
    border-top: var(--border);
    background-color: var(--white);
    padding: 1rem .5rem;
    clip-path: polygon(0 0, 100% 0, 0 0);
  }

  .header .flex .navbar .active{
    clip-path: polygon(0 0, 100% 100%, 0 100%);
  }

  .header .flex .navbar a{
    display: block;
    padding: 1.5rem 2rem;
  }
  .category .box-container{
    grid-template-columns: repeat(auto-fit, 16.5rem);
  }

  .category .box-container .box{
    flex-flow: column;
    text-align: center;

  }

  .section-title{
    font-size: 4rem;
    padding: 4rem 2rem; 
    }
}

@media (max-width:450px){

    html{
        font-size: 50%;
    }

    .section-title{
        font-size: 3.5rem;
        
    }


}


------------------------------------------------------------------------------->> about.html <<------------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>About</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in
                    Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>

        <div class="section-title">about us</div>

        <section class="about">

            <img
                src="https://i.pinimg.com/736x/5c/71/2d/5c712dcf445d6c05097951bfce5142e9.jpg"
                alt>
            <div class="box">
                <h3>Actually, Why to Choose us?</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
                    eligendi excepturi tenetur, saepe quam totam dicta quibusdam
                    ab labore vitae suscipit debitis officiis, voluptas quod ex
                    numquam. Recusandae libero optio, fuga voluptatem dolorem
                    officia, eos nam ipsam, illo debitis aperiam eum tempora hic
                    pariatur perspiciatis nulla. Quod fugiat fugit rem?</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                    Dolor amet veniam quasi ut, harum totam recusandae inventore
                    quod perspiciatis ea modi animi fugiat, deserunt assumenda
                    repellat, eos iste beatae qui.</p>

                <a href="contact.html" class="btn">contact us</a>
            </div>

        </section>

        <div class="section-title">famous reviews</div>

        <section class="reviews">

            <div class="box-container">

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">absolutly amazing results</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSOY0kwRbxFsEeIC3dd3FIjrRkc5UUhrQ8i4UiRVFLb_ImO6FTQsGCtvEjLrjRD1Fw9Rk0&usqp=CAU" alt="">
                    </div>     
                    <div>
                        <h3>hitik kumar nayak</h3>
                        <span>web designer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">excelent results</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="data:image/jpeg;base64,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" alt="">
                    </div>     
                    <div>
                        <h3>aditya kuamr</h3>
                        <span>frontent developer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">easy to use</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="data:image/jpeg;base64,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" alt="">
                    </div>     
                    <div>
                        <h3>sunil gupta</h3>
                        <span>software developer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">supper</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSsPUPV0SxXNfBnLnhETvpfhfotyR3lGnvuGw&s" alt="">
                    </div>     
                    <div>
                        <h3>ranjeet sharma</h3>
                        <span>content writer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">its help me so much</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTelHfbWJLKtOCgGwcV6wzd_NYHS8prrITMsA&s" alt="">
                    </div>     
                    <div>
                        <h3>ajit goyal</h3>
                        <span>design engineering</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">best website I shown ever</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRTThYD6o6_SayVtWJPyfM_u9_Ox2EEYGV2YA&s" alt="">
                    </div>     
                    <div>
                        <h3>jyoti misha</h3>
                        <span>buisness analytics</span>
                    </div>
                </div>


            </div
        </section>

            <footer class="footer">
                <selection class="grid">

                    <div class="box">
                        <h3>quick links</h3>
                        <a href="home.html"><i class="fas fa-angle-right"></i>
                            home</a>
                        <a href="about.html"><i class="fas fa-angle-right"></i>
                            about</a>
                        <a href="jobs.html"><i class="fas fa-angle-right"></i>
                            jobs</a>
                        <a href="contact.html"><i
                                class="fas fa-angle-right"></i>
                            contact us</a>
                        <a href="#"><i class="fas fa-angle-right"></i> filter
                            search</a>

                    </div>
                    <div class="box">
                        <h3>extra links</h3>
                        <a href="#"><i class="fas fa-angle-right"></i>
                            account</a>
                        <a href="login.html"><i class="fas fa-angle-right"></i>
                            login</a>
                        <a href="register.html"><i
                                class="fas fa-angle-right"></i>
                            register</a>
                        <a href="#"><i class="fas fa-angle-right"> post
                                job</i></a>
                        <a href="#"><i class="fas fa-angle-right">
                                dashboard</i></a>

                    </div>

                    <div class="box">
                        <h3>follow us</h3>
                        <a href="#"><i class="fab fa-facebook-f"></i>
                            facebook</a>
                        <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                        <a href="#"><i class="fab fa-instagram"></i>
                            instagram</a>
                        <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                        <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                    </div>

                </selection>

                <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK
                        KUMAR
                        NAYAK</spaan> | all rights reserved! </div>

            </footer>

            <!-- custom js file link -->
            <script src="js/sc"></script>

        </body>
    </html>

    -------------------------------------------------->>about.html<<----------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>About</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in
                    Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>

        <div class="section-title">about us</div>

        <section class="about">

            <img
                src="https://i.pinimg.com/736x/5c/71/2d/5c712dcf445d6c05097951bfce5142e9.jpg"
                alt>
            <div class="box">
                <h3>Actually, Why to Choose us?</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut
                    eligendi excepturi tenetur, saepe quam totam dicta quibusdam
                    ab labore vitae suscipit debitis officiis, voluptas quod ex
                    numquam. Recusandae libero optio, fuga voluptatem dolorem
                    officia, eos nam ipsam, illo debitis aperiam eum tempora hic
                    pariatur perspiciatis nulla. Quod fugiat fugit rem?</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                    Dolor amet veniam quasi ut, harum totam recusandae inventore
                    quod perspiciatis ea modi animi fugiat, deserunt assumenda
                    repellat, eos iste beatae qui.</p>

                <a href="contact.html" class="btn">contact us</a>
            </div>

        </section>

        <div class="section-title">famous reviews</div>

        <section class="reviews">

            <div class="box-container">

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">absolutly amazing results</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSOY0kwRbxFsEeIC3dd3FIjrRkc5UUhrQ8i4UiRVFLb_ImO6FTQsGCtvEjLrjRD1Fw9Rk0&usqp=CAU" alt="">
                    </div>     
                    <div>
                        <h3>hitik kumar nayak</h3>
                        <span>web designer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">excelent results</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="data:image/jpeg;base64,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" alt="">
                    </div>     
                    <div>
                        <h3>aditya kuamr</h3>
                        <span>frontent developer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">easy to use</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="data:image/jpeg;base64,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" alt="">
                    </div>     
                    <div>
                        <h3>sunil gupta</h3>
                        <span>software developer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">supper</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSsPUPV0SxXNfBnLnhETvpfhfotyR3lGnvuGw&s" alt="">
                    </div>     
                    <div>
                        <h3>ranjeet sharma</h3>
                        <span>content writer</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">its help me so much</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTelHfbWJLKtOCgGwcV6wzd_NYHS8prrITMsA&s" alt="">
                    </div>     
                    <div>
                        <h3>ajit goyal</h3>
                        <span>design engineering</span>
                    </div>
                </div>

                <div class="box">
                   <div class="star">

                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star"></i>
                    <i class="fas fa-star-half-alt"></i>
                </div>
                

                   <h3 class="title">best website I shown ever</h3>
                   <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.
                    Impedit aspernatur officia sit fugiat, odit enim.</p>
                    <div class="user">
                         <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRTThYD6o6_SayVtWJPyfM_u9_Ox2EEYGV2YA&s" alt="">
                    </div>     
                    <div>
                        <h3>jyoti misha</h3>
                        <span>buisness analytics</span>
                    </div>
                </div>


            </div
        </section>

            <footer class="footer">
                <selection class="grid">

                    <div class="box">
                        <h3>quick links</h3>
                        <a href="home.html"><i class="fas fa-angle-right"></i>
                            home</a>
                        <a href="about.html"><i class="fas fa-angle-right"></i>
                            about</a>
                        <a href="jobs.html"><i class="fas fa-angle-right"></i>
                            jobs</a>
                        <a href="contact.html"><i
                                class="fas fa-angle-right"></i>
                            contact us</a>
                        <a href="#"><i class="fas fa-angle-right"></i> filter
                            search</a>

                    </div>
                    <div class="box">
                        <h3>extra links</h3>
                        <a href="#"><i class="fas fa-angle-right"></i>
                            account</a>
                        <a href="login.html"><i class="fas fa-angle-right"></i>
                            login</a>
                        <a href="register.html"><i
                                class="fas fa-angle-right"></i>
                            register</a>
                        <a href="#"><i class="fas fa-angle-right"> post
                                job</i></a>
                        <a href="#"><i class="fas fa-angle-right">
                                dashboard</i></a>

                    </div>

                    <div class="box">
                        <h3>follow us</h3>
                        <a href="#"><i class="fab fa-facebook-f"></i>
                            facebook</a>
                        <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                        <a href="#"><i class="fab fa-instagram"></i>
                            instagram</a>
                        <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                        <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                    </div>

                </selection>

                <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK
                        KUMAR
                        NAYAK</spaan> | all rights reserved! </div>

            </footer>

            <!-- custom js file link -->
            <script src="js/sc"></script>

        </body>
    </html>

    --------------------------<<    contact.html   ---------------------------------------------------------------------------------
    

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Content Us</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>
















<div class="section-title">contact <i class="fa fa-users" aria-hidden="true"></i></div>






  <section class="contact">

       <div class="box-container">
          
          <div class="box">
            <i class="fas fa-map-marker-alt"></i>
                <a href="#">418-1 Terabun, Kamakura, Kanagawa 247-0064, Japan</a>
          </div>

          <div class="box">
            <i class="fas fa-phone"></i>
            <a href="tel:1234567890">123-456-7890</a>
            <a href="tel:1111222255">111-122-2255</a>
          </div>

          <div class="box">
            <i class="fas fa-envelope"></i>
            <a href="mailto:hitiknayakkumar@gmail.com">hitiknayakkumar@gmail.com</a>
            <a href="mailto:nayakranjan@gmail.com">nayakranjan@gmail.com</a>
          </div>

       </div>

       <form action="" method="post">
        <div class="flex">
            <div class="box">
                <p>name <span>*</span></p>
                <input type="text" name="name" required maxlength="20" placeholder="enter your name" class="input">
            </div>
            <div class="box">
                <p>email <span>*</span></p>
                <input type="email" name="email" required maxlength="50" placeholder="enter your email" class="input">
            </div>
            <div class="box">
                <p>number <span>*</span></p>
                <input type="number" name="number" min="0" max="9999999999" required maxlength="50" placeholder="enter your number" class="input">
            </div>
            <div class="box">
                <p>role <span>*</span></p>
                <select name="role" required class="input">
                    <option value="employee">job seeker (employee)</option>
                    <option value="employee">job provider (employee)</option>
                </select>
            </div>
        </div>
        <p>message <span>*</span></p>
        <textarea name="message" class="input" required maxlength="1000" placeholder="enter your message" cols="30" rows="10"></textarea>
        <input type="submit" value="send message" name="send" class="btn">
       </form>

  </section>
























          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>
        
    </body>
</html>




    
    --------------------------<<    home.html   ------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Home</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opportunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>




            




          <div class="home-container">
            
              <section class="home">
            
                  <form action="" method="post">
                      <h3>find your next job</h3>
                      <p>job title <span>*</span></p>
                      <input type="text" name="title" placeholder="keyword, category or company" required maxlength="20" class="input">
                      <p>job location</p>
                      <input type="text" name="location" placeholder="city, state or country" required maxlength="50" class="input">
                      <input type="submit" value="search job" name="search" class="btn">
                  </form>

              </section>

          </div>

          <section class="category">
            <h1 class="heading">job categories</h1>

            <div class="box-container">
                <a href="#" class="box">
                          <i class="fas fa-code"></i>
                          <div>
                            <h3>development</h3>
                            <span>2200 jobs</span>
                          </div>
                </a>
                <a href="#" class="box">
                          <i class="fas fa-pen"></i>
                          <div>
                            <h3>designer</h3>
                            <span>500 jobs</span>
                          </div>
                </a>
                <a href="#" class="box">
                          <i class="fas fa-holding-dollar"></i>
                          <div>
                            <h3>finance</h3>
                            <span>1000 jobs</span>
                          </div>
                </a>
                
                <a href="#" class="box">
                          <i class="fas fa-person-digging"></i>
                          <div>
                            <h3>labour</h3>
                            <span>1560 jobs</span>
                          </div>
                </a>
                <a href="#" class="box">
                          <i class="fas fa-headset"></i>
                          <div>
                            <h3>services</h3>
                            <span>760 jobs</span>
                          </div>
                </a>
                
                <a href="#" class="box">
                          <i class="fas fa-chalkboard-user"></i>
                          <div>
                            <h3>teacher</h3>
                            <span>5000 jobs</span>
                          </div>
                </a>
                <a href="#" class="box">
                          <i class="fas fa-wrench"></i>
                          <div>
                            <h3>engineer</h3>
                            <span>330 jobs</span>
                          </div>
                </a>

            </div>
          </section>




          <section class="jobs-container">
            <h1 class="heading">latest jobs</h1>
            <div class="box-container">

                    <div class="box">
                        <div class="company">
                            <img src="https://w7.pngwing.com/pngs/805/822/png-transparent-process-engineering-logo-design-engineer-engineer-people-logo-engineering.png" alt="">
                            <div>
                                <h3>Tesla co.</h3>
                                <p>1 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Design engineer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>KamaKura, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>10k- 25k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>flexible shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4rfqzNpIJgf_qL4ylXzfSuJx-GYMrQdjI5cmmeUiXlA&s" alt="">
                            <div>
                                <h3>Apple co.</h3>
                                <p>3 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">software developer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Tokyo, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>11k- 30k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>
                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1xI0IZeJ6mEM8jEZfKHuauDv0m7Qa8l3lSQ&s" alt="">
                            <div>
                                <h3>Toyota co.</h3>
                                <p>5 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Marketing Specialist</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Yokohama, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>16k- 27k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ453NVHG7vKcIx4jWtq8rgaXnXinQv3sJPOCnNc2NjHg&s" alt="">
                            <div>
                                <h3>ÆON co.</h3>
                                <p>7 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Store Manager</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Fukushima, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>

                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTaPiViFNR1RIJfCHVWRJKfdRZDK1znvghsQcNyDbkLpw&s" alt="">
                            <div>
                                <h3>Panasonic co.</h3>
                                <p>8 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Supply Chain Manager</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Osaka, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>



                    <div class="box">
                        <div class="company">
                            <img src="data:image/jpeg;base64,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" alt="">
                            <div>
                                <h3>Sony co.</h3>
                                <p>9 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Graphic Designer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Hamamatsu, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>19k- 24k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>
                    
                     
            </div>

                   <div style="text-align: center; margin-top: 2rem;">
                    <a href="jobs.html" class="btn">view all</a>
                   </div>


          </section>













          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <script src="js/sc"></script>
        
    </body>
</html>

    
    --------------------------<<    jobs.html   --------------------------------------------------------------------------------------------------------

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Job</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>








 



        <section class="job-filter">

            <h1 class="heading">filter jobs</h1>

            <form action="" method="post">
                <div class="flex">
                  <div class="box">
                      <p>job title <span>*</span></p>
                      <input type="text" name="title" placeholder="keyword, category or company" required maxlength="20" class="input">
                  </div>
                  <div class="box">
                    <p>job location</p>
                    <input type="text" name="location" placeholder="city, state or country" required maxlength="50" class="input">
                  </div>
                </div>
                <div class="dropdown-container">
                        
                        <div class="dropdown">
                            <input type="text" readonly placeholder="date posted" name="date" maxlength="20" class="output">
                            <div class="lists">
                                <p class="items">today</p>
                                <p class="items">3 days ago</p>
                                <p class="items">7 days ago</p>
                                <p class="items">15 days ago</p>
                                <p class="items">30 days ago</p>
 
                            </div>
                        </div>


                        <div class="dropdown">
                            <input type="text" readonly name="date" placeholder="work shifts" maxlength="20" class="output">
                            <div class="lists">
                                <p class="items">day shift</p>
                                <p class="items">night shift</p>
                                <p class="items">flexible shift</p>
                                <p class="items">fixed shift</p>
 
                            </div>
                        </div>


                        <div class="dropdown">
                            <input type="text" readonly name="date" placeholder="education level"  maxlength="20" class="output">
                            <div class="lists">
                                <p class="items">10th pass</p>
                                <p class="items">12th pass</p>
                                <p class="items">bachelor's degree</p>
                                <p class="items">master's degree</p>
                                <p class="items">diploma</p>
 
                            </div>
                        </div>


                        <div class="dropdown">
                            <input type="text" readonly name="date" placeholder="job type"  maxlength="20" class="output">
                            <div class="lists">
                                <p class="items">full-time</p>
                                <p class="items">part-time</p>
                                <p class="items">internship</p>
                                <p class="items">contract</p>
                                <p class="items">temperary</p>
                                <p class="items">fresher</p>
 
                            </div>
                        </div>

                        <div class="dropdown">
                            <input type="text" readonly name="date" placeholder="estimated salary"  maxlength="20" class="output">
                            <div class="lists">
                                <p class="items">1k or less</p>
                                <p class="items">1k - 5k</p>
                                <p class="items">5k - 10k</p>
                                <p class="items">10k - 20k</p>
                                <p class="items">20k - 30k</p>
                                <p class="items">30k - 40k</p>
                                <p class="items">40k - 50k</p>
                                <p class="items">50k - 1 lakh</p>
                                <p class="items">1 lakh -5 lakh</p>
                                <p class="items">5 lakh - 10 lakh</p>
                                <p class="items">10 lakh - 20 lakh</p>
                                <p class="items">20 lakh - 50 lakh</p>
                                <p class="items">50 lakh - 1 crore</p>
                                <p class="items">1 crore - 5 crore</p>
                                <p class="items">5 crore - 10 crore</p>
                                <p class="items">10 crore or more</p>
 
                            </div>
                        </div>



                </div>
            </form>

        </section>











        <section class="jobs-container">
            <h1 class="heading">all jobs</h1>
            <div class="box-container">

                    <div class="box">
                        <div class="company">
                            <img src="https://w7.pngwing.com/pngs/805/822/png-transparent-process-engineering-logo-design-engineer-engineer-people-logo-engineering.png" alt="">
                            <div>
                                <h3>Tesla co.</h3>
                                <p>1 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Design engineer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>KamaKura, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>10k- 25k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>flexible shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4rfqzNpIJgf_qL4ylXzfSuJx-GYMrQdjI5cmmeUiXlA&s" alt="">
                            <div>
                                <h3>Apple co.</h3>
                                <p>3 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">software developer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Tokyo, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>11k- 30k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>
                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1xI0IZeJ6mEM8jEZfKHuauDv0m7Qa8l3lSQ&s" alt="">
                            <div>
                                <h3>Toyota co.</h3>
                                <p>5 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Marketing Specialist</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Yokohama, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>16k- 27k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ453NVHG7vKcIx4jWtq8rgaXnXinQv3sJPOCnNc2NjHg&s" alt="">
                            <div>
                                <h3>ÆON co.</h3>
                                <p>7 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Store Manager</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Fukushima, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>

                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTaPiViFNR1RIJfCHVWRJKfdRZDK1znvghsQcNyDbkLpw&s" alt="">
                            <div>
                                <h3>Panasonic co.</h3>
                                <p>8 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Supply Chain Manager</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Osaka, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>



                    <div class="box">
                        <div class="company">
                            <img src="data:image/jpeg;base64,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" alt="">
                            <div>
                                <h3>Sony co.</h3>
                                <p>9 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Graphic Designer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Hamamatsu, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>19k- 24k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>
                    
                 
       
                      
                    <div class="box">
                        <div class="company">
                            <img src="data:image/jpeg;base64,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" alt="">
                            <div>
                                <h3>Honda Co.</h3>
                                <p>11 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Manufacturing Engineers</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Yokohama, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>19k- 27k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="data:image/png;base64,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" alt="">
                            <div>
                                <h3>Nissan Motors Co.</h3>
                                <p>19 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">IT support specialists</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Kyoto, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 21k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>full-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>
                       
                    <div class="box">
                        <div class="company">
                            <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wCEAAkGBxINEBIODQ8PDQ0PEA8NDg0ODQ8ODw0NFhEWFhURGBUYHSgsGBolGxYWIjEhJSkrMC4uGB8zODMsNzQuLjcBCgoKDg0OGhAQGC0mICYtKy0tKy4tLS0tLS0tLS0tLy0tKy0tLS0tLS8tLS0tLy0tKy0tLS0tKy4tLS0tLSsuNf/AABEIAOEA4QMBEQACEQEDEQH/xAAbAAADAAMBAQAAAAAAAAAAAAABAgMABQYHBP/EAEIQAAICAQIDBQQHBAYLAAAAAAECAAMRBBIFBiETMUFRcQciYZEUMlJigaGxI0LB0TVykqLw8RUkJTM0U3SCs8Lh/8QAGgEBAQADAQEAAAAAAAAAAAAAAAEDBQYEAv/EADMRAQACAQIFAQUGBgMAAAAAAAABAgMEEQUSITFBURMicYGxFDJhodHhBiNCkcHwM1Lx/9oADAMBAAIRAxEAPwDu1J8z8zKiq58z84Flz5n5wKqD5wHAMBwIU4EBtsAhYBCyAhYGbYBCwM2wBtgZtgDbAG2ANsDNsAbYCkQEIgIQZQjZ8/zhEmz5n5wJNnzPzMCLE+Z+ZgHJ8z8zAoqwKqsCyrAsqwHCwpwsBwsBtsA7YDBZAQsDNsA7YGbYA2wM2wBtgDbAG2ANsAbYAKwJlYCFZQjLIiTLKIssCLLAG2BZRAqogWVYFlEBwIVQCA4WA2IBAkDBYBAgZiAQIGYgDEAbYGbYA2wBiAMQBiApEBCsBCIE2EIkwlEWECLCAMQKoIFlECyCBZRAcCFUAgOBAbEgIEA4gECAcQDiBmIAxAGIAxAzEAYgDEAYgKRAQiBNhARhCIuJRFhAi4gLiBVRAsogWQQLKIFAIU4EBwJA+IBxAOIBAgHEDAIBxAGIAxAGIAxAGIAxAzEBSIEyICEQJsIRJxKIsIEXEBcQKLAskCyQLLAoIU4EBwJA+IBAgECAQIBxAzEA4gDEAYgDEAYgDEAYgZiApgTMBCIRNoEXlEXgReAIDrAskCyQLLAoIU4gOJA8AiAYDCBkAiBkAQBAEAQMgCAICmBNoCNCJtAk8oi8CDQFgUSBZIFkgWWBQSKYSigkDQCIDQCIGQEvvWpS9jrWi9S7sFUD4ky1rNp2rG8m8Q57V89aGo4FrWkf8qtmH9o4B+c2OPhOqv8A07fFinNSHz1e0LRMcHt0Hm1OR/dJn3bguqj0n5p9oo3vDeM6fV/8PfXacZKA4cDzKHqPlPDm02bD/wAlZj6f3ZIvWe0vumB9BAEAQBAVoCGAhhE2gSeUQeBFoCwHSBZIFkgWWBQQpxAoJA0AiAYDCBpOaeY6+HV5Ydpe+eypBwWP2ifBR5z2aLRX1V9o6R5n/fLHkyRSHA6Pheu48/bXWbKATh3BFS+Yrr8fX5mb/Jn0vDq8lI3t+fzn/DzRW+XrPZ1uh9nujrH7XtdQ3iXsKDPwCY/PM1WXjOpvPuzEfD92aNPSH0Xci6BhgUFD5pdaCPzmKvFtXE/f/vEPr2NPRzXGPZ7ZT+14fczlPeFbkJaD91xjJ+XrNlp+NUv7mevz8fOGK2CY61lblXnhlcaTiR2uW7JL3Gxg/dssHh16bvn5z413Co5fbafrHeY/D1j9H1iyzPu2egzn3oCAIAgK0CbQEaETaBJ5RF4EHgLAdIFkgWSBZYFBCnECgkDQCIBgT1WoWmt7bDhK1Z2PkoGTPqlJvaKx3lJnaHlvBNE/Hdc9+oz2CEPYMnpXk9nQPLuOfxPeZ1Opy14fpox4/vT9fMvHSJy23ns9WqrCKFQBVUBVVRgKAOgAnKzMzO8va43mPnc02NRo0Sx0JWy6zJRXHeqgfWI8Tn5zzZM8V6Q3mi4P7WntMs7RPaPOy+l5ltBBtVHU4yFBRh6dYjN6vnLw3H/RMx8XUabULagsQ5Vhkfy9Znid2ovSaWmtnD+0/lZdTS2tpX/WaF3WgD/f0AdcjxZR1HwBHlN5wbiE4cnsrz7s/lLBeu/V9Hsw5gOt0xptbdfpdqFicmyg/UY+ZGCD6A+M+OM6KNPm5qx7tvr5haW3h2U077CAICtAm0BGhE2gSeUReBB4CwHSBZIFkgWWBQQpxAoJA0AiBjttBY9wBJ9AJYjednza0ViZnw82504m9lLbmOLHVAueir1bH5TpOG6etckdOzl8GoyanUc156RvtD6uQLjp6k+zc5Zx+O1T8gJi4rX2t5/Bnrrr49Xy7+70jZ3mtZlqsZPrrW5X+sFOPznPT2dNjiJvET6vE6u7z6d/fn4zUz1d/O3h1yHoPQT0Q0893T8qMezceAfp6lRn+E9WGejTcSiPaRP4Ic5cTalFqqJVrQ25x3isdMDyznv+E9eGu87ta8f4Sx0+sKISmC6KVJUgDquCPQTrtdtn0MXnv0n/AAxV6Wezcp8UbVUHtDm2ttjN9sYyG9f5Tj8leWWZupjAgK0CbQEaETaBJ5RF4EHgLAdIFkgWSBZYFBCnECgkDQCIGOoYFT3EEH0MsTt1fNqxaJiXl/POheitVcHAtG1vBhtbB/8Ak6fheauS28ejnNPpr6fPNbenSfVtuSNG19VLYxWn1m8CVY+6PxE8nEssUvaPMri0Vsuqm0x7sTu72aJ0jy3m7ga6OwtVZWa3JZad4FtefDb4r8f854M2KKzvDreG62c9OW8TvHnxP7tho6u0KoGVM4952CqJ9Vruw5b8kTO27uOH6QUViteuOpb7THvM9lY5Y2hzubLOW82lpucOFPqEWykF3q3AoPrMhx3eZGO74zPhvyz1YZeQUo1nENqKzN2jDaFJYkIQRj1nW5Pc4b19I+rFH3nsvKnC20lJFnS2xt7r37BjAX1/nOQyW5pZm5mMCArQJtARoRNoEnlEXgQaAsB0gXSBZIFlgUEKcQHEgaAwgarjvFfoyhUwbWGRnqEX7R/hPTpsHtJ3ns1vENd9njlr96fycNxkNqa3DMXcjcCxydwOQJvdNy4rxMR0aDFnv7WL3ndruUeLPQTWjlGB3qPBh+8pHjPTxDTVye9MNjqLXxWjJSXS8w887Klr0426px+0bGRQPMZ7yfDynH6z+TbkiXYcD0n23HGfJG1fT1n9HBvcXJZ2LMxyzMSWY+ZJ75rJ69XYRWKxtEbQ61D0HoJmame8txwXjLUEI5LUnoR3mv4j4fCZqX2naXi1WkjJHNXv9Wo5r5rZw+wmuhchUB2tafDd6+U3Wj0ntb1rHXdoLTy7xLieWaiXe9vioPm5OSf8ec33F8kUx1wx/sQx0jru9F5d5kathVqGL1HoHY5ao+viv6TmcmKJ6wyu3nlUIAMCbQJtCEaBF5RF4EWgLAdIFkgWSBZYFBCnEBxIHgEQOI5iRl1D7zndhlP3MdB+Hd+E3OkmJxxs5DiVL11Npt57fBotfrVoXe/oqjvdvIT34sc5J2hiw4pyTtDjrdeVc2nCOWLqF6DPlN1XFHJyT1b6mLevJKdet7QkuffY5PxM4rivB8+C85K+9Weu/mPi77hfEMFsVcMRyzEbbfo+kPNA3Ts626D0H6TM0895S1euShd9rhR4ebfADxnp02ky6i/Ljrux5c9MUb2lxmv1T6+7Fa7K85AP7o+23x+E7fS6enDcG953t/vSHM6nL7fJNqxtDeaWkVKEXuH5nxM0OfNbNeb28vmI2fQrTCPTOWbHbS1Gzv24U+JrBwp+U8WTbm6PqGznwFaBNoCNCJtAi8oi8CLwFgOkCyQLJAssCghTiA4kDwCIHO88WU1aftrW22KcVAdWtY99YH558JsOHVyXy8lI+P4fi1/ENLXNTftMdnj3ENaXY2WHJ7lUdyjyH852WHDFI5YYMGCKV5atS5LnJ/ymPXa3Ho8XNbv4j1luNDob6m/JTt5n0UNIPd0nN6b+JMlZ2zV3ifTx+rodRwDHMROK20x69f8AwRvXuJx65nunUcI1XW8RE/jG0vDGDien6V3mPjvDbi3Xv0HaAfBa06esvs+D4+u9Z+cy88219um0/Q+m5cttbfqbMefvGyw/DJ7vznxm4/gw15dNT8tofWPhmW875bf5l0I0KVUlKlCgYfzLEd5J8Tic9Osy588Xy23+j3ajS46aea0jt1fEJ7Ghbvlrgjax8sCNOh/aP3bvuD4/p8piyZIrCvSFUKAFAAAAAHQADuE8ajAVoE2gI0Im0CLyiLwIvAWA6QLJAskCywKCFOIDiQPA1/HOMVaCo3XH4JWPr2v4KP5+E9Gm02TUX5KR+z5veKxvLxjmLjtmssN95691dYPu1p9lf4nxnaaPR009OSnzn1l4Zmck7y+bl3gN/Fb+zq91Rg23Ee5Sn8SfAePzM+9ZrMekx81u/iPVmrTptDZc48sXaEVhaHbTorZvrU2KWJHViO49PHE4vieq+1Wrb4ug/hv+V7SMto3mY2+Eejlksz3HM1Uw6tUWT52Hc1v0HoP0mTZqZ7qq0myw+mus2AoqlmYEBVBJOR5CfVOlofGeY9nbmnxLZ8G5Nd8Pqz2ad/ZKQXb1I+r+vpNhfN/1crs7XT0LUorrUIijCqowAJ5pndTwBAVoE2gI0Im0CLyiLwIvAWA6QLJAskCywKCFOIDiQPA8K5l46+rta64nGStVfhXXnooH6md3otJTBjitfnPq8FpnJZ8nLnAbuK39nX7qDBuuIJSlP4sfAePpkzJrNbj0mPmnv4j1/ZmpTw904HwerQUrp9Ou1F6lj1ex/F2PiTOG1GoyajJN7z1eiI2hsMTCrScT5R0OrJa7SVFz32IDS5/7kIMk1iXqxa3Pi+7efr9Wiv8AZboW+o+qq+CXIw/vqf1nzyQ9leNaiO+0/JsU5KoHTtbyB076x/6xyQwzxLJPiH2aflbTJ3o1hH27G/QYl5IY7a/NPnZtKNMlQxWioPJVCz622eW17Wne07qQ+WQBAEBWgTaAjQibQIvKIvAi8BYDpAskCyQLLAoIU4gOJA4gcPxn2aUaq5rkvt04clnqVUdcnqdhP1fxzN3p+OZcOOKTWJ27Sx+zjw+/jWto5Z4a11NDWVUtWGQOFstd2C72Yjqf8dJq9RqMmovN8k7y+4iIbriXFhp9FbrihZadK+rNQbBYLWX2Z/DGZgVzmu9oaU6DQ8ROmdl4hdXp1qFqg1F9+GLY6/U/ONhvOceYBwnRW656mvWk1g1qwQtusVO8/wBbMDTc3c/JwvS6TVHTPedaAy1JYFZB2Qc9SOuM4jYbjXcy008OPFeracaZdWoBALhlBRM+BJIHqYHzci81rxnTvqFpfTdnc+nap3DtuVVOcgD7Xd8IGqHtHpPFf9Fdg+3tzpBrd69kdSKt/Z7cd+73e/vjYbDn7m9eCUV6h6G1Pa3dgESwVkHs3fOSD9n84FddzZTXwxuL0qb9OKV1CoGCMwJAKE9cMCSD8QYG14TrRqtPTqQpQX01XhCclA6BtufHGYH1QFaBNoCNCJtAi8oi8CLwFgOkCyQLJAssCghTiA4kDwCIHBe3L+hL893a6XPp2ywNJxzQ8dHDL2v1vDm0Y0NrW1pRYLW03YHcoO3623pnzlGl5g6cu8CY/VTW6dmbwVf23Uy+R3fttcDgmqyQMtpwPifpCSR3Gh5p03barlrSWD3Xp1AtQ+X0WkH8t0DQcFvs1el0PLVrZuo4tdRrBjO7Q6Ru1IP3SSAD9yB0vs14mmi0/HbrOiaXievvYfdVc4H9nEg88bWsOEpaNHxAcRXiJ42dedG/0I2F8ZF2fq7QpzjGfnKPRPabr01ml4Lqa8Gu/inD7lB6jayMcH54kHM8xq3BK+K8EfP0HWUWa7hbEnCMHU2acfI9Pug97Sj1zlD+jtD/ANDo/wDwJINtAVoE2gI0Im0CLyiLwIvAWAyQLJAukCywHEKoIDiQNAIgabnHlxOL6N9FbY9KWNWxesAsNjhh3+kC/GdFU+ht0d9wppt07aNrmZV2h6ymfe6Z+EDUajlTRjhVfCNXaG0wVa67rLEqsLhiyup7tw/PxGIGnHs5rZ9PTxLi2r19FTbtPw/UWVqtuwfvDvsAH5ZHdmUdHxPgNOq4jo9Y1+3UcPS5k0ylPfS1dhZh3gSCXDuVNLRxO/itbk6nUqaTUWQ1owCbyoAzuPZjPqfOBqG5B09tXEtJVrnH+kdWNXqRX2TWUN2pfswPAE4HXwEo6Wzh+mfR2cN3J9HTTfQ7UV1zTSatgz9k7Rn8JBzNfJOmPD9Hpjr2s03DtWNbVqS1RB2sx7NmzgKCxHw6CUbjnTlOjjmnSq5ymxxdTqKtrMoI6gZ6FWGPkD4SDccK0Y0tFOmVi60U1UKzYBYIgUMceJxA+mArQEaBNoQjQIvKIvAi0BYDJAskCyQLLAoIU4gUEgaARA+Ti9N9lLJpLl02oJXZc9QuVQGBYbD35GR+Msbb9R83MVNjrSKdos+kIQz1m1F/Zv1ZQR0/HxlqNbjs6eGld9KVoFO+lrmrH0fGxgB0Phnp1l9UbDV/s9bW9QZrLUSi9DU7KunXtXS0PjCEMzA9eu4DvxPmOyvirqP0wLsftF11upezs2CnSnRlFO/GCMlFxnvX4T68BtEp+l7Njg16jV3sxrcJ2b1qFIfGDncOgPg3kZJ7BeCad11jvYp2seIdiRWy7AdWhYO37273Cvd0Dd/fLbsDox/s66jYw1CafUJehrdWfUFX3MDj39zZYEZzukn7wrYFs0S77iCjVutq6V/dtRgy5pxlhkAHz8weseR9T/SL9GDUV0WtspRgWrFq6e0qCw2nvx1HWOkSNggIADHc2AGIGATjqceE+QYCtAm0BGhE2gSeUReBBoCwHSBZIFkgWWBQQpxAcSB4BEAiARAOYGQDAEAQBmAMwBAEDICtAm0BDCJtAi8oi8CLwFgMsCywLLAssCghTiA4gPICIBEBhAyARAyAIAgCAIGQBAEBTAmYCGETaBJ5RF4EHgLCmUwiywLIYFlMBwYVQGA4MBsyA5gNmAQYGZgHMDMwBmAMwMzAGYAzAGYAzAUmAhMCZMBGMIi5lEWMCLGAuYBUwLIYFlMCymBQGFODAcGQNmAQYDAwDmAcwMBgZmBmYAzAGYAzAGYAzAGYCkwEJgTJhCMYEWMoixgRcwFzAxTAspgWQwLKYDgwpwYFAYDAyAgwCDAIMA5gHMDMwBmAMwMzAGYAzAGYAzAUmBMmAhMIRjAixlEWMCLmAMwFVoFlaBZWgWVoDhoU4aA4aA+6QENAIaAd0A7oGboGboGboA3QBugDdAG6AN0DN0BS0CZaAhaAjNKiLNAkzQIu0Bd0BFaBVGgWVoFlaA4eFOHgOGgMGgENAIaQMGgZugENAzdAG6AN0AboGb4A3QBugDdAUtAQtAQtKEZpERZpRJ2gRZoGboH1CA4gUWFOIQwhTCAwgGQEQMEAwMgGBkDIAgCBkAQMgZAUwBAQyhTIhGhUzKhDCjCP/9k=" alt="">
                            <div>
                                <h3>Hitachi, Ltd.</h3>
                                <p>18 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">HR roles</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Nagoya, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>

                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQDIOlVbV61mCVxB7qXhyJOPoWT5B9Lm9a7HW01pUb_F4ciKx7wG-CRYaNLOj3eCS4z-5o&usqp=CAU" alt="">
                            <div>
                                <h3>Kawasaki Heavy Industries, Ltd.</h3>
                                <p>8 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Aircraft Designer</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Kobe, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>fixed shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>


                    <div class="box">
                        <div class="company">
                            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTaPiViFNR1RIJfCHVWRJKfdRZDK1znvghsQcNyDbkLpw&s" alt="">
                            <div>
                                <h3>Canon Inc.</h3>
                                <p>8 days ago</p>
                            </div>
                        </div>
                        <h3 class="job-title">Supply Chain Manager</h3>
                        <p class="location"><i class="fas fa-market-alt"></i>
                        <span>Osaka, Japan</span></p>
                        <div class="tags">
                            <p><i class="fas fa-yen-sign"></i>
                            <span>18k- 20k</span></p>
                           <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                           <p><i class="fas fa-clock"></i> <span>night shift</span></i></p>
                        </div>
                        <div class="flex-btn">
                            <a href="view_job.html" class="btn">view details</a>
                            <button type="submit" class="far fa-heart" name="save"></button>
                        </div>

                    </div>




                     
            </div>

             </section>











          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>

        <script>

             let dropdown_items = document.querySelectorAll('.job-filter form .dropdown-container .dropdown .lists .items');

             dropdown_items.forEach(items =>{
                   items.onclick = () =>{
                    items_parent = items.parentElement.parentElement;
                    let output = items_parent.querySelectorAll('output');
                    output.value = items.innerText;
                   }
             });

        </script>
        
    </body>
</html>

    
    --------------------------<<    login.html -------------------------------------------------------------------------------------------------------------

    <!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Login</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>











<div class="account-form-container">
    <section class="account-form">

        <form action="" method="post">
            <h3>welcome back!</h3>
            
            <input type="email" required name="email" maxlength="50" placeholder="enter your email" class="input">
            <input type="password" required name="pass" maxlength="20" placeholder="enter your password" class="input">
            <p>don't have an account? <a href="register.html">register now</a></p>
            <input type="submit" value="login now" name="submit" class="btn">
        </form>

    </section>
</div>













          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>
        
    </body>
</html>


    --------------------------<<    register.html----------------------------------------------------------------------------------------------------------

    <!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Register</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>














        <div class="account-form-container">
            <section class="account-form">
        
                <form action="" method="post">
                    <h3>create new account!</h3>
                    <input type="text" required name="name" maxlength="20" placeholder="enter your name" class="input">
                    <input type="email" required name="email" maxlength="50" placeholder="enter your email" class="input">
                    <input type="password" required name="pass" maxlength="20" placeholder="enter your password" class="input">
                    <input type="password" required name="c_pass" maxlength="20" placeholder="confirm your password" class="input">
                    <p>already have an account? <a href="login.html">login now</a></p>
                    <input type="submit" value="register now" name="submit" class="btn">
                </form>
        
            </section>
        </div>














          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>
        
    </body>
</html>




    --------------------------<<    script.js  -----------------------------------------------------------------------------------------------------------

    let navbar =document.querySelector('.head .flex .navbar');

document.querySelector('#menu-btn').onclick = () =>{
    navbar.classList.toggle('active');
}

window.onscroll = () => {
    navbar.classList.remove('active');
}

document.querySelectorAll('input[type="number"]').forEach(inputNumber => {
    inputNumber.oninput = () =>{
        if(inputNumber.ariaValueMax.length > inputNumber.maxLength) inputNumber.value = inputNumber.value.length.slice(0, inputNumber.maxLength);
    }; 
    
});


    --------------------------<<    view_company.html ---------------------------------------------------------------------------------------------------------------------

    <!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>View Company</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" class="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>


             <section class="view-company">

               <h1 class="heading">company detail</h1>

               <div class="detail">

                <div class="info">
                       <img src="https://w7.pngwing.com/pngs/805/822/png-transparent-process-engineering-logo-design-engineer-engineer-people-logo-engineering.png" alt="">
                       <h3>Tesla Co.</h3>
                       <p><i class="fas fa-map-market-alt"></i> KamaKura, Japan</p>
                </div>

                <div class="description">
                    <h3>about company</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur harum doloribus minus, delectus quisquam fugiat magnam similique eos quam? Minus cumque inventore deleniti reiciendis dolor magni iusto quisquam laborum perspiciatis.</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Debitis sed quibusdam dignissimos expedita, esse alias a nemo id! Itaque, totam!</p>

                </div>

                    <ul>
                        <li>4 jobs posted</li>
                        <li>established at 27-09-2003</li>
                        <li>367 working employess</li>
                    </ul>

               </div>


             </section>
            


























 
             
        
    
             <section class="jobs-container">
                <h1 class="heading">jobs they offer</h1>
                <div class="box-container">
    
                        <div class="box">
                            <div class="company">
                                <img src="https://w7.pngwing.com/pngs/805/822/png-transparent-process-engineering-logo-design-engineer-engineer-people-logo-engineering.png" alt="">
                                <div>
                                    <h3>Tesla co.</h3>
                                    <p>1 days ago</p>
                                </div>
                            </div>
                            <h3 class="job-title">Design engineer</h3>
                            <p class="location"><i class="fas fa-market-alt"></i>
                            <span>KamaKura, Japan</span></p>
                            <div class="tags">
                                <p><i class="fas fa-yen-sign"></i>
                                <span>10k- 25k</span></p>
                               <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                               <p><i class="fas fa-clock"></i> <span>flexible shift</span></i></p>
                            </div>
                            <div class="flex-btn">
                                <a href="view_job.html" class="btn">view details</a>
                                <button type="submit" class="far fa-heart" name="save"></button>
                            </div>
    
                        </div>
    
    
                        <div class="box">
                            <div class="company">
                                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4rfqzNpIJgf_qL4ylXzfSuJx-GYMrQdjI5cmmeUiXlA&s" alt="">
                                <div>
                                    <h3>Tesla co.</h3>
                                    <p>3 days ago</p>
                                </div>
                            </div>
                            <h3 class="job-title">software developer</h3>
                            <p class="location"><i class="fas fa-market-alt"></i>
                            <span>Tokyo, Japan</span></p>
                            <div class="tags">
                                <p><i class="fas fa-yen-sign"></i>
                                <span>11k- 30k</span></p>
                               <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                               <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                            </div>
                            <div class="flex-btn">
                                <a href="view_job.html" class="btn">view details</a>
                                <button type="submit" class="far fa-heart" name="save"></button>
                            </div>
    
                        </div>

                        <div class="box">
                            <div class="company">
                                <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1xI0IZeJ6mEM8jEZfKHuauDv0m7Qa8l3lSQ&s" alt="">
                                <div>
                                    <h3>Tesla co.</h3>
                                    <p>5 days ago</p>
                                </div>
                            </div>
                            <h3 class="job-title">Marketing Specialist</h3>
                            <p class="location"><i class="fas fa-market-alt"></i>
                            <span>Yokohama, Japan</span></p>
                            <div class="tags">
                                <p><i class="fas fa-yen-sign"></i>
                                <span>16k- 27k</span></p>
                               <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                               <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                            </div>
                            <div class="flex-btn">
                                <a href="view_job.html" class="btn">view details</a>
                                <button type="submit" class="far fa-heart" name="save"></button>
                            </div>
    
                        </div>

                        <div class="box">
                            <div class="company">
                                <img src="data:image/jpeg;base64,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" alt="">
                                <div>
                                    <h3>Tesla co.</h3>
                                    <p>9 days ago</p>
                                </div>
                            </div>
                            <h3 class="job-title">Graphic Designer</h3>
                            <p class="location"><i class="fas fa-market-alt"></i>
                            <span>Hamamatsu, Japan</span></p>
                            <div class="tags">
                                <p><i class="fas fa-yen-sign"></i>
                                <span>19k- 24k</span></p>
                               <p><i class="fas fa-briefcase"></i> <span>part-time</span></i></p>
                               <p><i class="fas fa-clock"></i> <span>day shift</span></i></p>
                            </div>
                            <div class="flex-btn">
                                <a href="view_job.html" class="btn">view details</a>
                                <button type="submit" class="far fa-heart" name="save"></button>
                            </div>
    
                        </div>
    
    

    
                      

                        
                         
                </div>

    
              </section>




















          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>
        
    </body>
</html>


    --------------------------<<    view_job.html -----------------------------------------------------------------------------------------------------------------------------------

    <!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>View Job</title>

        <!-- custom css file link -->
        <link rel="stylesheet" href="css/style.css">
    </head>
    <body>

        <header class="header">

            <section class="flex">

                <div id="menu-btn" class="fas fa-bars-staggered"></div>

                <a href="home.html" class="logo"><i
                        class="fas fa-briefcase"></i>Work Opertunity in Japan.</a>

                <nav class="navbar">
                    <a href="home.html">home</a>
                    <a href="about.html">about</a>
                    <a href="jobs.html">jobs</a>
                    <a href="contact.html">contact</a>
                    <a href="login.html">account</a>
                </nav>

                <a href="#" slot="btn" style="margin-top: 0;">post job</a>

            </section>
        </header>





           <section class="job-details">

                   <h1 class="heading">job details</h1>

                   <div class="detail">
                        <div class="job-info">
                             <h3>Design engineer</h3>
                             <a href="view_company.html">Tesla co.</a>
                              <p><i class="fas fa-map-market-alt"></i>KamaKura, Japan</p>
                        </div>
                            
                        <div class="basic-details">
                            <h3>salary</h3>
                                 <p>10000 - 25000 per month</p>
                            <h3>benefits</h3>
                                 <p>work from home, health insurances</p>
                            <h3>job type</h3>
                                 <p>part-time</p>
                            <h3>schedule</h3>
                                 <p>day shift</p>     
                        </div>
                        <ul>
                            <h3>requirements</h3>
                            <li>educatin : <span>graduate</span></li>
                            <li>age : <span>25+</span></li>
                            <li>language : <span>japanese, nihongo, english</span></li>
                            <li>experience : <span>3+ years</span></li>
                        </ul>

                        <ul>
                            <h3>qualification</h3>
                                <li>Bachlor's (Preferred)</li>
                                <li>PHP : 1year (Preferred)</li>
                                <li>CAD : 1year (Preferred)/li>
                                <li>Materials Science : 1year (Preferred)</li>
                                <li>total work : 3 years (Required)</li>
                        </ul>
                        <ul>
                            <h3>skills</h3>
                            <li>autoCAD</li>
                            <li>hybrid mesh generation</li>
                            <li>pointwise software proficiency</li>
                            <li>grid quality assessment</li>
                            <li>boundary conditions and solver requirements:</li>
                            <li>automation and scripting</li>
                        </ul>
                        <div class="description">
                            <h3>
                                <p>job description</p>
                                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laudantium cupiditate quae eos amet, sint ex molestiae. Earum, totam enim delectus incidunt vel ipsam eos officiis nostrum voluptate porro! Dolores, ut.</p>
                                <ul>
                                    <li>Hiring 5 candidate for this job</li>
                                    <li>posted 2 days ago</li>
                                </ul>
                            </h3>
                        </div>
                        <form action="" method="post" class="flex-btn">
                            <input type="submit" value="apply now" name="apply" class="btn">
                            <button type="submit" class="save"><i class="fas fa-heart"></i><span>save job</span></button>
                        </form>
                   </div>

           </section>






          
           <footer class="footer">
            <selection class="grid">
                
                <div class="box">
                    <h3>quick links</h3>
                    <a href="home.html"><i class="fas fa-angle-right"></i> home</a>
                    <a href="about.html"><i class="fas fa-angle-right"></i> about</a>
                    <a href="jobs.html"><i class="fas fa-angle-right"></i> jobs</a>
                    <a href="contact.html"><i class="fas fa-angle-right"></i> contact us</a>
                    <a href="#"><i class="fas fa-angle-right"></i> filter search</a>
                    
                </div>
                <div class="box">
                    <h3>extra links</h3>
                    <a href="#"><i class="fas fa-angle-right"></i> account</a>
                    <a href="login.html"><i class="fas fa-angle-right"></i> login</a>
                    <a href="register.html"><i class="fas fa-angle-right"></i> register</a>
                    <a href="#"><i class="fas fa-angle-right"> post job</i></a>
                    <a href="#"><i class="fas fa-angle-right"> dashboard</i></a>
                    
                </div>

                <div class="box">
                    <h3>follow us</h3>
                    <a href="#"><i class="fab fa-facebook-f"></i> facebook</a>
                    <a href="#"><i class="fab fa-twitter"></i> twitter</a>
                    <a href="#"><i class="fab fa-instagram"></i> instagram</a>
                    <a href="#"><i class="fab fa-linkedin"></i> linkedin</a>
                    <a href="#"><i class="fab fa-youtube"></i> youtube</a>
                </div>

            </selection>

        <div class="credit">&copy; copyright @2024 by <spaan>mr. HITIK KUMAR NAYAK</spaan> | all rights reserved! </div>

           </footer>



        <!-- custom js file link -->
        <script src="js/sc"></script>
        
    </body>
</html>









