<script>
    export let data;
    let mail = 'abhinav14863@gmail.com';
    let id = 'nobody@gmail.com' ;
    let send = () => {
        let body = document.getElementById("text").value;
        let email = id;
        let subject = data.post.title;
        window.location = "mailto:" + email + "?subject=" + subject + "&body=" + body;
    }
</script> 

<input type="enter the mail id" bind:value={id}>

<button class="p-10 mx-auto bg-blue-500" on:click={send}> mail send</button>

<h1 class="sm:text-4xl text-3xl text-white mt-10 mb-5 text-center">{data.post.title}</h1>
<textarea id="text" cols="100" class="mx-auto max-w-full block text-white  text-lg sm:text-2xl sm:leading-loose leading-relaxed p-6 h-screen bg-gray-900">{data.post.content}</textarea>

