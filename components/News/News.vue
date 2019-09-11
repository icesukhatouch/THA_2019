<template>
    <b-container>
        <b-row>
            <b-col class="d-flex align-items-center">
                <div class="headline"></div>
            </b-col>
            <b-col class="topic">NEWS</b-col>
        </b-row>
        <div id="posts">
            <PostPreview
                v-for="post in posts"
                :key="post.id"
                :title="post.title"
                :excerpt="post.previewText"
                :thumbnailImage="post.thumbnailUrl"
                :id="post.id">
            </PostPreview>
        </div>
        <b-row>
            <div class="headline"></div>
        </b-row>
    </b-container>
</template>


<script>
import PostPreview from '@/components/News/PostPreview/PostPreview'
export default {
    components: {
        PostPreview
    },
    data() {
        return {
            posts: [
                {
                    title: 'Title of this post',
                    previewText: 'preview text',
                    thumbnailUrl: 'https://i0.wp.com/images-prod.healthline.com/hlcmsresource/images/AN_images/benefits-of-pineapple-1296x728-feature.jpg?w=1155&h=1528',
                    id: 'title-of-this-post'
                },
                {
                    title: '22Title of this post',
                    previewText: '22preview text',
                    thumbnailUrl: 'https://i0.wp.com/images-prod.healthline.com/hlcmsresource/images/AN_images/benefits-of-pineapple-1296x728-feature.jpg?w=1155&h=1528',
                    id: '22title-of-this-post'
                },
                {
                    title: '33Title of this post',
                    previewText: '333333preview text',
                    thumbnailUrl: 'https://i0.wp.com/images-prod.healthline.com/hlcmsresource/images/AN_images/benefits-of-pineapple-1296x728-feature.jpg?w=1155&h=1528',
                    id: '33333title-of-this-post'
                }
            ]
        }
    }
}
</script>
<style scoped>
    .topic {
        font-size: 5rem;
        color: #FDD738;
    }
    .headline {
        border: 2px white solid;
        width: 40rem;
        margin-top: 2rem;
    }
    #posts {
        padding-top: 2rem;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }
    @media(min-width: 35rem) {
        flex-direction: row;
    }
</style>
