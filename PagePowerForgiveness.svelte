<script>
  import { Router, Route, Link } from "svelte-navigator";
  import PageShelf from "./PageShelf.svelte";
  import PageHeader from "./PageHeader.svelte";
  import { styles } from "./styles.js";
  import { toc } from "./toc.js";
  import { onMount } from "svelte";
  import "@lottiefiles/lottie-player";
  import { create } from "@lottiefiles/lottie-interactivity";

  let page = toc[10];
</script>

<style>
</style>

<PageShelf />

<!-- All styles are defined under styles.js -->

<div class={$styles.container}>

  <PageHeader title={page.title} author={page.author} level={page.level} words={page.words} />


  <!-- Change this whole section below! -->

  <section class={$styles.b_content}>
    <!-- graphic -->
    <img src="pages/forgiveness/11 - 01.jpg" class={$styles.image} alt="Forgiveness Header">
  </section>

  <section class={$styles.a_content}>
    <p class={$styles.p}>Easter is far more than a holiday or a celebration; it is power. Jesus taught us to love our enemies and to bless those who persecute us. These are not just words. As his compassionate plea from the cross shows — “Father, forgive them, for they know not what they do” — he practiced what he preached. So did Stephen, the first Christian martyr, who prayed much the same thing as he was being stoned to death: “Father, do not hold this against them.”</p>
    <p class={$styles.p}> <strong class={$styles.strong}>Many people, including Bible-believing Christians, dismiss such an attitude as self-destructive foolishness. </strong> How can we embrace someone intent on harming or killing us? Why not fight back in self defense? What about justice? </p>
    <blockquote class={$styles.quote}>Refusing to forgive is tantamount to re-crucifying Christ. Instead of seeing stones rolled away, we throw stones at each other. </blockquote>
    <p class={$styles.p}>All the while we eagerly pray, “Forgive us our debts, as we forgive our debtors.” Familiar as they are, I often wonder whether we really mean what we say when we repeat these words from the Lord's Prayer, and whether we sufficiently consider their meaning. Besides, Jesus was adamant when it came to the issue of forgiveness: “Go, and be reconciled to your brother, then come and offer your gift...If you forgive others when they sin against you, your heavenly Father will also forgive you. But if you do not forgive others their sins, your Father will not forgive your sins” (Matthew 5:24; 6:14-15).</p>
    <p class={$styles.p}>Refusing to forgive is tantamount to re-crucifying Christ. Instead of seeing stones rolled away, we throw stones at each other.  What so many people today fail to realize is that <strong class={$styles.strong}> forgiveness is the door to peace and happiness. Forgiving is not ignoring wrongdoing, but overcoming the evil inside us and in our world with love.</strong> To forgive is not just a command of Christ but the key to reconciling all that is broken in our lives and relationships. In the words of Martin Luther King, Jr.—</p>
    <div class={$styles.quotelong}>
    <p class="{$styles.p} mt-10">Returning hate for hate multiplies hate, adding deeper darkness to a night already devoid of stars. Darkness cannot drive out darkness; only light can do that. Hate cannot drive out hate; only love can do that. Hate multiplies hate, violence multiplies violence, and toughness multiplies toughness in a descending spiral of destruction... Love is the only force capable of transforming an enemy into a friend. We never get rid of an enemy by meeting hate with hate; we get rid of an enemy by getting rid of enmity. </p> </div>
    <p class={$styles.p}>I've lived long enough to learn that failure to forgive leads down the path of destruction — of bitterness, self-hate, alienation, relentless cycles of conflict, and downright misery. <strong class={$styles.strong}>But forgiveness can vanquish all such pain.</strong> Why else did Jesus command us to forgive? It can heal both the forgiver and the forgiven. In fact, it could change the world if we allowed it to. But too often we stand in its way, not daring to let it flow through us unchecked. If only we would dare! </p>
    <blockquote class={$styles.quote}>Why else did Jesus command us to forgive? It can heal both the forgiver and the forgiven. In fact, it could change the world if we allowed it to.</blockquote>
    <h2 class={$styles.h2}>Steven Mcdonald</h2>
    <p class={$styles.p}><strong class={$styles.strong}>When Christians do put Christ command into practice by forgiving, they create a ripple effect that can touch thousands of lives, and even affect the course of history. </strong></p>
  </section>

  <section class={$styles.a_content}>
    <!-- graphic -->
    <p><img src="pages/forgiveness/11 - 02.png" class={$styles.image} alt="Steven McDonald in the hospital"/></p>
    <p class={$styles.p}>Steven McDonald, a close friend of mine and a New York City police officer, stopped to question three youths in Central Park one day in 1986. He was shot and paralyzed from the neck down. Steven had been married less than a year and his wife was two months pregnant. <strong class={$styles.strong}>Steven forgave his attacker, and in so doing found peace and purpose in his life.</strong></p>
    
    <!-- graphic -->
    <p><img src="pages/forgiveness/11 - 03.png" class={$styles.image} alt="Steven McDonald quote on him forgiving his attacker"/></p>
  
    <p class={$styles.p}>Despite being bound to a wheelchair and breathing machines, Steven has traveled several times to conflict-ridden Northern Ireland to speak about reconciliation. And he regularly visits high schools to speak about the power of forgiveness to resolve personal conflicts. His life is effecting changes in people in ways neither he nor anyone else would ever have imagined prior to his assault. </p>

    <h2 class={$styles.h2}>Chris Carrier</h2>
    <!-- graphic -->
    <p><img src="pages/forgiveness/11 - 04.png" class={$styles.image} alt="Newpaper clipping of abduction story" /></p>
    <p class={$styles.p}>When we forgive we set ourselves free from the demon of bitterness. But we also set loose the power of love in the world. When Miami native Chris Carrier was ten, a former family employee abducted him, assaulted him, shot him in the head, and left him to die in the Everglades. But Chris survived. In the years that followed, he struggled daily with the insecurity of knowing that his abductor was at large. Recognizing that staying angry would never change anything, Chris found the strength to move on. Then some 20 years later he received a telephone call that changed his life again. It was the police calling to notify him that an elderly man at a local nursing home, David McAllister, had confessed to being his abductor. </p>
    <p class={$styles.p}>Chris visited him the following day. He saw how David's body was ruined by alcoholism and that, unable to see, he was now facing death with only his regrets to keep him company. At the end of their time together, David clasped Chris's hand and told him he was sorry. As he spoke, something came over Chris like a wave. As he said later: “Why should anyone have to face death without family, friends, the joy of life — without hope. I couldn't do anything but offer him my forgiveness and friendship.” </p>

    <!-- graphic -->
    <p><img src="pages/forgiveness/11 - 05.png" class={$styles.image} alt="Chris Carrier visiting his kidnapper in a nursing home"/></p>

    <p class={$styles.p}>And friendship indeed. In the days that followed, Chris visited David as often as he could, usually bringing along his wife and their two daughters. They spent hours talking, reading, and even praying together, and as they did, the old man's hardness gradually melted away.</p>
    <p class={$styles.p}>If the cross and resurrection are not just historical happenings but present realities, which I believe they are, then what we celebrate at Easter is the healing power of God's forgiveness at work in our world today. God's forgiveness can transform lives on a personal level, but it can influence events on a broader scale as well.</p>
    
    <h2 class={$styles.h2}>The “Awakening”</h2>
    <p class={$styles.p}>Such was the case in the “awakening” at Möttlingen, Germany, which began on New Year's Eve 1843, when a young man known for his wild carousing and violent temper came to the door of pastor Christoph Blumhardt to confess all his sins. This began an unprecedented wave of confessions in which one remorseful villager after another came to reveal secret sins and reconcile their differences. Pierced to the heart, people from all walks of life felt compelled from within to break out of old ways. Stolen goods were returned, enemies reconciled, infidelities and crimes (including a case of infanticide) confessed, and broken marriages restored.</p>
    <p class={$styles.p}>Jesus offered his disciples the “keys of the kingdom.” We hold the key of forgiveness in our hands, and we must choose whether or not to use it. Christ wants to use our hands, wounded as they may be, to extend his forgiveness to the world. Will they be closed, or outstretched like his?</p>
    <!-- real end-->
    
    
    
  </section>

</div> <!-- /.container -->
