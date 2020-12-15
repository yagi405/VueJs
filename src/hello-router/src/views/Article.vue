<template>
    <div class="article">
        <h1>This is an article page</h1>
        <span> ArticleID : {{id}} </span>
    </div>
</template>

<script>
export default {
    name:'Article',
    props:['id'],
}
</script>