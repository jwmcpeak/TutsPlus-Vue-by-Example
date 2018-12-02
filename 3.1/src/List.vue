<template>
    <div>
        <ul>
            <li v-for="item in listItems">
                {{item}}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    props: ['listItems']


}
</script>
