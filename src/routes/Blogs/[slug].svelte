<script context="module">
//    import {cards} from '../../store.js'
    export async function load(ctx) {
        let slug = ctx.page.params.slug;
    //    let data = getD()
        return { props: { slug} };
    }
</script>

<script>
  import supabase from '$lib/db';
  export let slug;
    // console.log(D.then((doc)=> console.log(doc.data)))
</script>

<div class="select-none dark">
  <section class="flex flex-col items-center w-full py-5 bg-gray-900 font-jetMono dark:bg-white">
    <div class="w-11/12">
      <article class="flex flex-col w-full p-1 shadow-lg from-green-400 via-emerald-400 to-teal-400 dark:sw bg-gradient-to-tr dark:from-cyan-400 dark:to-teal-200 rounded-3xl">
          <p class="px-1.5 py-0.5 text-white dark:text-gray-800 m-2 w-max opacity-80 text-base sm:text-lg ml-auto sm:rounded-lg rounded-md">{supabase[slug-1].date}</p>
          <h1 class="p-3 pl-1 mb-2 ml-1 text-3xl font-thin text-gray-900 border shadow-xl sm:text-5xl md:text-7xl sm:ml-3 rounded-xl max-w-max dark:text-cyan-900">{supabase[slug-1].topic}</h1>
          <p class="p-3 mb-3 text-base text-white sm:text-xl">{supabase[slug-1].content}</p>
      </article>
    </div>
  </section>
</div>
