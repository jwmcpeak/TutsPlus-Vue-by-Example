<template>
    <div>
        <h2>{{itemType}}</h2>
        <ul>
            <li v-for="(item, index) in listItems" :key="index">
                {{item}}
            </li>
        </ul>
        <p v-if="listItems.length > 0">There are {{listItems.length}} {{itemType.toLowerCase()}}.</p>
        <p v-else>There are no {{itemType.toLowerCase()}}.</p>
    </div>
</template>

<script>
export default {
    props: {
        itemType: {
            default: ''
        },
        listItems: {
            default: () => []
        }
    }
}
</script>
