<template>
    <v-container>
    <div class="header">
        <v-layout align-center>
            <div class = "logo" @click="moveHome"> Yun Hye In's Portfolio</div>
            <v-spacer></v-spacer>
        </v-layout>
        </div>
        </v-container>
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
        box-shadow: 0 3px 3px #eee;
        position: fixed;
        z-index: 100;
        background: white;
        left: 0;
        right: 0;
        top: 0;
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