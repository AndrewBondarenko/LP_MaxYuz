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

                        <div class="content-image">
                            <img src="../assets/images/bannerPhoto.png" alt="Max Yuz">
                            <div class="image-border">
                            </div>
                        </div>

                        <div class="content-title">
                            <div class="title-text">
                                <h1>HI - I'M MAX YUZ,</h1>
                                <H1>AND I AM OUT OF FRAME.</H1>
                            </div>

                            <div class="title-border">
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
        width: 68%
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
                &:hover
                    border-bottom: 2px solid whitesmoke
            .menu-item
                cursor: pointer
                h2
                    font-weight: 300
        .banner-content
            margin-top: 17vh
            display: flex
            flex-direction: row
            color: whitesmoke
            .content-image
                display: flex
                width: 450px
                img
                    height: 450px
                    width: 450px
                .image-border
                    height: 400px
                    width: 400px
                    border: 2px solid whitesmoke
                    position: absolute
                    margin-top: 22px
                    margin-left: -44px
            .content-title
                display: flex
                margin: 197px auto 0 9px
                .title-text
                    h1
                        width: max-content
                        font-weight: 300
                .title-border
                    height: 140px
                    width: 284px
                    border: 2px solid whitesmoke
                    position: absolute
                    margin-top: 0
                    margin-left: -27px


</style>
