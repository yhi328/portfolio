<template>
    <div class="header">
        <v-layout align-center>
            <div class = "logo" @click="moveHome"> Yun Hye In's Portfolio</div>
            <v-spacer></v-spacer>
            <v-btn @click=moveAbout>ABOUT</v-btn>
            <v-btn @click=moveWork>WORK</v-btn>
        </v-layout>
        </div>
</template>

<script>
    export default {
        methods: {
            moveHome() {
            this.$router.push("/")
        },
            moveWork() {
            this.$router.push("/WorkView")
        },
            moveAbout() {
            this.$router.push("/AboutView")
        }
    }
}
    </script>

<style scoped>
    .header{
        padding:20px;
        box-shadow: 0 6px 6px #eee;
    }
    .header .logo{
        font-size:20px;
        font-weight:bold;
    }
    .v-btn {
        border: none;
        outline: none;
        box-shadow: none;
        color: none;
    }
</style>