<template>
    <div class="main">
        <div class="container">
            <div class="block">
                <div class="block-banner">
                    <div class="banner-menu">
                        <div class="menu-logo">

                            <div class="logo-text">
                                <h2>MAX YUZ</h2>
                            </div>
                        </div>
                        <div class="menu-item">
                            <h2><a href="#about">ABOUT ME</a></h2>
                        </div>
                        <div class="menu-item">
                            <h2><a href="#contact">CONTACT ME</a></h2>
                        </div>
                    </div>
                    <div class="banner-content">
                        <div class="banner-content-header">
                            <div class="banner-content-image">
                                <img src="../assets/images/bannerPhoto.png" alt="Max Yuz">
                                <div class="banner-image-border">
                                </div>
                            </div>

                            <div class="banner-content-title">
                                <div class="banner-title-text">
                                    <h1>HI - I'M MAX YUZ,</h1>
                                    <H1>AND I AM OUT OF FRAME.</H1>
                                </div>
                                <div class="banner-title-border">
                                </div>
                            </div>

                            <div class="logo-img">
                                <img src="../assets/images/logo2.png" alt="">
                            </div>

                        </div>
                        <div class="banner-content-description">
                            <div class="banner-content-description-name">
                                <h2>MAX YUZ</h2>
                            </div>
                            <div class="banner-content-description-spec">
                                <h2>CAMERAMAN</h2>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="block">
                <div class="block-about" id="about">
                    <div class="about-title">
                        <h2>ABOUT ME</h2>
                    </div>
                    <div class="about-content">
                        <div class="about-content-description">
                            <div class="about-content-description-text">
                                <h2>MAX YUZ</h2>
                                <h2>20 YEARS OLD</h2>
                                <h2>KYIV CITY</h2>
                                <h2>CAMERAMAN</h2>
                            </div>
                            <div class="about-content-description-photo">
                                <img src="../assets/images/maxyuz1.png" alt="Max Yuz">
                            </div>
                        </div>

                        <div class="about-content-image">
                            <img src="../assets/images/maxyuz3.jpg" alt="Max Yuz">
                        </div>
                        <div class="about-content-image-border-1">

                        </div>

                        <div class="about-content-image">
                            <img src="../assets/images/maxyuz2.jpg" alt="Max Yuz">
                        </div>
                        <div class="about-content-image-border-2">

                        </div>

                    </div>
                </div>
            </div>

            <div class="block">
                <div class="block-contact"  id="contact">
                    <div class="contact-title">
                        <h2>CONTACT ME</h2>
                    </div>
                    <div class="contact-info">
                        <div class="contact-info-text">
                            <h2>EMAIL : maxyuz.production@gmail.com</h2>
                            <h2>PHONE NUMBER: +380 63 858 2636</h2>
                        </div>
                    </div>
                    <div class="contact-links">
                        <div class="contact-links-item">
                            <a href="https://www.instagram.com/max_yuz/?hl=ru" target="_blank">
                                <img src="../assets/images/instagram.png" alt="">
                            </a>
                        </div>
                        <div class="contact-links-item">
                            <a href="https://www.youtube.com/channel/UC2NOFzo1h_YpEMVveeEUF1g" target="_blank">
                                <img src="../assets/images/youtube.png" alt="">
                            </a>
                        </div>
                        <div class="contact-links-item">
                            <a href="" target="_blank">
                                <img src="../assets/images/facebook.png" alt="">
                            </a>
                        </div>
                    </div>

                    <div id="contact-form">
                        <ContactForm></ContactForm>
                    </div>

                </div>
            </div>

        </div>
    </div>
</template>


<script>
import ContactForm from '../components/ContactForm'

    export default {
        name: "Desktop",
        components: {
            ContactForm
        },
        data() {
            return {
            }
        }
    }
</script>

<style scoped lang="sass">
    @import url('https://fonts.googleapis.com/css?family=Barlow+Semi+Condensed&display=swap')

    .main
        display: flex
        flex-direction: column
        width: 100%
        height: max-content
        margin: 0
        background-color: #10100e
        font-family: 'Barlow Semi Condensed', sans-serif
        color: whitesmoke
    a
        text-decoration: none
        color: whitesmoke

    .container
        display: flex
        flex-direction: column
        width: 90%
        margin: 0 auto

    .block
        min-height: 100vh


    .block-banner
        display: flex
        flex-direction: column
        width: 765px
        margin: 0 auto
        .banner-menu
            display: flex
            flex-direction: row
            margin: 10px 0 0 0
            color: whitesmoke
            justify-content: space-between
            .menu-logo
                cursor: pointer
                display: flex
                flex-direction: row
                h2
                    font-weight: 300

            .menu-item, .menu-logo
                cursor: pointer
                text-align: center
                text-transform: uppercase
                position: relative
                overflow: hidden
                transition: .3s
                &:after
                    position: absolute
                    transition: .3s
                    content: ''
                    width: 0
                    left: auto
                    right: 0
                    bottom: 0
                    margin-bottom: 10px
                    height: 2px
                    background: whitesmoke
                &:hover
                    cursor: pointer
                    &:after
                        width: 100%
                        left: 0
                h2
                    font-weight: 300
        .banner-content
            margin-top: 17vh
            display: flex
            flex-direction: column
            color: whitesmoke
            .banner-content-header
                display: flex
                flex-direction: row
                .banner-content-image
                    display: flex
                    width: 450px
                    img
                        height: 450px
                        width: 450px
                    .banner-image-border
                        height: 400px
                        width: 400px
                        border: 2px solid whitesmoke
                        position: absolute
                        margin-top: 22px
                        margin-left: -44px
                        transition: 1.5s
                        &:hover
                            margin-left: 0
                            transition: 1.5s
                .banner-content-title
                    display: flex
                    margin: 197px auto 0 9px
                    .banner-title-text
                        h1
                            width: max-content
                            font-weight: 300
                    .banner-title-border
                        height: 140px
                        width: 284px
                        border: 2px solid whitesmoke
                        position: absolute
                        margin-top: 0
                        margin-left: -27px
                        transition: 1.5s
                        &:hover
                            margin-left: -5px
                            transition: 1.5s
                .logo-img
                    position: absolute
                    margin-top: 391px
                    margin-left: 391px
                    z-index: 100
                    img
                        height: 50px

            .banner-content-description
                display: flex
                flex-direction: row
                justify-content: space-between
                width: 450px
                .banner-content-description-name,
                .banner-content-description-spec
                    h2
                        font-weight: 300

    .block-about
        display: flex
        flex-direction: column
        /*width: 45%*/
        width: 765px
        margin: 50px auto 100px auto
        .about-title
            margin: 50px auto 40px auto
            h2
                color: whitesmoke
                font-weight: 300
        .about-content
            display: flex
            flex-direction: column
            .about-content-description
                display: flex
                flex-direction: row
                justify-content: space-between
                .about-content-description-text
                    width: 350px
                    text-align: left
                    border: 2px solid whitesmoke
                    padding: 20px
                    h2
                        color: whitesmoke
                        font-weight: 300
                    h2:first-child
                        margin-top: 0
                        margin-bottom: 50px
                        font-size: 34px

                .about-content-description-photo
                    height: 350px
                    width: 350px
                    img
                        height: 350px
                        width: 350px

            .about-content-image
                width: 765px
                margin: 20px auto 0 auto
                img
                    width: 765px

            .about-content-image-border-1
                height: 390px
                width: 650px
                border: 2px solid whitesmoke
                position: absolute
                margin-top: 400px
                margin-left: 140px
                transition: 1.5s
                &:hover
                    margin-left: 110px
                    transition: 1.5s

            .about-content-image-border-2
                height: 400px
                width: 580px
                border: 2px solid whitesmoke
                position: absolute
                margin-top: 925px
                margin-left: -45px
                transition: 1.5s
                &:hover
                    margin-left: 0
                    transition: 1.5s


    .block-contact
        display: flex
        flex-direction: column
        width: 600px
        margin: 50px auto 100px auto
        .contact-title
            margin: 0 auto 40px auto
            h2
                color: whitesmoke
                font-weight: 300
        .contact-info
            display: flex
            flex-direction: column
            border: 2px solid whitesmoke
            padding: 20px
            margin-bottom: 25px
            .contact-info-text
                text-align: left
                h2
                    font-weight: 300
                h2:first-child
                    margin-top: 0
                h2:last-child
                    margin-bottom: 0

        .contact-links
            display: flex
            flex-direction: row
            justify-content: center
            .contact-links-item
                height: 45px
                padding: 1px
                background-color: whitesmoke
                border-radius: 50%
                margin: 10px
                cursor: pointer
                img
                    height: 45px

</style>
