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
                            <h2>ABOUT ME</h2>
                        </div>
                        <div class="menu-item">
                            <h2>CONTACT ME</h2>
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
                <div class="block-photos">

                </div>
            </div>

            <div class="block">
                <div class="block-form">

                </div>
            </div>

        </div>
    </div>
</template>

<script>
    export default {
        name: "Main"
    }
</script>

<style scoped lang="sass">
    @import url('https://fonts.googleapis.com/css?family=Barlow+Semi+Condensed&display=swap')

    .main
        display: flex
        flex-direction: column
        width: 100%
        height: 100vh
        margin: 0
        background-color: #10100e
        font-family: 'Barlow Semi Condensed', sans-serif


    .container
        display: flex
        flex-direction: column
        width: 60%
        margin: 0 auto
        height: 100vh
        /*background-color: whitesmoke*/

    .block-banner
        display: flex
        flex-direction: column
        width: 67%
        margin: 0 auto
        .banner-menu
            display: flex
            flex-direction: row
            margin: 10px 0 0 0
            color: whitesmoke
            justify-content: space-between
            .menu-logo
                cursor: pointer
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
            margin-top: 10vh
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
            .banner-content-description
                display: flex
                flex-direction: row
                justify-content: space-between
                width: 450px
                .banner-content-description-name,
                .banner-content-description-spec
                    h2
                        font-weight: 300

</style>
