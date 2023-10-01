<script>
  import TagCloud from "TagCloud";
  const container = ".content";
  import { onMount } from "svelte";
  const texts = [
    "3D",
    "TagCloud",
    "JavaScript",
    "CSS3",
    "TailwindCSS",
    "Svelte",
    "SvelteKit",
    "Vercel",
    "Git",
    "Github",
  ];
  const options = {
    maxSpeed: "fast",
  };

  onMount(() => {
    TagCloud(container, texts, options);
  });
</script>

<h1
  class="text-center mb-4 text-6xl font-extrabold tracking-tight leading-none  md:text-5xl lg:text-6xl text-white"
>
  About Us
</h1>
<p
  class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400"
/>
<p
  class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400 px-4 block"
/>

<div class="px-4 md:px-0">
  <ul>
    <li>
      <p
        class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400 "
      >
        We are excited to introduce our new email template website designed to promote a culture of effective and
        efficient communication among college students. The website offers a wide range of templates for various
        scenarios, such as requesting information from professors, scheduling meetings, and networking with professionals.
      </p>
    </li>
    <li>
      <p
        class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400"
      >
        Our templates are designed to be easy to use and customize, allowing students to quickly and effectively
        communicate their needs and ideas. They are also crafted to maintain a professional and respectful tone,
        thereby promoting a positive image of the college community.
      </p>
    </li>
    <li>
      <p
        class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400"
      >
        We believe that by fostering a culture of effective communication, we can help students succeed both
        academically and professionally. Our templates serve as a valuable resource for students who are new to the
        college environment or who want to enhance their communication skills.
      </p>
    </li>
    <li>
      <p
        class="mb-8 text-lg font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400"
      >
        We would love for you to check out our website and share your thoughts. We are always eager to receive feedback
        and suggestions on how to further improve our service.
      </p>
    </li>
  </ul>
</div>

<h1
  class="text-center mb-4 text-6xl font-extrabold tracking-tight leading-none  md:text-5xl lg:text-6xl text-white"
>
  <span
    class="text-transparent bg-clip-text bg-gradient-to-b from-gray-900 via-purple-900 to-violet-600"
    >Tech Stack</span
  >
</h1>

<div class="px-4 md:px-0">
  <p
    class="mb-2 text-xl font-normal text-center lg:text-xl sm:px-16 xl:px-48 text-gray-400"
  >
    We believe that the key to success in web development is staying up-to-date with the latest technologies and
    best practices. Our tech stack is built on a combination of cutting-edge technologies that allow us to create fast,
    efficient, and user-friendly web applications. Our core tech stack includes:<br/><br />
  </p>
  <span class="content tagcloud  text-2xl   mx-auto text-purple-600 " />
</div>
<br /><br /><br />
<h1
  class="mt-2 text-center mb-4 text-4xl font-extrabold tracking-tight leading-none  md:text-4xl lg:text-4xl text-white"
>
  <span
    id="problems" class="mt-6 text-transparent bg-clip-text bg-[radial-gradient(ellipse_at_top_left,_var(--tw-gradient-stops))] from-gray-900 via-purple-900 to-violet-600"
    >Navigating Problems</span
  >
</h1>

<div class="px-4 md:px-0">
  <p
    class="mb-8 text-lg font-normal text-left lg:text-xl sm:px-16 xl:px-48 text-gray-400 px-4 block"
  >
    We encountered several problems while working on our project. Here are a few notable ones along with their solutions:<br /><br />
    1. <b>New Lines in JavaScript String: </b><br />
    All of the templates on our website are stored in easily editable JavaScript stores, and the entire mail is stored
    as a single string for ease of navigation and editing. This meant we had to include all of the line breaks
    inside the string itself.<br /><br />

    <a
      class="underline italic"
      href="https://stackoverflow.com/questions/10154429/javascript-string-with-new-line-but-not-using-n"
      >The solution</a
    >
    --- We discovered that using "\n" would solve our problem. Upon further research, we also learned about
    template literals, which made storing entire mails as a string much easier. This contributed to making
    the project more beginner-friendly.<br /><br />

    2. <b>Setting the Content of the Textarea as the Body of the Email:</b><br />
    Our next challenge was bringing those strings into the textarea while keeping them editable
    and sending the edited text as the body of the email.<br /><br /><a
      class="underline italic"
      href="https://stackoverflow.com/questions/44710300/how-to-add-the-content-of-a-textarea-to-the-body-of-an-email"
      >The solution</a
    >
    --- This took a significant amount of time, as we explored multiple solutions, each with its own set of problems.
    After extensive searching, we finally found a solution that worked without requiring a major overhaul of our system.<br /><br />

    3. <b>Adding Line Breaks into the Email Body:</b><br />
    Although it might not seem like a significant issue, this was by far the most challenging problem to solve.
    We tried multiple solutions that didn't work as intended. For example, replacing new lines
    with <br> tags proved ineffective.<br /><br />
    <a
      class="underline italic"
      href="https://stackoverflow.com/questions/22765834/insert-a-line-break-in-mailto-body"
      >The solution</a
    >
    --- After extensive searching and trying out different solutions, we finally discovered that email text uses
    a special symbol to insert line breaks:
    <code>" %0D%0A "</code>
    <br /><br />
    <center> Thanks for reading till the very end. Peace ✌️ </center>
  </p>
</div>
