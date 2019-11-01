<template>
    <div class="contact-form">
        <h2 class="contact-form_title">SEND ME A MESSAGE</h2>

        <div v-if="isSending" class="loading">SENDING...</div>
        <div v-if="isSent" class="loading">YOUR MESSAGE IS SENT</div>

        <form class="form" @submit="onSubmit">
            <input required name="name" v-model='contact.name' placeholder="Name" type="text" autocomplete="off">
            <input required name="email" v-model="contact.email" placeholder="E-mail" type="email" autocomplete="off">
            <textarea name="message" v-model="contact.message" rows="4" placeholder="Message"></textarea>
            <button class="button">Send</button>
        </form>
    </div>
</template>

<script>
    export default {
        name: "ContactForm",
        data() {
            return {
                contact: {
                    name: '',
                    email: '',
                    message: ''
                },
                isSending: false,
                isSent: false
            }
        },
        watch: {
            isSent: function(){
                setTimeout(()=>{
                    this.isSent = false
                },4000);
            }
        },
        methods: {
            onSubmit(e) {
                e.preventDefault();
                let currentObj = this;
                this.isSending = true;

                this.axios.post('https://max-yuz.herokuapp.com/feedback', {
                    email: this.contact.email,
                    name: this.contact.name,
                    message: this.contact.message
                })
                    .then(function (response) {
                        currentObj.output = response.data;
                        currentObj.isSending = false;
                        currentObj.isSent = true;
                        currentObj.clearForm();
                        console.log("ok");
                    })
                    .catch(function (error) {
                        currentObj.output = error;
                        currentObj.isSending = false;
                        currentObj.clearForm();
                        console.log(error);
                    });
            },
            clearForm() {
                for (let field in this.contact) {
                    this.contact[field] = ''
                }
            },
        }
    }
</script>

<style scoped lang="sass">

    .contact-form
        margin: 0 auto
        max-width: 600px
        width: 100%

        .contact-form_title
            color: whitesmoke
            text-align: center
            font-weight: 300
            margin-top: 15px

        .form
            display: flex
            flex-direction: column
            font-size: 16px

        input
            &[type="email"], &[type="text"]
                border-bottom: solid 1px whitesmoke
                border-left: none
                border-right: none
                border-top: none
                font-family: 'Barlow Semi Condensed', sans-serif
                padding: 10px 7px
                margin-bottom: 25px
                outline: none
                background-color: #10100e
                color: whitesmoke
                box-sizing: border-box
            &::placeholder
                color: whitesmoke
            &:focus
                border-bottom: solid 2px whitesmoke
                padding: 10px 7px 9px 7px

        textarea
            border: solid 1px whitesmoke
            font-family: 'Barlow Semi Condensed', sans-serif
            padding: 10px 7px
            height: 120px
            margin-bottom: 25px
            outline: none
            resize: none
            background-color: #10100e
            color: whitesmoke
            &::placeholder
                color: whitesmoke


        .button
            background: #10100e
            font-family: 'Barlow Semi Condensed', sans-serif
            border: solid 2px whitesmoke
            color: white
            cursor: pointer
            padding: 10px 50px
            text-align: center
            text-transform: uppercase

            &:hover
                background: whitesmoke
                border: solid 2px whitesmoke
                color: #10100e

        input
            &[type="email"], &[type="text"]
                font-size: 15px
                border-radius: 0

        textarea, .button
            font-size: 15px
            border-radius: 0
</style>
