<template>
    <div class="signIn">
        <div class="textSignIn">
            <h2>{{ heading }}</h2>
            <div class="signUp">
                <p>{{ subText }}</p>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue"

let props = defineProps([
    "heading",
    "subText"
])
let heading = ref(props.heading), subText = ref(props.subText)

</script>

<style>
.textSignIn {
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    width: 100%;
}

.textSignIn h2 {
    font-family: 'Poppins';
    font-size: 21px;
    font-weight: 700;
}

h2, p{
    margin: 0.2rem
}

.textSignIn p {
    font-family: 'Poppins';
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
    letter-spacing: 0em;
    text-align: left;
}
</style>