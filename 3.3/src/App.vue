<template>
    <div>
        <div>
            <h2>Hello Vue.js</h2>
            <p>This is some content.</p>
        </div>
        <div>
            <List item-type="Fruit" 
                :list-items="['apples', 'oranges', 'bananas']" />
        </div>
        <div>
            <List item-type="Guitars" 
                :list-items="guitars" />
        </div>
    </div>
</template>


<script>
import List from './List.vue';
import axios from 'axios';

export default {
    components: {List},
    data() {
        return {
            guitars: []
        };
    },
    created() {
        axios.get('/guitars.json').then(res => {
            this.guitars = res.data.items;
        });
    }
}
</script>
