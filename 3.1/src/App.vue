<template>
    <div>
        <div>
            <h2>Hello Vue.js</h2>
            <p>This is some content.</p>
        </div>
        <div>
            <List :list-items="['apple', 'orange', 'banana']" />
        </div>
    </div>
</template>


<script>
import List from './List.vue';
export default {
    components: {List}
}
</script>
