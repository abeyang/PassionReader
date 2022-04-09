<script>
  import { Router, Route, Link } from "svelte-navigator";
  import PageShelf from "./PageShelf.svelte";
  import PageHeader from "./PageHeader.svelte";
  import { styles } from "./styles.js";
  import { toc } from "./toc.js";
  import { onMount } from "svelte";
  import "@lottiefiles/lottie-player";
  import { create } from "@lottiefiles/lottie-interactivity";

  let page = toc[11];

  function handleLoad(event) {
    create({
      mode: "scroll",
      player: "#graphic1",
      actions: [
        {
          visibility: [0.1, 0.7],
          type: "loop",
          frames: [0, 379]
        }
      ]
    });

    create({
      mode: "scroll",
      player: "#graphic2",
      actions: [
        {
          visibility: [0.1, 0.7],
          type: "loop",
          frames: [0, 359]
        }
      ]
    });
  }
</script>

<style>
</style>

<PageShelf />

<!-- All styles are defined under styles.js -->

<div class={$styles.container}>

  <PageHeader title={page.title} author={page.author} level={page.level} words={page.words} />

  <section class={$styles.b_content}>
    <!-- graphic -->
    <lottie-player id="graphic1"
              src="pages/thief/12-01-seesaw.json"
              class={$styles.image}
              on:load={handleLoad}>
    </lottie-player>
  </section>

  <section class={$styles.a_content}>
    <p class={$styles.p}>Five years ago I came to believe in Christ’s teachings, and my life suddenly changed; I ceased to desire what I had previously desired, and began to desire what I formerly did not want.</p>  
    
    <p class={$styles.p}>What had previously seemed to me good seemed evil, and what seemed evil seemed good. It happened to me as it happens to a man who goes out on some business and suddenly decides that the business is unnecessary and returns home. All that was on his right is now on his left, and all that was on his left is now on his right; his former wish to get as far as possible from home has changed into a wish to be as near as possible to it.</p>
    
    <p class={$styles.p}><strong class={$styles.strong}>The direction of my life and my desire became different, and good and evil changed places…</strong> I, like that thief on the cross, have believed Christ’s teaching and been saved. This is no far-fetched comparison, but the closest expression of the condition of spiritual despair and horror at the problem of life and death in which I lived formerly, and of the condition of peace and happiness in which I am now.</p>
    
    <p class={$styles.p}>I, like the thief, knew that I had lived and was living badly. I, like the thief, knew that I was unhappy and suffering. I, like the thief to the cross, was nailed by some force to a life of suffering and evil. And as, after the meaningless sufferings and evils of life, the thief awaited the terrible darkness of death, so did I await the same thing.</p> 
  </section>

  <section class={$styles.b_content}>
    <!-- graphic -->
    <lottie-player id="graphic2"
              src="pages/thief/12-02-ball.json"
              class={$styles.image}
              on:load={handleLoad}>
    </lottie-player>
  </section>

  <section class={$styles.a_content}>
    <blockquote class={$styles.quote}>In all this I was exactly like the thief, but the difference was that life still awaited me here.</blockquote>
    
    <p class={$styles.p}>In all this I was exactly like the thief, but the difference was that life still awaited me here. And I did not understand that life. It seemed to me terrible. But suddenly I heard the words of Christ and understood them, and life and death ceased to seem evil, and instead of despair I experienced happiness and the joy of life undisturbed by death.</p>  
    
    
  </section>

</div> <!-- /.container -->
