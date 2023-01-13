<script>
    export let data;
</script> 

<h1 class="text-4xl mb-10 text-center">{data.post.title}</h1>
<div class="max-w-2xl mx-auto">{@html data.post.content}</div>