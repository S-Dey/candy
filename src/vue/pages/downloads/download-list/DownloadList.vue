<template>
    <div class="download-list">
        <download-item v-for="download of downloads" :download="download"/>
    </div>
</template>

<script>

    // Vuex stuff
    import {mapState} from 'vuex';

    // Components
    import DownloadItem from './DownloadItem';

    export default {
        components: {DownloadItem},

        data() {
            return {};
        },

        computed: {
            ...mapState(['downloads'])
        }
    };

</script>

<style lang="scss" scoped>

    .download-list {

    }

    .download-item {
        margin: 1em 2em;
    }

</style>