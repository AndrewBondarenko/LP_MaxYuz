<template>
    <div>
        <div class="block">
            <div class="block-banner">
                <div class="banner-content">
                    <div class="banner-content-header">
                        <div class="banner-content-description">
                            <div class="banner-content-description-name">
                                <h2>MAX YUZ</h2>
                            </div>
                            <div class="banner-content-description-spec">
                                <h2>CAMERAMAN</h2>
                            </div>
                        </div>
                        <div class="banner-content-image">
                            <img src="../assets/images/bannerPhoto.png" alt="Max Yuz">
                            <div class="banner-image-border">
                            </div>
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
                    </div>

                    <div class="about-content-image">
                        <img src="../assets/images/maxyuz3.jpg" alt="Max Yuz">
                    </div>

                    <div class="about-content-image">
                        <img src="../assets/images/maxyuz2.jpg" alt="Max Yuz">
                    </div>

                </div>
            </div>
        </div>

        <div class="block">
            <div class="block-contact">
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

                <div>
                    <ContactForm></ContactForm>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
import ContactForm from '../components/ContactForm'

    export default {
        name: "Mobile",
        components: {
            ContactForm
        }
    }
</script>

<style scoped lang="sass">

    .block-banner
        display: flex
        flex-direction: column
        width: 310px
        margin: 0 auto 50px auto
        color: whitesmoke
        .banner-content
            margin-top: 15px
            display: flex
            flex-direction: column
            .banner-content-header
                display: flex
                flex-direction: column
                width: 310px
                margin: 0 auto
                .banner-content-image
                    display: flex
                    width: 320px
                    img
                        height: 310px
                        width: 310px
            .banner-content-description
                display: flex
                flex-direction: row
                justify-content: space-between
                width: 310px
                margin-bottom: 0
                .banner-content-description-name,
                .banner-content-description-spec
                    h2
                        font-weight: 300

    .block-about
        display: flex
        flex-direction: column
        width: 310px
        margin: 20px auto 50px auto
        .about-title
            margin: 20px auto 10px auto
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
                    width: 310px
                    text-align: left
                    border: 2px solid whitesmoke
                    padding: 20px
                    h2
                        color: whitesmoke
                        font-weight: 300
                        font-size: 18px
                    h2:first-child
                        margin-top: 0
                        margin-bottom: 20px
                        font-size: 34px

                .about-content-description-photo
                    height: 310px
                    width: 310px
                    img
                        height: 310px
                        width: 310px

            .about-content-image
                width: 310px
                margin: 20px auto 0 auto
                img
                    width: 310px


    .block-contact
        display: flex
        flex-direction: column
        width: 310px
        margin: 20px auto 100px auto
        color: whitesmoke
        .contact-title
            margin: 0 auto 10px auto
            h2
                color: whitesmoke
                font-weight: 300
        .contact-info
            display: flex
            flex-direction: column
            border: 2px solid whitesmoke
            padding: 15px
            margin-bottom: 25px
            .contact-info-text
                text-align: left
                h2
                    font-weight: 300
                    font-size: 18px
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

    .contact-form
        margin: 0 auto 50px auto
        max-width: 310px
        width: 100%

</style>
