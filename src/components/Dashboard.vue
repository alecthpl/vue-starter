<template>
    <div id="dashboard">
        <section>
            <div class="col1">
                <div class="profile">
                    <h5>{{ userProfile.name }}</h5>
                    <p>{{ userProfile.title }}</p>
                    <div class="create-post">
                        <p>create a post</p>
                        <form @submit.prevent>
                            <textarea></textarea>
                            <button class="button">post</button>
                        </form>
                    </div>
                </div>
            </div>
            <div class="col2">
                <div>
                    <p class="no-results">There are currently no posts</p>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    import { mapState } from 'vuex'
    import moment from 'moment'

    export default {
        data() {
            return {

            }
        },
        computed: {
            ...mapState(['userProfile'])
        },
        methods: {

        }
    }
</script>
