<template>
    <body>
        <div class="grass"></div>
        <div class="content">
            <div class="container">
                <CompBox class="about-me"
                    title="About Me"
                    msg="Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna ali">
                </CompBox>
            </div>
            <div class="container">
                <CompBox class="research"
                    title="Research Interests"
                    msg="Lorem ipsum dolor sit amet, consectetuer adipiscing elit, sed diam nonummy nibh euismod tincidunt ut laoreet dolore magna ali">
                </CompBox>
            </div>
        </div>
    </body>
</template>
<script>
    import { Options, Vue } from "vue-class-component";
    import CompBox from "@/components/CompBox.vue"; // @ is an alias to /sr
    @Options({
        data() {
            return {
                did_say_hello: false
            };
        },
        components: {
            CompBox,
        },
        created() {
                console.log("Hello from vue!", this.did_say_hello)
                this.did_say_hello = true
                console.log("Changed", this.did_say_hello)
        },
        methods: {
            myFunction(locale) {
                this.did_say_hello = true
                console.log("Hello world", this.did_say_hello)
            },
        }
    })
    export default class LandingPage extends Vue {}
</script>

<style scoped>
    .grass {
        z-index: 10;
        position: absolute;
        bottom: 0em;
        left: 0;
        right: 0;
        width: 100%;
        border-radius: 0.5em;
        height: 3em;
        background-color: #2f9d63;
    }
    .container {
        height: 100vh;
        width: 100%;
        display: flex;
        align-items: center;
    }
</style>