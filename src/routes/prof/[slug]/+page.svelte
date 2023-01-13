<script>
    export let data;
    let mail = 'abhinav14863@gmail.com'
</script> 

<h1 class="sm:text-4xl text-3xl text-white mt-10 mb-5 text-center">{data.post.title}</h1>
<div class="mx-auto text-white max-w-6xl text-lg sm:text-2xl sm:leading-loose leading-relaxed p-6 h-screen">{@html data.post.content}</div>

<!-- <button class="p-10 mx-auto bg-blue-500">

    <a href="mailto:{mail}?subject={data.post.title}&body={data.post.content}">tell a friend</a>
</button> -->