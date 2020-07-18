<template>
    <div class="container">
        <div class="row mt-4">
            <div class="col-md-4 mt-3" v-for="product in products" v-bind:key="product.title">
                <product :title="product.title" :img="product.img" :content="product.content" v-bind:key="product.title"></product>
            </div>
        </div>
    </div>
</template>
<script>
import product from './product.vue'

export default {
    name : 'products',
    components : {
        product,
    },

    data (){
        return {
            products : [
                {title:'Product One',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=23'},
                {title:'Product Two',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=24'},
                {title:'Product Three',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=22'},
                {title:'Product Four',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=21'},
                {title:'Product Five',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=20'},
                {title:'Product Five',content:'Contetndsfa lasdfu asdfk lasduf asldf uasdf liaudf asfd',img:'https://picsum.photos/600/300/?image=25'},
            ],
        }
    }
}
</script>