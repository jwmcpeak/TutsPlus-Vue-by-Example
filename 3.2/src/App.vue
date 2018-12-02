<template>
    <div>
        <div>
            <h2>Hello Vue.js</h2>
            <p>This is some content.</p>
        </div>
        <div>
            <List item-type="Fruit" :list-items="['apples', 'oranges', 'bananas']" />
        </div>
        <div>
            <List item-type="Guitars" :list-items="['Les Paul', 'PRS Starla', 'Strat']" />
        </div>
    </div>
</template>


<script>
import List from './List.vue';
export default {
    components: {List}
}
</script>
