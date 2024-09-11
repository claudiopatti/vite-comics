<script>
import AppMainBottom from './AppMainBottom.vue';

export default {
    data() {
      return {
      };
    },
    components: {
        AppMainBottom
    }
}
</script>

<template>
    <main >
        <section class="fistSectionMain">
            <div class="container">
                <div class="contentContainer">
                    --&gt; Content goes here &lt;--
                </div>
            </div>
        </section>

        <AppMainBottom />
    </main>
</template>

<style lang="scss" scoped>
/* general */


.container {
    max-width: 1000px;
    margin: 0 auto;
    display: flex;
}


/* main  */
.fistSectionMain {
    background-color: black;

    .container {
        .contentContainer {
            color: white;
            font-size: 20px;
            padding: 30px 0;
            font-weight: bold;
        }
    }
}


</style>