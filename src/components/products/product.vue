<template>
    <div>
                <b-card
                    :title="title"
                    :img-src="img"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="mb-2"
                >
                    <b-card-text>
                    {{content}}
                    </b-card-text>

                    <b-button href="#" variant="primary">Details</b-button>
                </b-card>
    </div>
</template>
<script>
export default {
    name : 'product',
    props: {
        title: String,
        img:String,
        content:String
    }
}
</script>