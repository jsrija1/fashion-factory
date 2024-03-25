<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;300;400;500;600&display=swap");

:root{
    --main-color:#210464;
    --primary:#f0fff7;
    --black:#141414;
    --white:#fff;
    --bg:#f2f2f2;
    --light-black:#666;
}

*{
    font-family: 'Poppins', sans-serif;
    margin: 0; padding: 0;
    box-sizing: border-box;
    outline: none;
    border: none; text-decoration: none;
    text-transform: capitalize;
    transition: .2s linear;
}


html{
    font-size: 62.5%;
    overflow-x: hidden;
    scroll-behavior: smooth;
    scroll-padding-top: 6rem;
}

html::-webkit-scrollbar{
    width: 1rem;
}

html::-webkit-scrollbar-track{
    background: var(--white);
}

html::-webkit-scrollbar-thumd{
    background: var(--main-color);
}

section{
    padding: 3rem 9%;
}

.heading{
    text-align: center;
    color: var(--main-color);
    text-transform: uppercase;
    margin-bottom: 4rem;
    margin-top: 2rem;
    font-size: 4rem;
}


.btn{
    display: inline-block;
    margin-top: 1rem;
    padding: 1rem 3rem;
    border: .1rem solid var(--main-color);
    border-radius: .5rem;
    cursor: pointer;
    font-size: 1.7rem;
    color: var(--main-color);
}

.btn:hover{
    background: var(--main-color);
    color: var(--white);
}

/*header*/
.header{
    position: fixed;
    top: 0; left: 0;
    right: 0;
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 2rem 9%;
    background: var(--primary);
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0,0.1);
}

.header .logo{
    font-size: 2.2rem;
    font-weight: bolder;
    color: var(--main-color);
}

.header .navbar a{
    font-size: 1.7rem;
    margin-left: 2rem;
    color: var(--black);
}

.header .navbar a:hover{
    color: var(--main-color);
}

#menu{
    font-size: 2.5rem;
    cursor: pointer;
    color: var(--main-color);
    display: none;
}

.home{
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: url("images\1.jpg") no-repeat;
    background-size: cover;
    background-attachment: fixed;
}

.home .content{
    max-width: 60rem;
    text-align: center;
}

.home .content h3{
    font-size: 5rem;
    text-transform: unset;
    color: var(--black);
    padding-bottom: 3.5rem;
}

.about .row{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 2 rem;
}


.about .row .content{
    flex: 1 1 40rem;
}

.about .row .content h3{
    font-size: 3.5rem;
    color: var(--black);
    text-transform: uppercase;
}

.about .row .content p{
    font-size: 1.6rem;
    color: var(--light-black);
    padding: 2rem 0;
    line-height: 2;
}


.about .row .image{
    flex: 1 1 40rem;
}

.about .row .image img{
    width: 100%;
}

.services{
    background: var(--bg);
}

.services .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
    gap: 2rem;
    margin-top: 8rem;
}

.services .box-container .box{
    text-align: center;
    padding: 3rem;
    background: var(--white);
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0,0.1);
    border-radius: 1rem;
    margin-bottom: 8rem;
}

.services .box-container .box:hover,
.services .box-container .box:hover .icon{
    background: var(--primary);
}

.services .box-container .box .icon{
    width: 13rem;
    height: 13rem;
    line-height: 13rem;
    background: var(--white);
    border-radius: 50%;
    margin: -11rem auto 2rem;
    border: 1.8rem solid var(--bg);
}

.services .box-container .box .icon img{
    width: 5rem;
    margin-top: 2rem;
}

.services .box-container .box .content h3{
    font-size: 2rem;
    padding: 1rem 0;
    color: var(--main-color);
}

.services .box-container .box .content .line{
    background: var(--main-color);
    width: 30%;
    height: .4rem;
    margin: 2rem auto;
    border-radius: 5rem;
}

.services .box-container .box .content p{
    font-size: 1.4rem;
    color: var(--black);
    line-height: 2;
}

.services .box-container.box .content ul{
    margin: 2rem 0;
    list-style: none;
}

.services .box-container .box .content ul li{
    padding: .5rem;
    font-size: 1.4rem;
    color: var(--black);
}

.services .box-container .box .content ul li i{
    font-size: 1.4rem;
    columns: var(--white);
    padding: .5rem;
    margin-right: 1rem;
    background: var(--main-color);
    border-radius: 50%;
}

.newarrivals .controls{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
    gap: 1.5rem;
    list-style: none;
}

.newarrivals .controls .buttons{
    padding: 3rem 2rem;
    background: var(--white);
    cursor: pointer;
    margin-bottom: 3rem;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0,0.1);
    text-align: center;
    border-radius: 1rem;
}

.newarrivals .controls .buttons img{
    height: 6rem;
    width: auto;
}

.newarrivals .controls .buttons h3{
    font-size: 1.7rem;
    padding-top: 1rem;
    color: var(--light-black);
}

.newarrivals .controls .buttons .active{
    background: var(--primary);
}

.newarrivals .image-container .box{
    background: var(--white);
    border-radius: 1rem;
    box-shadow: 0 .5rem 1rem rgba(0, 0, 0,0.1);
    overflow: hidden;
}

.newarrivals .image-container .box:hover .image img{
    transform: scale(1.1);
}

.newarrivals .image-container .box .image{
    height: 25rem;
    overflow: hidden;
    width: 100%;
}

.newarrivals .image-container .box .image img{
    height: 100%;
    width: 100%;
    object-fit: cover;
}

.newarrivals .image-container .box .content{
    padding: 2rem;
}

.newarrivals .image-container .box .content .link{
    font-size: 2rem;
    color: var(--main-color);
}

.newarrivals .image-container .box .content p{
    padding: 1rem 0;
    font-size: 1.4rem;
    color: var(--light-black);
    line-height: 2;
}

.newarrivals .image-container .box .content .icon{
    padding-top: 1rem;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.newarrivals .image-container .box .content .icon a{
    font-size: 1.4rem;
    color: var(--light-black);
}

.newarrivals .image-container .box .content .icon a:hover{
    color: var(--main-color);
}

.newarrivals .image-container .box .content .icon a i{
    padding-right: .5rem;
    color: var(--main-color);
}


.newsletter{
    background: url() no-repeat;
    background-position: center;
    background-size: cover;
}

.newsletter .content{
    max-width: 70rcm;
    margin: 1rem auto;
    text-align: center;
}

.newsletter .content p{
    font-size: 1.5rem;
    line-height: 2;
    color: var(--light-black);
}

.newsletter .content form{
    margin-top: 2rem;
    background: var(--white);
    border-radius: .5rem;
    border: .2rem solid var(--main-color);
    padding: .8rem;
    display: flex;
}

.newsletter .content form .email{
    width: 100%;
    font-size: 1.6rem;
    color: var(--main-color);
    padding: 0 1.3rem;
    text-transform: capitalize;
}

.newsletter .content form .btn{
    margin-top: 0;
    background: none;
}

.newsletter .content form .btn:hover{
    background: var(--main-color);
}

.footer .box-container{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
    gap: 1.5rem;
}

.footer .box-container .box h3{
    font-size: 2rem;
    padding: 1.5rem 0;
    color: var(--main-color);
}

.footer .box-container .box a{
    display: block;
    font-size: 1.4rem;
    color: var(--black);
    padding: 1rem 0;
}

.footer .box-container .box a{
    display: block;
    font-size: 1.4rem;
    color: var(--black);
    padding: 1rem 0;
}

.footer .box-container .box a i{
    color: var(--main-color);
    padding-right: .5rem;
}

.footer .box-container .box a:hover i{
    padding-right: 2rem;
}

.footer .credit{
    text-align: center;
    margin-top: 2.5rem;
    padding: 1rem;
    padding-top: 2.5rem;
    font-size: 2rem;
    color: var(--black);
}

.footer .credit span{
    color: var(--main-color);
}

@media(max-width:991px){

    html{
        font-size: 55%;
    }

    .header{
        padding: 2rem 3rem;
    }

    section{
        padding: 3rem 5rem;
    }
}

@media(max-width:768px){

    #menu{
        display: inline-block;
    }

    .header .navbar{
        position: absolute;
        top: 99%; left: 0; right: 0;
        background: var(--primary);
        border-top: .1rem solid #aaa;
        clip-path: polygon(0 0, 100% 0, 0 0);
    }

    .header .navbar.active{
        clip-path: polygon(0 0, 100% 100%, 0 100%);
    }

    .header .navbar a{
        display: block;
        margin: 2rem;
        color: var(--light-black);
    }

}

@media(max-width:500px){
    html{
        font-size: 50%;
    }

    .newsletter .content{
        max-width: 100%;
    }
}
</style>
