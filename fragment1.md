[[include :scp-wiki:component:hoverlinks]]

[[include :scp-wiki:theme:black-highlighter-theme]]
[[include :scp-wiki:theme:minimalist-bhl]]
[[module css]]
/* Minimalist BHL modifications */
/* Recover default selection styles */
::-moz-selection, ::selection {
    background: Highlight; color: HighlightText;
}
:root {
  --lgurl: url(https://scp-wiki.wikidot.com/local--files/scp-9001/analytics_dept_animated.svg);
}
#header h1 a::before { -webkit-text-stroke-width: 3px }
#header h2 span::before { -webkit-text-stroke-width: 2px }
#header::before {
  top: 0.25rem;
  background-size: auto calc(var(--header-height-on-desktop) - .5rem);
  opacity: 0.15;
}
div.page-rate-widget-box { margin-bottom: 0.25rem }

/* Recover Sigma image borders */
div.scp-image-block { border: solid 1px #666; box-shadow: 0px 1px 6px rgba(0, 0, 0, 0.25); }

/* Light theme image captions */
:is(div.image-block, div.scp-image-block) {
  gap: 0;

  :is(.image-caption, .scp-image-caption) {
    background-color: rgb(235, 235, 235);
    color: rgb(var(--swatch-text-general));
    border-top: thin solid #666;
  }
}
[[/module]]

[[module css]]
/* Better image block positioning from component:croqstyle, adapted for BHL */
@media (max-width: 550px) {
  div.scp-image-block:is(.block-right, .block-left) {
    float: none;
    margin-inline: auto;
    max-width: 100% !important;
  }
}

.footnotes-footer, .equation-number {
  display: none;
}
.rotate {
  transform: rotate(-0.5deg);
}
@media (max-width: 550px) {
  .rotate {
    transform: rotate(-0.2deg);
 }
}

#main-content hr {
  height: 1px;
  border-top: 2px solid rgba(0, 0, 0, 0.5);
  border-bottom: 1px solid rgba(0, 0, 0, 0.5);
  margin-block: 1rem;
  background: none;
}

#header-extra-div-1, #header-extra-div-2 {
  background-image: url(https://scp-wiki.wikidot.com/local--files/scp-9001/thread.webp);
  display: block;
  position: absolute;
  height: 10rem;
  aspect-ratio: 1547 / 1220;
  background-size: auto 100%;
  background-repeat: no-repeat;
  top: 0;
}
#header-extra-div-1 {
  transform: translateX(-1.5rem);
  left: 0;
}
#header-extra-div-2 {
  transform: scaleX(-1) translateX(-1.5rem);
  right: 0;
}
@media (max-width: 900px) {
  #header-extra-div-1 {
    transform: none;
    background-position: -1.5rem center;
  }
  #header-extra-div-2 {
    transform: scaleX(-1);
    background-position: -1.5rem center;
  }
}

.hover {
    text-decoration: none;
    border-bottom: none;
    color:blue;
}
.hover:hover {
     text-decoration: none;
    border-bottom: none;
    color:#004c00;
}

.hover span {    display: none;}
.hover:hover span {
    position: absolute;
    display: inline;
    margin: 20px 0px;
    height: auto;
    width: auto;
    background: #FFF;
    border: 1px solid #000;
    color: black;
    padding: 0.5em;
}
.hover:hover span span {
    position: relative;
    margin: auto;
    height: auto;
    width: auto;
    border: none;
    padding: 0;
}

.emergency-update {
  margin-block: 1.5rem;
  padding: 0.75rem 1.5rem;
  border: 0.25rem solid #444444;
  box-shadow: 0px 1px 6px rgba(0,0,0,.2);
  color: #444;
  max-width: 35rem;
  margin-inline: auto;
  position: relative;
}
@media (max-width: 700px) {
  .emergency-update {
    padding-inline: 1rem;
    margin-inline: max(-2.5vw, -1rem);
  }
}
.emergency-update::before, .emergency-update::after {
  content: "";
  height: 0.3rem;
  left: 0;
  right: 0;
  background-image: repeating-linear-gradient(135deg, gold 0ch, gold 1ch, darkgray 1ch, darkgray 1.75ch, gold 1.75ch);
  position: absolute;
}
.emergency-update::before { top: 0 }
.emergency-update::after { bottom: 0 }

.classified-banner {
  display: grid;
  justify-content: center;
  align-items: center;
  justify-items: center;
}
.classified-banner__dept {
  width: 15rem;
  grid-row: 1;
  grid-column: 1;
  opacity: 0.06;
}
.classified-banner__text {
  grid-row: 1;
  grid-column: 1;
  text-align: center;
}

.forum {
  display: grid;
  grid-template-columns: 3rem 1fr;
  max-width: 40rem;
  margin-inline: auto;
  padding-bottom: 1rem;
}
.forum__post {
  border: thin solid #c9c9c9;
  box-shadow: rgba(0, 0, 0, 0.06) 0px 1px 3px, rgba(0, 0, 0, 0.1) 0px 1px 2px;
  grid-column: 2;
  line-height: 1.25;
  position: relative;
  background-color: white;
  color: rgb(51, 51, 51);
  margin-top: 1rem;
}
.forum__post--op {
  grid-column: 1 / span 2;
}
.forum__post-header {
  border-bottom: thin solid #c9c9c9;
  padding: 0.85rem 1.5rem 0.85rem 3.75rem;
  position: relative;
  background-image: linear-gradient(to top, rgb(246, 246, 246), rgb(251, 251, 251));
  color: rgb(51, 51, 51);
}
.forum__post-pfp {
  font-size: 1.1rem;
  font-weight: 500;
  text-align: center;
  color: black;
  background-color: var(--bg, lightblue);
  border: thin solid rgba(0, 0, 0, 0.1);
  border-radius: 99rem;
  aspect-ratio: 1 / 1;
  width: 2.2rem;
  line-height: 2.2rem;
  position: absolute;
  left: 0.75rem;
  top: 50%;
  transform: translateY(-50%);
}
@media (max-width: 550px) {
  .forum__post-email {
    display: none;
  }
}
.forum__post-content {
  padding: 0 1.5rem;
}
/* Vertical line + horizontal branch for replies */
.forum__post--reply::before {
  content: "";
  position: absolute;
  left: -1.5rem;
  top: calc(-1rem - 1px);
  bottom: 0;
  border-left: thin solid #c9c9c9;
}
.forum__post--reply::after {
  content: "";
  position: absolute;
  left: -1.5rem;
  top: 2rem;
  width: 1.5rem;
  border-bottom: thin solid #c9c9c9;
}
.forum__post--reply:last-child::before {
  height: calc(3rem + 1px);
}

.overwatch-order {
  --logo-size: 4rem;
  border: medium solid firebrick;
  background: white;
  color: #444;
  display: grid;
  grid-template-columns: var(--logo-size) 1fr;
  min-height: var(--logo-size);
  border-radius: calc(var(--logo-size) / 2);
  overflow: hidden;
  margin-block: 0.5em;
}
.overwatch-order__content {
  padding-inline: 1em;
  align-content: center;
  background-image: linear-gradient(to right, #f001, #f000);
}
.overwatch-order__content p { margin-block: 0.25rem; }
.overwatch-order__title {
  font-weight: bold;
  font-size: 1.2em;
  line-height: 1.2;
}
.overwatch-order__logo {
  background-color: firebrick;
  img { filter: invert(1); }
}

.project-proposal.blockquote {
  background-color: #d0ebff44;
  --tables-header-txt: var(--swatch-text-general);
  --tables-header-bg: 208, 235, 255;
}
.project-proposal.blockquote :is(div.image-block, div.scp-image-block) :is(.image-caption, .scp-image-caption) {
  background-color: rgb(var(--tables-header-bg));
}
.project-proposal.blockquote .blockquote {
  background-color: #d0ebff88;
  margin-inline: 1rem;
}

.samples {
  display: grid;
  max-width: 38rem;
  grid-template-columns: 16rem auto;
  align-items: center;
  margin-inline: auto;
  border: thin solid grey;
  border-radius: 0.5rem;
  padding: 0 1rem 1rem;
  gap: 1rem 2rem;
  font-style: italic;
  background-color: rgba(0, 0, 0, 0.05);
  box-shadow: 0px 3px 5px rgba(0, 0, 0, 0.1);
}
.samples__header {
  grid-column: 1 / span 2;
  border-bottom: thin dashed currentColor;
}
.samples__image-heading {
  grid-column: 1 / span 1;
  p { margin: 0 }
}
.samples__desc-heading {
  grid-column: 2 / span 1;
  p { margin: 0 }
}
.samples__image {
  grid-column: 1 / span 1;
  overflow: hidden;
  align-self: start;
  border-radius: 0.5rem;
  box-shadow: 0px 3px 5px rgba(0, 0, 0, 0.25);
}
.samples__image .image {
  width: 100%;
  aspect-ratio: 3 / 2;
  object-fit: cover;
}
.samples__desc {
  grid-column: 2 / span 1;
  margin-block: -1rem;
  position: relative;
}
.samples__desc::after {
  content: "";
  position: absolute;
  width: 1.5rem;
  border-bottom: thin dashed currentColor;
  top: 1.75em;
  right: calc(100% + 0.5rem);
}
@media (max-width: 550px) {
  .samples {
    display: flex;
    flex-direction: column;
  }
  .samples__image-heading, .samples__desc-heading, .samples__desc::after {
    display: none;
  }
  .samples__image {
    margin-top: 0.5rem;
  }
}

.o5-8 {
  font-weight: 800;
  color: deeppink;
  position: relative;
  isolation: isolate
}

.o5-8::before {
  content: "";
  position: absolute;
  inset: 0.1em -0.1em;
  background-color: currentColor;
  opacity: 0.05;
  filter: blur(3px);
  border-radius: 0.5ch;
  z-index: -1;
}

body { overflow-x: hidden }
[[/module]]

[[module css]]
/* Ethics Committee block - inspired by SCP-8980 by Yossipossi */

@import url(https://scp-wiki.wikidot.com/local--files/scp-8980/departuremono.css);

.ethics {
  border: medium solid rgb(10, 70, 10);
  background-color: rgba(10, 70, 10, 0.1);
}

.ethics__header {
  background-image: linear-gradient(to right, rgb(12, 80, 12), rgb(8, 60, 6));
  background-color: rgb(10, 70, 10);
  color: white;
  font-family: 'Departure Mono', monospace;
  font-size: 1.5em;
  padding-block: 0.5em;
  text-align: center;
}
.ethics__header img {
  height: 100%;
}

.ethics__content {
  padding: 0.5rem 1rem;
}

.ethics__content .blockquote {
  border-color: rgb(10, 70, 10);
  background-color: rgba(10, 70, 10, 0.1);
}
[[/module]]

[[>]]
[[module Rate]]
[[div_]]
[[size small]]Page 1 of 2[[/size]]
[[/div]]
[[/>]]

[[div class="blockquote classic curved"]]

{{**2007年4月17日、ベリーマン博士による研究発表**}}

I'd like to thank you all for your attendance. I understand your time is precious, ladies and gentlemen, so I'll do my best to make this -- oh, well? Right to it. First slide, please?

　紳士淑女の皆様がた、ご出席に感謝いたします。貴重なお時間を拝借しますので、私もこの発表を--　　--いえ、本題に入りましょうか。　それじゃ、最初のスライドいただける？

So! Consider the cognitohazard agent as traditionally employed by the Foundation to protect both its documents and its facilities. How exactly is it that they work? Next slide.

　と、いうことで！　これまでわれわれ財団は、われわれの記録や施設を守るために認識災害エージェントを運用してきました。では、その仕組みについてはご存知でしょうか？　次のスライドどうぞ。

In terms of visual cognitohazards, it's not as simple as targeting the lateral geniculate nucleus, nor is merely a matter of V2 processing that renders the agent effective. It's many things in conjunction: The brain's phonological and sematic cortexes performing simeosis, the temporal lobe deriving meaning from the image, the mind's processes of recall and memory retrieval working to interpret what the eye is seeing -- it's in exploiting this complex dialogue between regions of the brain where we've historically found success. Next slide.

　まず、視覚的認識災害について考えていきましょう。これは決して単純なものではありません。ただ外側膝状体を狙えばいいというわけでも、第二次視覚野による認識災害エージェントの処理の問題というわけでもありません。多くのことが、同時に起こっているのです。大脳の音韻野および意味野が記号過程を辿り、側頭葉が画像から意味を抽出し、われわれは無意識のうちに記憶を思い返し、それに基づいて目で見たものを解釈しようとする。脳の複数領域に渡る、この極めて複雑な対話を、われわれはこれまである種悪用してきたのです。そしてそれは、一定の成功を収めています。次のスライドどうぞ。

Though there's been good work done over the years, insofar that we have agents that can influence behavior, render viewers unconscious, or outright induce a grand mal seizure, visual cognitohazards have their limits.

　長年の素晴らしい研究の結果、われわれは視覚を通じて様々な認識災害を起こすことができます。行動に影響を及ぼしたり、失神させたり、あるいは問答無用の大発作を引き起こしたり。どれも大変結構です。が、従来の視覚的認識災害にはやはり限界があります。

By a show of hands, are any of you familiar with Sumerian cuneiform?

　皆様の中にシュメールの楔形文字がわかる方は--　　--手を挙げてくださる？

Excellent. Next slide, please?

　素晴らしいですわ。では次のスライドを。

[[div class="scp-image-block block-center" style="width: 100%"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/remember_us_cuneiform.webp]]
[[/div]]

Haha! Bit of a jumpscare for some of you, huh? You must be read-in to the SCP this cognitohazard protects, and I'm sure the wheels are beginning to turn. For our more stone-faced members: the cuneiform you see in the upper-right quadrant of this image, in normal circumstances, would say "remember us" in English bordered on either side by ellipses.

　ごめんあそばせ！　ちょっと驚かせちゃったかしら？　これが保護しているSCPに対するアクセス権をお持ちの方なら、もうピンと来てることでしょう。ですが何が何やらという方のために、少し補足させてもらいます。この画像の右上あたりにある楔形文字は、英語で言うところの「remember us」という意味で、このフレーズは両側を三点リーダで挟まれています。

Yes? Ah! No, don't worry -- if that were the case, it'd be an infohazard. Don't worry about intentionally picturing it in one's mind's eye; imagination is merely simulation, and an imperfect one at that. You'd need to directly visually process it in totality for it to be effective. **That** is our limitation.

　はい？　いいえ、ご心配なさらず。もしそれがそうであるとしたら、これは情報災害です。もし元の画像を心の中で描いてしまったとしても、大丈夫です。想像とは模擬にすぎません。それゆえに不完全なのです。この効果を発揮するためには、直に視認しなければならないのです。これこそが、われわれの限界です。

Even in cases where text does not contribute to the presentation of the cognitohazard, one still has to account for identity, for culture. This is all to say: perception is inherently subjective, and thus there is no //objective// means through which to effectively convey a cognitohazard.

　テキストが認識災害の発現に関わらない場合も、われわれは対象のアイデンティティや、文化的背景を考慮しなければなりません。つまるところこうです。認識とは、本質的に主観的であり、客観的な認識災害をもたらす手法は存在しない……。

Until today. Next slide, please.

　ですが、それも今日までです。次のスライドを。

[[div class="scp-image-block block-center" style="width: 100%"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/langfordfractal.webp]]
[[/div]]

Everyone, please! Please! It's alright. Director? Director, please, calm down. Look around you -- everyone is unharmed. Let's get off this slide.

　皆さま！　大丈夫！　大丈夫ですから！　管理官？　どうぞ冷静になって。誰も傷ついていませんよ。さっさと次のスライドに行きましょう。こんなもの見てられませんからね……

What you just saw was a visualization from a fractal mathematical set, an image that instills in its viewers a mild sense of dizziness. I understand this in itself is not impressive, but what is notable is its versatility. This image achieves a 100% efficacy rate amongst human volunteers, vastly outperforming the previous 61% record. It has even expressed its effects to some degree in animal testing. This is the real deal.

　たった今皆さまがご覧になったのは、数学におけるフラクタル集合を視覚化したものです。これを視認した者は、少し目眩のような感覚を覚えるはずです。この効果自体は、大したものではありません。真に特筆すべきは、万能性です。人間の志願者に対して、この画像が100%の有効性を示しました。これまでの最高記録記録であった61%など、もはや比較にもなりません。動物に対する試験においてさえも、一定の効果を示しています。どうですか。モノが違うでしょう。

Future memeticists need not be concerned with trivialities such as //'context'// and //'culture'// -- mathematics is absolute. Think of it: fractals are a universal component of nature, underpinning reality itself! From the infinitesimal expression of bacterial proteins to the macroscopic ordered chaos of the universe itself, it all comes down to the complex interplay of numbers and figures; the interdimensionality of fractal systems. The language of the universe.

　未来のミーム学者は、もはや「文脈」や「文化」などという些事に囚われる必要はないのです。数学こそが絶対です。考えてもみてください。フラクタルは、自然の普遍的構成要素です。現実そのものの基礎となっているのですよ！　細菌タンパクなどのミクロの世界から、宇宙全体の秩序ある混沌といったマクロ世界まで、全て結局は数字と図形の複雑な相互作用--　　--つまりフラクタルの多次元性であって、それこそが宇宙の言語なのです。

What you've seen today is much, much less than a mere tip of the iceberg. The fractal space is infinite, and we've barely begun exploring it -- and I'm looking for computer science expert collaborators to help me explore it even faster.

皆さまが本日目撃したものは、氷山の一角のさらに隅にすぎません。フラクタル空間は無限です。そしてわれわれは、その中に立ち入ったばかりです。そして私はいま、共同研究者として計算機科学の専門家を求めています。フラクタル空間の探索を、より早めるために。

Today you have //felt// the utility of my work. We have only scraped the surface, ladies and gentlemen. Together, let us discover its depths.

本日、皆さまはこの研究の実用性を肌で感じたことでしょう。ですが、これは極めて表層的なものです。ここにおられる紳士淑女の皆さまがたと共に、その深みまで行けることを期待しております。
[[/div]]

-----

[[table style="border: none; width: 100%;"]]
[[row]]
[[cell]]
[[size 125%]]**アイテム番号:** SCP-9001[[/size]]
[[/cell]]
[[cell style="text-align: right;"]]
[[size 125%]]###990000|**レベル4/9001**##[[/size]]
[[/cell]]
[[/row]]
[[row]]
[[cell]]
[[size 125%]]**オブジェクトクラス:** Thaumiel[[/size]]
[[/cell]]
[[cell style="text-align: right;"]]
[[size 125%]]###990000|**機密**##[[/size]]
[[/cell]]
[[/row]]
[[/table]]
-----
[[div class="scp-image-block block-center" style="width:100%;"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/controlroom.webp alt=""]]
[[div class="scp-image-caption"]]
サイト・ロメロ-5。SCP-9001の生産拠点。
[[/div]]
[[/div]]

-----

**Special Containment Procedures:** Once per quarter, Fractal Cognitohazardous Images (FCI) produced through SCP-9001 are to be forwarded via dedicated secure fiber-optic cable to Protected Site-7. All FCIs must be transmitted alongside research data describing the effects of each image. These packages are to be analyzed by second-generation [[span class="hoverlink"]][[[aiad-homescreen|AIC]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Artificially Intelligent Conscripts[[/span]][[span class="hoverlink-text"]]Sentient digital agents developed by the Artificial Intelligence Applications Division (AIAD). AICs operate by a loose set of Standard Principles that ensures they adhere to Foundation protocol and work in the interest of the organisation at all times. [[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/aiad-homescreen/itlogo3.png/small.jpg)"]]-[[/span]][[/span]][[/span]] to corroborate their stated effects and catalogue according to their intensity.

**特別収容プロトコル:** 四半期に一度、SCP-9001によって生成されたフラクタル的認識災害画像(FCI)は、各画像の効果を記述した研究データと共に、専用かつセキュアな光ファイバケーブルを通じて、プロテクション・サイト-7へ転送されます。
これらのパッケージは、第二世代[[span class="hoverlink"]][[[aiad-homescreen|AIC]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]人工知能徴募員[[/span]][[span class="hoverlink-text"]]人工知能適用課(AIAD)によって開発された、意識をもつデジタル・エージェント。AICは、緩やかに定められた一連の「標準原則」に基づいて稼働する。この原則は、彼らが常に財団のプロトコルを遵守し、組織の利益に沿って行動することを保証するものである。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/aiad-homescreen/itlogo3.png/small.jpg)"]]-[[/span]][[/span]][[/span]]によって分析され、記述された効果を実際に確かめた後、その強度に応じてカタログ化されます。

Catalogued FCIs and their innoculants, if any, are to be individually contained on isolated external hard drives in Protected Site-7's Secure Data Storage. Third-Order and Second-Order FCIs may be requisitioned by personnel with Level 3 clearance for research, testing, field use, and D-Class procurement.

カタログされたFCI、およびそれに対する免疫となる画像は、プロテクション・サイト-7のセキュアなデータ・ストレージ内の、隔離された外付けハードドライブに保管されます。
第三級及び第二級FCIは、レベル3以上のクリアランスを持つ職員による請求のもと、研究、実験、実地使用、及びDクラス職員の調達を目的として利用されます。。

First Order FCIs require Level 5 clearance with additional authorization from no fewer than three signatories, including the director of RAISA and at least two members of the O5 Council. All personnel read-in to SCP files and Top Secret documents protected by First Order FCI are to be given access to the necessary innoculants. FCIs are not to be handled by any personnel with a CRV[[footnote]] "Cognitive Resistance Value" - The metric which determines one's ability to withstand exposure to mind-altering sensory effects.[[/footnote]] rating of less than 9.5.

第一級FCIの利用には、レベル5クリアランスに加え、RAISA長官及び2名以上のO5評議会メンバを含む、三名以上の署名による追加の認可を必要とします。第一級FCIによって保護されているSCPファイル及び最高機密文書へのアクセス権を持つすべての職員に対して、必要な防疫措置が提供されます。
また、CRV[[footnote]]「認知抵抗値」--　　--精神に変容をきたす効果への暴露に対し、個々人が持つ耐性を測定するための指標。[[/footnote]]が9.5以下の職員は、FCIを扱うことが禁じられています。

To prevent unauthorized viewing, distribution, or theft, FCIs are to be stored with quantum-proof encryption (currently AES-256) viewable only through a dedicated file-embedded module or standalone window application. Each encrypted FCI is to be uniquely keyed (currently with NIST FIPS 203, ML-KEM-1024) to be viewable only in its corresponding per-file embed or per-user window. The modules and windows employ protections against copy-pasting, screenshotting, and other capture methods. Analog printing or reproduction of FCI requires approval from the O5 Council, registration, and tracking.

不正な閲覧、配布、盗難を防ぐため、FCIは耐量子暗号化(現在はAES-256を使用)を施した上で保管され、専用の埋め込み型モジュールまたはスタンドアロン・ウィンドウ・アプリケーションを通してのみ閲覧可能とされます。暗号化された各FCIは、対応するファイルごとの埋め込み、またはユーザごとのウィンドウにおいてのみ閲覧可能となるよう、一意なキー設定(現在はNIST FIPS 203, ML-KEM-1024を使用)がされます。

Per Ethics Committee mandate, files containing First Order FCI are each to be preceded by a warning regarding their presence. Due to the internal prevalence of their colloquial terminology in the wake of Incident-9001-1, such warnings are to refer to First Order FCI in common parlance: "Berryman-Langford Kill Agents".

倫理委員会の指定に基づき、第一級FCIを含むすべてのファイルは、その存在に関する警告を冒頭に付与される必要があります。インシデント9001-1を受け、財団内部においては第一級FCIを指す口語的用語が普及しました。そのため、当該警告文においては、その通俗的な表現である「ベリーマン=ラングフォード・ミーム殺害エージェント」という呼称を使用してください。

[[div class="emergency-update"]]

[[=]]
+ ATTENTION

Special Operatives and Task Force Agents assigned to the ongoing SCP-9001-A crisis are advised to continue through to the second page of this file.

現在進行中のSCP-9001-A変乱にアサインされている特殊工作員および任務部隊員は、このファイルの2ページ目まで閲覧することを推奨されています。

[[/=]]
[[/div]]

 _

[[div class="scp-image-block block-right" style="width: 300px"]]
[[html]]
<video autoplay muted loop width="300" playsinline poster="https://scp-wiki.wikidot.com/local--files/scp-9001/fractal-pentazoom-fallback.webp">
<source src="https://scp-wiki.wikidot.com/local--files/scp-9001/fractal-pentazoom-vp8.webm" type="video/webm">
<img src="https://scp-wiki.wikidot.com/local--files/scp-9001/fractal-pentazoom-fallback.webp" width="300" style="display: block">
</video>
<script>
  const video = document.querySelector("video")
  if (window.matchMedia("(prefers-reduced-motion: reduce)").matches) {
    video.removeAttribute("autoplay")
    video.controls = true;
    video.pause()
  }
</script>
[[/html]]
[[div class="scp-image-caption"]]
Visual traversal of a dead region within SCP-9001 exhibiting no anomalous effects.
SCP-9001の失活領域の実例。この領域は異常な効果を示さない。
[[/div]]
[[/div]]

**Description:** SCP-9001 is the Berryman-Langford set: an algorithm that, while mathematically sound and relatively simple, is capable of generating visual cognitohazards. Computer-generated visualizations of SCP-9001 produce patterns with intricate levels of detail similar to that of the Mandelbrot set; the anomalous nature of SCP-9001 becomes apparent in that these depictions contain innumerable points/still frames that impart a variety of anomalous effects. These include:

* Subliminal [Third Order]:
 * Imagery which influences neurotransmitters in order to compel behavior.
* Deleterious [Second Order]:
 * Imagery which induces physical effects such as nausea, seizure, and unconsiousness.
* Fatal [First Order]:
 * Imagery which triggers intracranial aneurysms leading to immediate death.

**説明:** SCP-9001は、ベリーマン=ラングフォード集合です。これは数学的に健全かつ比較的単純なアルゴリズムでありながら、視覚的な認識災害をもたらす能力を持ちます。コンピュータを用いて描画されたとき、SCP-9001はマンデルブロ集合に類似した自己相似図形を示します。
SCP-9001の異常性は、その描画の中に含まれる、種々の異常な効果を示す無数の点や静止画において発現します。以下に、その異常な効果の例を挙げます。

* 識閾下 [第三級]
 * 行動を強制するために、神経伝達物質に影響を与える画像。
* 有害 [第二級]
 * 吐き気、発作、意識喪失などの身体的効果を誘発する画像。
* 致死 [第一級]
 * 即死に至る頭蓋内動脈瘤を誘起する画像。

[[div class="blockquote"]]
In more detailed terms, the human visual system can be expressed as the abstract equation [[$ f(x)=y $]], where [[$ x $]] is an image matrix (cone and rod cells in the eye, analogous to pixels for a computer), [[$ f $]] is a function that takes [[$ x $]] as input which expresses the brain's internal processing, and [[$ y $]] is the output of how the brain interprets the image. SCP-9001 is the result of a convex optimization searching over the field of possible images for an [[$ x $]] to produce a target neural output [[$ y $]] resulting in a desirable effect.
[[>]]
//Dr. Langford, Project HYDRA Senior Researcher//
[[/>]]
[[/div]]

[[div class="blockquote"]]
より専門的な語を用いてみよう。抽象的にいえば、人間の視覚システムは[[$ f(x)=y $]]なる関数として表現することができる。このとき[[$ x $]]は画像行列(ディスプレイのピクセルに類似する、眼球内の錐体細胞および桿体細胞)、[[$ f $]]は[[$ x $]]を入力として受け取る関数(脳内における処理)、[[$ y $]]は脳がその画像をどう解釈したかの出力である。
望ましい効果をもたらす標的ニューラル出力[[$ y $]]を生成するための[[$ x $]]を、可能な画像の領域にわたって探索する「凸最適化」こそが、SCP-9001である。
[[>]]
//HYDRA計画上席研究員、ラングフォード博士//
[[/>]]
[[/div]]

Beyond the intricate geometric patterns found within visual depictions of typical fractal sets (including swirls, intersecting lines, and self-similar shapes), FCIs derived from the Berryman-Langford set have multiple points that form markers and superstructures visually implying the presence of biological features (such as tendrils, feathers, scales and faces) despite the mathematical purity of the generation procedure. The implications of this remain unknown, but the prevailing theory is that this can be accounted for as simple pareidolia.

一般的なフラクタル集合の視覚的描写に含まれる複雑な幾何学的パターン(渦巻、交差線、自己相似図形など)に加え、数学的に純粋な手段によって生成されているにも関わらず、ベリーマン=ラングフォード集合から派生したFCIには、生物学的な特徴(触手、羽毛、鱗、顔など)の存在を視覚的に示唆するマーカーや上位構造を形成する、複数の「点」が存在します。
詳細な原因は不明なものの、最も有力な仮説において、この現象は単純なパレイドリアによるものであるとされています。

While SCP-9001 was adopted with a focus on human subjects, FCIs have produced results with non-human animals. Third and Second Order FCIs show less utility due to simpler brain function, but First Order FCIs have proven efficacy in all primates and most mammals, as well as many species of arachnids.

SCP-9001は、人間の被験者に焦点を当てて採用された一方で、FCIは人間以外の動物に対しても有効性を示しています。人間以外の動物を対象とした場合、その脳機能の単純さにより、第三級及び第二級のFCIは期待された効果を示さない傾向にあるものの、第一級FCIは、すべての霊長類とほとんどの哺乳類、ならびに多くのクモ類の種において有効性が認められました。







 _

 _



[[=]]
+++ __歴史__
[[/=]]

[[div class="classified-banner"]]
[[div class="classified-banner__dept"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/analytics_dept_animated.svg]]
[[/div]]

[[div class="classified-banner__text"]]
SCP-9001

以下のファイル群は
[[size 133%]]分析部門**HYDRA計画**[[/size]]
に関連し、閲読には**3/HYDRA**クリアランスを要す。

無許可のアクセスを禁じる。
[[/div]]
[[/div]] [!-- .classified-banner --]

+++ 2007年、4月

On 2007-04-17, Dr. Ava Berryman led a presentation on the cognitohazard production aspect of Project HYDRA to a much wider range of staff than had previously been aware of it, with the intention of attracting personnel to the project with the skillset necessary for its advancement.

2007年4月17日、エイヴァ・ベリーマン博士はHYDRA計画における「認識災害生成」についてのプレゼンテーションを行なった。このプレゼンテーションは、計画の実行に必要な技能を持つ人材を発掘することを目的としていた。本計画の存在を把握していないスタッフも、多数出席した。

Amongst attendees was one Dr. Robert Langford, a computer science researcher within the Department of Analytics, who at the time was working on the detection of cognitohazards via machine learning as part of [[span class="hoverlink"]][[[scp-3334|Project CIRCE]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Project CIRCE[[/span]][[span class="hoverlink-text"]]A Department of Analytics effort to use AI techniques to detect visual cognitohazards. Project CIRCE leveraged convolutional neural networks, an architecture modeled off the human vision system. After advances in reinforcement learning and natural language processing, it was succeeded by Project MEDUSA in order to unify efforts to classify visual memetic hazards as well.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wikidot.com/local--files/scp-9001/circe.webp)"]]-[[/span]][[/span]][[/span]]. Several days later, he proposed to meet Dr. Berryman to offer his expertise, and would be flown to Site Romero-5 to meet with her.

その出席者たちの中に、一人の男がいた。ロバート・ラングフォード博士は解析部門に所属する、計算機科学の研究者であった。当時は[[span class="hoverlink"]][[[scp-3334|CIRCE計画]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]CIRCE計画[[/span]][[span class="hoverlink-text"]]解析部門による、AI技術を用いた視覚的認識災害の検出を目的とした試み。本計画においては、人間の視覚システムをモデルとしたアーキテクチャである「畳み込みニューラルネットワーク」を活用していた。強化学習および自然言語処理の発展を受け、視覚的ミーム災害の分類も目的とすることになったため、MEDUSA計画が本計画を引き継いだ。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wikidot.com/local--files/scp-9001/circe.webp)"]]-[[/span]][[/span]][[/span]].の一環として、機械学習による認識災害の検出に取り組んでいた。

[[div class="blockquote" style="margin-bottom: 1rem"]]

[[include component:image-block
| name=https://scp-wiki.wikidot.com/local--files/scp-9001/langford.webp
| caption=ラングフォード博士。ベリーマン博士の研究室にて撮影。
| width=300px
]]

**映像記録9001-1**

**関係者:**
* エイヴァ・ベリーマン上席研究員(神経学者、ミーム学者。サイト・ロメロ-5所属)
* ロバート・ラングフォード研究員(AI研究者。解析部門所属、CIRCE計画メンバー)

**はしがき:** のちにSCP-9001となるプロジェクトに関する、初期の会話。

**〈記録開始〉**

//Dr. Langford enters Dr. Berryman's office. Dr. Berryman is watering a substantial collection of flower bouquets and a leafless bonsai tree on some wooden cabinets. She turns to greet him.//

ラングフォード博士がベリーマン博士のオフィスへ入る。ベリーマン博士は、木製のキャビネットの上に置かれた多数の花束と、葉の落ちた盆栽に水をやっている。彼女は振り向いて、ラングフォード博士に挨拶をした。

**Dr. Berryman:** Dr. Langford, how do you do?

**ベリーマン博士:** ごきげんよう、ラングフォード博士。

**Dr. Langford:** Um, well.

**ラングフォード博士:** あ……どうも。

//They shake hands.//

両名は握手をする。

**Dr. Berryman:** Why don't you have a seat, my dear fellow. I'm glad we could find time for this conversation. I quite enjoyed your and Dr. Reddy's presentation on the use of neocognitrons[[footnote]]Archaic term for convolutional neural networks, used for AI computer vision.[[/footnote]] for detecting cognitohazards.

**ベリーマン博士:** ささ、どうぞお座りになって。こうやってお互いにお話しできる時間がうまいこと見つかってくれて嬉しいわ。ネオコグニトロン[[footnote]]畳み込みニューラルネットワークのことを指す、古い用語。AIコンピュータを展望する際に用いられた。[[/footnote]]を用いた認識災害の検知についてのプレゼン、あれは面白かったわね。あなたがレディ博士と一緒にやったやつ。

**Dr. Langford:** Thank you, Dr. Berryman. I've watched a few of your lectures myself, including your latest, and I'd also have to say they're quite groundbreaking. I'm honored that you liked mine and Dr. Reddy's so much -- although really, to give credit where it's due, Dr. Reddy was the brains behind the work. I've only been here for a few years.

**ラングフォード博士:** ありがとうございます、ベリーマン博士。ぼくもあなたの講義を何件か拝見しました。もちろん、例のやつも。本当に画期的な内容だと思いますよ。それから、レディ博士とぼくの講演も気に入ってくださって嬉しいです。ですが実際、あれの功績はレディ博士に帰すべきです。彼女こそがあの研究のブレインですから。ぼくなんか、ここに来てまだ数年ですし。

**Dr. Berryman:** Talent and experience are fungible to a degree. I admire Dr. Reddy, but she's… she has her own ideas about things, let's just say.

**ベリーマン博士:** 才能と経験は可換よ。ある程度はね。レディ博士は確かに凄い人だけれど……まあ、人には人の考え方があるってことね。あんまり強くは言えないけど。

//Dr. Langford does not immediately respond. Dr. Berryman hovers her fingers over the cluster of tiny white flowers pinned to her hair.//

ラングフォード博士は返答に詰まる。ベリーマン博士は、彼女の髪に挿さっている小さな白い花の束に軽く触れた。

**Dr. Berryman:** I see these have caught your attention, Dr. Langford.

**ベリーマン博士:** どうしてもこのお花が気になるようね。ラングフォード博士？

**Dr. Langford:** Um… yes. My apologies.

**ラングフォード博士:** ええ、少々……失礼しました。

**Dr. Berryman:** It's only natural. Carrot flowers, or as the Yankees call them, Queen Anne's Lace. They grew on the estate where I was raised. To me, their most interesting feature is that they grow in recursive layers of flower shapes: each flower grows in a flower-shaped bunch, and the bunches themselves form a larger flower shape. That self-similarity carries a fractal structure, like my research. But ah, where's my manners? Allow me to offer you a drink first before we get into the weeds.

**ベリーマン博士:** 当たり前の反応ね。これは人参の花。アメリカじゃこれを「アン女王のレース」なんて呼ぶらしいわ。小さい頃に住んでた場所に、よくこれが生えてたの。私にとって一番面白いのは、この花が同じ形を繰り返しながら咲くこと。一輪一輪が集まって花の形をした房になって、さらに大きい目で見てやると、房自体もさらに大きい花の一部になっている。つまり自己相似構造を持っているということ。わたしの研究のようにね。あらやだ。私ったらとんだ無作法ね。小難しい話を始める前に、まずは一杯どう？

//Dr. Berryman retrieves a bottle of scotch, two glasses, and some ice cubes from a drawer. She pours out the two glasses and reaches over to place one in Dr. Langford's hand.//

ベリーマン博士は、机の引き出しからスコッチの瓶と二つのグラス、それに幾つかの氷を取り出した。彼女はグラスに酒を注ぎ、うち一つをラングフォード博士に手渡した。

**Dr. Langford:** I'm quite alright, Dr. Berryman.

**ラングフォード博士:** ぼくは大丈夫です。ベリーマン博士。

**Dr. Berryman:** Please, I insist. We both work with mind-altering phenomena far worse than this. Humans think their beans so secure, ensconced in their thick skulls, when all it takes to throw it off balance is just a little drink, a little smack, perhaps just the right kind of little picture…

**ベリーマン博士:** お願い。ぜひ飲んで。私たちこんなものよりずっと酷い精神変容現象を扱ってるんだから。脳みそって頭蓋の中にあるから安全だって、人間はそう思ってるみたいだけど、ちょっと飲んだり、ちょっとどついたり、あるいはちょうどいい画像なんか見せたら、あっという間にバランスを崩しちゃうんだから……

//Dr. Langford hesitates, then takes a sip.//

ラングフォード博士は躊躇い、そして一口飲む。

**Dr. Berryman:** No, not yet!

**ベリーマン博士:** まだ。まだダメよ！

**Dr. Langford:** But you told me--

**ラングフォード博士:** でもあなたが飲めって--　　--

**Dr. Berryman:** This is quality Macallan, you need to aerate it and... oh, dear, I'm so sorry. You've not tried scotch before, have you?

**ベリーマン博士:** これ、ちゃんとしたマッカランよ。まずは空気に触れさせて--　　--あら、ごめんなさいね。スコッチは初めてだったかしら？

//Dr. Langford nods.//

ラングフォード博士は頷く。

**Dr. Berryman:** Well, cultural context //is// everything, I suppose -- as I'm sure you remember, actually. There have always been plenty of "non-anomalous" cognitohazards: war photography, political propaganda, pornography. So far, most prior work, and my colleagues', have focused on this avenue, engaging the higher functions of the brain's temporal lobe to make anomalously emotional, anomalously disgusting, anomalously meaningful cognitohazards… but it never works on everyone in the same way to the same degree.

**ベリーマン博士:** 文化的背景こそが全てなのよ。つまり--　　--あなたも知っているはずだけれど、非異常の認識災害なら山ほどあるでしょう？　戦争写真とか、政治プロパガンダとか、ポルノグラフィとか……。これまでの研究も、私の同僚も、この方向性でやってきたのよ。つまり側頭葉の高次機能を刺激して、異常に感情的にしたり、異常なほど嫌な気分にさせたり、異常な意味を感じさせる認識災害だったり……でも、これが全員に同じように、同じ程度に効くことは決してないのよね。

**Dr. Langford**: Because non-universality of human experience is the one universal.

**ラングフォード博士:** 経験の非普遍性こそが、唯一普遍のものですから。

**Dr. Berryman:** Absolutely, Dr. Langford, and I'm so glad that you can recognize this stumbling block so quickly when so many of my colleagues can't… but anyway, I personally think there is another approach. There is another potential universal: everyone sees -- well, at least tautologically, those who //can// see. Everyone can detect edges, recognize rough and smooth surfaces, outline curves. We all must share //some// universal features at the lowest levels of the visual cortex. The optic nerve is a direct chain into the brain that we can //yank//, and the closer to the eye the less tangled it is.

**ベリーマン博士:** その通りよ、ラングフォード博士。こんなにも早く、この障害に気づいてくれて嬉しいわ。私の同僚なんか、ほとんど気にも留めてくれないのに……。ともかく、別のアプローチがあると思うの。普遍的になりうるもの--　　--それは見ることよ。けったるい言い方になるけど、見ることができる人は見ることができるじゃない？　何かの端っこを認識して、表面がざらついてるか滑らかかもわかって、曲線を描くことだって、誰もができる。視覚野の奥底に、我々誰もが持つ共通の何かがあるに違いないわ。視神経って、直接脳に繋がってるでしょ。そこをぐいっと行くのよ。目に近ければ近いほど、単純だし。

**Dr. Berryman:** We already know it's possible! In epileptics, high-frequency flashes translate directly into high-frequency electrical neuron signals directly into seizures. But, alas, it doesn't work on everyone. Images that trigger an extreme end-state in the brain, the principle, is there, if only we knew how to trigger it more generally. I've mapped the whole house, and just need to find the door -- so, Dr. Langford, tell me: can you help me?

**ベリーマン博士:** それが可能だってことはもうわかってるの！　てんかん患者がいい例ね。高周波のストロボは、そのまま高周波の電気信号となって発作を引き起こすの。でも残念なことに、これも全員に効くわけじゃない。脳の極端な終末状態を引き起こすような画像は、少なくともその原理は確かに存在してるのよ。ただ、それを普遍的に引き起こす方法がわからないだけで……家の間取りはわかってるけど、ドアの場所がわからないみたいな状況ね。ねえ、ラングフォード博士。教えてちょうだい。あなたは、私を助けてくれる？

**Dr. Langford:** Hmmm, well, my first thought is that your issue is fundamentally something akin to data compression. The brain and its billions of neurons are such a high-dimensional object. Trying to cram the trigger for a specific brain-state into a small image would be Herculean.

**ラングフォード博士:** ええと……ああ。まず最初に、データの圧縮が根本的な問題だと思いました。そもそも脳は数十億のニューロンが集まってできている、非常に高次元な物体です。画像を見せるだけで、脳の特定の状態を引き起こすと言うのは、途方もないことですよ。

**Dr. Berryman:** There is a way to compress the infinite into the finite.

**ベリーマン博士:** 無限を非有限に圧縮する方法は、あるはずだけど。

**Dr. Langford:** Not as a compression algorithm, in my experience. Are you thinking of a mathematical function or a generator instead, perhaps?

**ラングフォード博士:** ぼくの経験上、圧縮アルゴリズムでそれをやるのは無理です。なにか数学的な関数か、生成器のようなものをお考えなのですか？

**Dr. Berryman:** Yes, but we're looking to convey something visual. Something even denser, even more intricate.

**ベリーマン博士:** そうね。でも我々は、視覚的な何かを伝達しようとしているのよ。もっと緻密で、複雑な何かを。

//Dr. Berryman picks up a writepad from her desk and writes an equation on it.//

ベリーマン博士はデスクからメモ帳を取り、そこに方程式を書き込む。

[[math]]
z_{n+1}=z_n^2+c
[[/math]]

**Dr. Langford:** This is the Mandelbrot set in the complex plane, isn't it? One of the first fractals.

**ラングフォード博士:** 複素平面における、マンデルブロ集合を表した式ですね？　最初期のフラクタルだ。

**Dr. Berryman:** Well said, Dr. Langford. An entire universe of infinite detail, infinite complexity, encoded into a single equation of three terms. A well with no bottom, an ocean with no floor, a fall with no end. Even our physical universe has an end, a minimum, a digital pixelation: the Planck length. In some deep sense, a fractal is more real than reality.

**ベリーマン博士:** 正解よ、ラングフォード博士。たった三項の短い方程式に、宇宙そのものの無限のディテールと無限の複雑さが詰まっているの。さながら、底なき井戸、奈落の海、永遠の落下……。この宇宙にすら、プランク長という終わりが、最小単位が、デジタルなピクセル化があるというのにね。フラクタルは現実よりももっと「本物」なのよ。

**Dr. Langford:** I'll grant you that's intriguing, but humans are more visual than explicitly mathematical. Even anoraks like us don't actually calculate fractals in our heads.

**ラングフォード博士:** ええ、実に興味深いですね。ですが、人間は数学的というよりも、むしろ視覚的な存在です。ぼくらのようなオタクですら、頭の中でフラクタルを計算したりはしないでしょう。

**Dr. Berryman:** I imagine football players don't look fondly on their high school physics classes, and yet they calculate the trajectories of their balls all the same. Have you ever read the book //The Little Prince//?

**ベリーマン博士:** 確かに、フットボール選手が高校物理の授業をいちいち復習してるってわけじゃないと思うけど、それでも彼らはボールの軌道を計算してるでしょ。『星の王子さま』って読んだことある？

//Dr. Langford shakes his head.//

ラングフォード博士が首を横に振る。

**Dr. Berryman:** It's a nice story, I recommend it. But the relevant part is when the Little Prince asks the narrator to draw him a sheep. He draws successively less realistic sketches until finally, in exasperation, the narrator just draws a box and claims the sheep is inside. But though you can't see it directly, in your mind's eye, you can still see the sheep in the box, can't you?

**ベリーマン博士:** いい話だから、ぜひ読んでみて。ここで重要なのは、王子さまが語り手に羊を描いてくれと頼んだパートよ。彼は何回か描いてみたけど、どうにもリアルにならなくって。それで仕舞いには、半ばヤケになって「羊の入っている箱」を描いたの。たとえ見えなくても、心の目を使えば、箱の中に羊がいることはわかるでしょ？

**Dr. Langford:** Of course.

**ラングフォード博士:** わかるね。

**Dr. Berryman:** Your brain isn't seeing though. It's imagining. It's //calculating//.

**ベリーマン博士:** でも、脳そのものは見ているわけじゃないの。想像して、計算してるのよ。

**Dr. Langford:** Decompression.

**ラングフォード博士:** データの解凍。

**Dr. Berryman:** Exactly.

**ベリーマン博士:** その通り。

**Dr. Langford:** But you can't do that with fractals. A sheep, sure, but an infinitely complex fractal? It's completely different!

**ラングフォード博士:** でもフラクタルでそれはできませんよ。羊ならわかりますが、無限に複雑なフラクタルじゃ……何もかもが違いますよ！

**Dr. Berryman:** Are you familiar with MKULTRA?

**ベリーマン博士:** じゃあMKULTRAって知ってる？

**Dr. Langford:** The American CIA project where they gave a bunch of people hallucinogenic drugs?

**ラングフォード博士:** 米国中央情報局の、多数の人に幻覚剤を投与したプロジェクトですよね？

**Dr. Berryman:** It was a joint effort with the Foundation Special Projects Division, run by the current O5-8. LSD, DMT, mushrooms.

**ベリーマン博士:** LSDとか、DMTとか、幻覚キノコとかね。あれって実は財団の特殊計画部門との共同だったのよ。今のO5-8が責任者だった。

//Dr. Langford exhales slowly.//

ラングフォードはゆっくりと深呼吸する。

**Dr. Langford:** That… that was //us//? I'm really hoping we had a good reason for //that.//

**ラングフォード博士:** それ……それを、我々が？　さぞ良い理由があったのでしょうね。

**Dr. Berryman:** Of course we did. Did you think they'd declassify the useful findings?

**ベリーマン博士:** もちろんよ。大発見をしたとして、財団がそれを機密解除すると思う？

**Dr. Langford:** Well, what did we find?

**ラングフォード博士:** それで、大発見とは？

**Dr. Berryman:** Fractals. Fractals everywhere. Fractals integrated into the whole field of vision: the ground, the walls, the structures, the tunnels, the so-called "machine elf" entities.

**ベリーマン博士:** フラクタルよ。フラクタルが至る所にあったの。フラクタルが視界全体と融合したのよ。床も、壁も、構造も、トンネルも、いわゆる「機械の妖精」にも。

**Dr. Langford:** Machine elves?

**ラングフォード博士:** 機械の妖精？

**Dr. Berryman:** Let's not get distracted. The important part is-- look, these drugs yank the visual cortex away from physical reality, and what does it imagine, what does it //calculate// instead in its temporary deranged state? Fractals. Of course I had to explore deeper. My own testing confirmed those findings. The neural maps in the low-level striate cortex responsible for the most basic building blocks in vision? Detecting edges, curves, and surfaces? Those building blocks are rotationally symmetric //fractals//.

**ベリーマン博士:** そこはどうでもいいのよ。重要なのはここよ。つまりね、その薬物が視覚野を現実から引き剥がすの。そんな狂いじみた状態で、脳は何を想像して、何を計算したんだと思う？　フラクタルよ。当然、もっと深く探究しなくちゃいけなかった。私の実験でも、その発見は実証されたわ。視覚の基本のさらに基本--　　--端とか曲線、表面を検出する、低次有線皮質の神経マップ--　　--その構成要素こそが、回転対称なフラクタルだったの。

**Dr. Langford:** Stop, stop, hold on a second. You're telling me you looked at everything done in MKULTRA, and your decision was to… //continue// that research?

**ラングフォード博士:** ちょっと、ちょっと。ちょっと待ってください。つまりあなたは、MKULTRAが何をやったかを全部知った上で、それを……その研究を受け継ぐことを決めたのですか？

**Dr. Berryman:** No, no, don't think of it like that. It's standard procedure across the Foundation, after all. I've read the Project CIRCE files and Protocol 10-Kempelen. Even you use D-class to confirm cognitohazards for training data. Why do //you// do it?

**ベリーマン博士:** いや、いや。それは違うわ。結局これも、財団からしたら普通のやり方じゃない。CIRCE計画についても、10-ケンペレン手順についても、私は知ってるのよ。あなただってDクラスを使ってるじゃない。訓練データ用の認識災害を確認するために。

**Dr. Langford:** //That// is for a good reason. What you're talking about is-- is-- you couldn't possibly have done that with Ethics Committee approval.

**ラングフォード博士:** それとこれとは違います。あなたのそれは--　　--それは不可能ですよ。倫理委員会の承認を得た上で、そんなことをするのは

**Dr. Berryman:** But approve they did, Dr. Langford.

**ベリーマン博士:** でも承認されてるわ、ラングフォード。

//Dr. Langford falls silent.//

ラングフォード博士は沈黙する。

**Dr. Berryman:** I'll tell you what I told them, and I hope you find it as convincing as they did. What I propose is not an idle, wasteful science experiment, Dr. Langford, but a revolutionary //tool//. A tool that could have many uses, if it were flexible enough. To protect the Foundation and its data and its personnel and yes, its anomalies, of course, but more than that. Think of a more peaceful world, one protected from the next anomalous cognitohazard via mass distribution of our own protective ones. Think of a reality bender finally going home to hug their family, tears in their eyes -- unthinkable, right? -- after we use a targeted cognitohazard to wipe the anomaly from their brain. Think of the people in your own life, surely at least a few friends or family, whose minds have seen better days and aren't their full selves anymore. Chemicals and pills are no way to treat the brain, harsh mallets that they are. Vision is a system directly tied to it, with far greater granularity.

**ベリーマン博士:** あなたにも教えてあげる。きっとあなたも、倫理委員会と同じように納得してくれるはずよ。あれはお遊びみたいな科学実験なんかじゃないの、ラングフォード博士。あれは道具なの。革命的な道具。十分な柔軟性さえ確保できたら、いろんなことに使えるはずなの。財団や、うちらのデータとか学者たちとか、アノマリーももちろん保護できてしまう。でもそれだけじゃないの。想像してみて。もっと平和な世界を。我々が防護用の認識災害を広く配ることで、さらなる異常な認識災害から守られた世界を。現実改変者がようやく家に帰れて、家族と抱きしめ合うことができるような世界を。彼らの目には、きっと涙が浮かぶことでしょう……想像できないでしょう？　我々の標的性認識災害が、彼らの脳から異常性を消し去ってしまえば、そんなことが可能になってしまうのよ。あなたのこれまでの人生の中にも、そういう人はいたはずよ。友人や家族のうちに、精神の全盛を過ぎ去ってしまって、すっかり変わってしまったような人たちが。薬品や錠剤は、脳を治すには粗暴すぎるわ。あれは力任せの木槌みたいなものよ。けれども視覚は脳に直結しているシステムで、それを使えば遥かに精密な制御が可能になるの。

//Dr. Langford stares into his drink.//

ラングフォード博士は、手中の酒を見つめる。

**Dr. Langford:** Of course I can think of a few such people, and of course I'd very much like to help them.

**ラングフォード博士:** もちろん、そういう人は何人か思い当たりますし、彼らを助けたいとももちろん思っています。

**Dr. Berryman:** We are //this// close to changing the course of human history, from the individual to society, and for the better. My prior work has taken us this far; the end is in sight, just a little bit farther away.

**ベリーマン博士:** あともう少しで、人類史の流れを変えられるところまで来てるの。個人から社会へ、そしてより良い方に向かって。ようやくここまで来れたわ。そして、ゴールはもう目の前。手を伸ばせば届きそうなくらい--　　--。

**Dr. Langford:** You've definitely convinced me of the impact, alright. But let's be realistic: this would be an exceptionally dangerous tool ripe for abuse, even with well-intentioned people like ourselves. The Foundation would keep it under lock and key, and rightly so.

**ラングフォード博士:** 影響力については、よくわかりました。ですが……より現実的な話をしましょう。もし濫用されてしまったら、これは非常に危険な道具になる可能性があります。我々のような善意の人も、当然気をつける必要があります。財団はこの技術を秘匿しますよ。その権限を以って。

**Dr. Berryman:** The Foundation would //supervise// it and ensure only its beneficial use, the same way it does and has done successfully for thousands of other items. We have the Ethics Committee to be sure, as you pointed out. Ultimately there is no containment more profound than explanation. And that is what we will do: not just for the cognitohazards we develop, but for //all// cognitohazards. The "anomalous" is arbitrary, just things we're too small to understand yet, but everything follows rules. I understand some of these rules myself: the rules of the brain, certainly. But I've realized I alone cannot further bridge the gap between the input and the output. I don't know how to turn the brain into a math problem to solve, where the answer is the perfect trigger fractal we're searching for. I certainly can't program. But your AI model, your solving techniques, and your evident insight, these I need to go from understanding to //creation//.

**ベリーマン博士:** むしろ財団は監督して、益をもたらすようにしか使われないように保証するのよ。他の何千というアイテムに対して行なっているのと同じようにね。あなたが指摘した通り、何かがあった時のための倫理委員会もあるわ。言ってしまえば、解明こそが究極の収容よ。そして、それこそが我々のなすべきことなの。我々は、ただ認識災害を作るだけじゃない。全ての認識災害を解明するのよ。「異常」という尺度は極めて恣意的なものね。我々の未熟ゆえに、理解できないというだけなのに。けれども全ては規則のもとに成り立っているの。その規則のうち、私もいくらかはわかってる。たとえば脳のルールとかは、もちろん。でも、入力と出力の間にある差を、私だけじゃ埋められないということに気づいたの。脳そのものを解くべき数学の問題として扱う方法なんか知らないし、完璧なトリガーフラクタルを見つける方法も知らない。プログラムも出来やしないわ。でもあなたのAIモデル、あなたの解法、そしてあなたの明快な洞察力さえあれば、理解から創造へと進むことができる。

//Dr. Berryman leans forward.//

ベリーマン博士は身を乗り出す。

**Dr. Berryman:** Are you with me?

**ベリーマン博士:** ついてこれてるかしら？

//Dr. Langford nods his head.//

ラングフォード博士は頷く。

**Dr. Langford:** I-I'm quite honored you esteem my abilities so.

**ラングフォード博士:** こ、光栄です……ぼくをそんなに評価してくださって。

**Dr. Berryman:** Excellent. I'd like you to transfer to Site Romero-5 and meet with me at least every other day. Let's immediately get to work on a project proposal to submit to O5-8.

**ベリーマン博士:** 素晴らしいわ。あなたにはサイト・ロメロ-5へ転属して、少なくとも隔日で私と会合してほしいの。さて、O5-8へ提出するための計画書を仕上げましょう。

**Dr. Langford:** O… 5? This is serious, then.

**ラングフォード博士:** O……5？　話が変わってきましたね。

**Dr. Berryman:** I can see it in your eyes, Dr. Langford. You want to play in the big leagues, don't you? This is your chance.

**ベリーマン博士:** あなたの目を見ればわかるわ、ラングフォード博士。大舞台に出たいんでしょう。チャンスは目の前にあるわ。

**Dr. Langford:** Of course… let's do it.

**ラングフォード博士:** もちろん……やりましょう。

**<記録終了>**
[[/div]]

[[include :scp-wiki:component:image-block
| align=center
| name=https://scp-wiki.wikidot.com/local--files/scp-9001/romero5.webp
| caption=サイト・ロメロ-5
| width=450px
]]

Shortly after meeting with Dr. Berryman, Dr. Langford voluntarily transferred from Project CIRCE to Project HYDRA, and relocated from Site-15 to Memetics Research Site Romero-5 within a week. Dr. Langford would quickly prove to be a crucial hire for Project HYDRA.

ベリーマン博士との面談の直後、ラングフォード博士は自らの意志でCIRCE計画からHYDRA計画へ移動し、また一週間以内にサイト-15からミーム学研究サイト・ロメロ-5へと拠点を移した。彼はまもなく、彼自身がHYDRA計画にとって極めて重要な人材であることを証明することとなる。

-----

In 2007, the cognitohazard generation algorithm employed a Monte Carlo method to randomly sample the mathematical set discovered by Dr. Berryman, and then generated fractal imagery based on the resulting seed values. While it was the most reliable method known to Dr. Berryman's team at the time, it was not efficient in the slightest, and the vast majority (> 99.9%) of images depicted 'dead regions' of the fractal space with no cognitohazardous effect on observers.

2007年当時、認識災害生成アルゴリズムは、ベリーマン博士が発見した数学的手法に対しランダムなサンプリングを実施する、モンテカルロ法を用いていた。それによって得られたシード値に基づき、アルゴリズムはフラクタルを生成していた。これは、当時のベリーマン博士らのチームが知る中で最も信頼性の高い手法であった一方で、効率性は皆無に等しかった。これによって生成された画像の99.9%以上は、観測者に認識災害的効果をもたらさないような、フラクタル空間における「失活領域」を描写したものであった。

Dr. Langford began by applying a Hessian-approximating optimization algorithm based on machine-learning techniques to augment this process, resulting in small efficiency gains. In doing so, he identified that the Monte Carlo process was fundamentally deficient, and suggested that the team derive the fractal set formulas that defined the space in order to solve them directly. Dr. Berryman had been unaware that this was a possibility, and so Dr. Langford began the task himself.

ラングフォード博士はまず、機械学習に基づいたヘッセ近似最適化アルゴリズムを適用してこのプロセスを補強し、効率をわずかながら向上させた。その過程で、彼はモンテカルロ法が根本的に不完全であることを見出した。それゆえに、彼はチームに対して、フラクタル集合を定義する方程式を導出し、それを直接解くことを提案した。ベリーマン博士はそれが可能であることを認識していなかったため、ラングフォード博士は自身でこの課題に取り組み始めた。

However, Dr. Langford complained on numerous occasions about Dr. Berryman's policy regarding potential exposure of her team to cognitohazards, and this came to a head when he put his thoughts in writing on the Site's internal communications system.

しかしながら、ラングフォード博士は、ベリーマン博士がチームに対して課していた、認識災害への潜在的な曝露に関する方針について、幾度となく不満を漏らしていた。そしてその不満は頂点に達し、彼は自身の考えを、サイトの内部通信システムにおいて文書化した。

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**HYDRA計画の安全手順について**
ロバート・ラングフォード [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Dr. Berryman,

ベリーマン博士

I've only been here a few weeks now, but in that time I've found some practices that, while apparently routine here, deeply trouble me.

ぼくはまだここに来てから数週間ほどです。しかし、ここで日常的に行われている種々の慣習には、非常に大きな問題が含まれていると感じます。

This isn't coming out of nowhere. Project CIRCE was only working on detecting cultural coghaz, but even that necessitated several safety protocols, and I don't feel safe without them. It's like I've stepped into a new workshop and I'm the only one who's heard of a respirator.

ともすれば、このポストを唐突なものだと感じる方もおられるかもしれません。CIRCE計画は文化的認識災害の検出にのみ取り組んでいましたが、それでさえもいくつかの安全手順が必要でした。そして、ぼくはそれらの手順抜きでは、安全を感じることができません。まるで新しい作業場に入った時に、ぼくだけが防塵マスクの存在を知っているかのような気分です。

I don't need to go far to find something that really shouldn't be happening at all. The team is, as standard, looking at the images they generate to see whether they're cognitohazardous or not. That's insanity. We might not have made anything dangerous //yet//, but we will!

決して起こってはならないものとは何か。それをわざわざここで申し上げる必要もないでしょう。標準的な手順として、チームは生成された画像を見て、それが認識災害を持つものかどうかを確認しています。これは狂気の沙汰です。我々は危険なものを作り出しているわけではありません。ですが、いつの日かは生まれるものです。

I must insist that we adopt at least the most essential of those policies:

* HYDRA計画のスタッフは、たとえそれが単なる失活領域だと推測される場合であっても、認識災害生成プロセスの出力を決して視認してはならない。
* 代わりに、全ての潜在的なFCIを、手順10-ケンペレンを介して確認し、分類せねばならない。

少なくとも、このような基本的な方針だけでも採用することを強く求めます。

* Project HYDRA staff must never view the output of the cognitohazard generation process, even if we suspect it's just going to be a dead region.
* Instead, we must confirm and classify any potential FCIs via Protocol 10-Kempelen.

I know that you know of it already, Ava, but for the benefit of everyone else, Protocol 10-Kempelen is a process used by Project CIRCE, where you have a number of D-Class monitored by fMRI scanners, and you show them the cognitohazards and record what effects it has on them. It's a buffer layer between us and the cognitohazards, for our own protection.

エイヴァはすでにご存知かと思いますが、そうでない方々のために補足させてください。手順10-ケンペレンはCIRCE計画において使用されているプロセスで、fMRIスキャナで監視された複数のDクラス職員に認識災害を見せ、彼らに対する影響を記録するものです。これは、我々と認識災害の間に設けられた緩衝層であり、我々自身を保護するためのものです。

Site-15 has its own 10-Kempelen facility that keeps a rotating population of 50 D-Class at all times. I recommend we verify our FCIs remotely using that resource, instead of having to build our own facility.

サイト-15には独自の10-ケンペレン施設があります。そこでは常に50人のDクラス職員が交代で勤務しています。そのリソースを活用し、我々のFCIの有効性を遠隔で確かめることを提案します。そうすれば、新しく施設を建設する必要はありません。

I respect you, and I respect the work you're doing, I truly do. But this brazen disregard of safety standards -- to word it mildly! -- will only cost us in the long run.

ぼくはあなたと、あなたの研究に敬意を持っています。それは本当です。ですが、控えめに申し上げても、安全基準をこれほど露骨に無視していれば、将来的に大きな代償を払うことになるでしょう。

[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: HYDRA計画の安全手順について**
エイヴァ・ベリーマン [[span class="forum__post-email"]]<@@ava.berryman@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: tomato"]]AB[[/span]]
[[/div]]

[[div class="forum__post-content"]]
This is just going to grind Project HYDRA to a halt.

これはHYDRA計画を停止させる提案にすぎません。

Your concerns are noted, but at this stage of the work, speedy testing and iterative development are more important. O5-8 wants this work done yesterday, after all!

あなたの懸念はわかりました。ですが研究のこの段階においては、迅速な試験と反復的な開発の方が重要です。何と言っても、O5-8は昨日までにこの仕事を終わらせることを望んでおられますから！

[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: HYDRA計画の安全手順について**
サマンサ・ヒュース [[span class="forum__post-email"]]<@@shug3@memetics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: sandybrown"]]SH[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Holy shit. Yes, we need to implement these policies. Thank you, Langford, for bringing this up.

かなりヤバいですね。確かにこのポリシーを適用する必要がありそうです。ラングフォードくん、提案ありがとうございます。

I'll handle O5-8. Everyone needs to stop work //immediately// until we have this rectified.

O5-8は任せてください。ポリシーが改定されるまで、全職員は直ちに作業を中止してください。

Berryman, you and I need to have a word.

ベリーマンくん。あなたとは話し合いをする必要がありそうです。

[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

Under Site Director Hughes' direction, the cognitohazard production process was changed so that personnel were not to view their outputs at all, but instead send them to Site-15 for review.

サイト管理官ヒュースの指導のもと、認識災害生産プロセスは変更された。全職員は、アルゴリズムの出力結果を直接視認することは認められなくなった。これら出力結果はサイト-15へ送信され、レビューを受けることになった。

In the interests of investing in that process' efficiency, O5-8 subsequently ordered the unification of Project CIRCE and several related projects, to consolidate all Foundation research into cognitohazard detection. The resulting project would eventually be named Project MEDUSA, and its goal would be to provide a single source of automated, scalable cognitohazard detection.

研究の効率性を向上させる試みの一環として、O5-8はCIRCE計画と、それに関連する複数のプロジェクトの統合を命じた。結局、認識災害検出に関する財団の研究はすべて統合されることとなった。この統合プロジェクトは、MEDUSA計画と名付けられた。本プロジェクトにおいては、自動化された、かつ拡張可能な認識災害検出の単つソースを提供することが目標とされた。

Additionally, O5-8 ordered Dr. Berryman to experiment with reproducing Procedure 10-Kempelen locally at Site Romero-5, to reduce the project's dependency on Site-15 and on D-Class. Dr. Berryman was loaned several researchers from the main project for this purpose. The duration of this experiment and its outcome, if any, are not on record.

さらに、O5-8はベリーマン博士に対し、10-ケンペレン手順をサイト・ロメロ-5において部分的に再現する実験を行うように命じた。これはMEDUSA計画のサイト-15およびDクラスへの依存度を下げるためのものであった。このため、ベリーマン博士には、MEDUSA計画から数人、研究員が貸し出された。この実験の期間、および結果については、記録が残されていない。

Dr. Langford, who was now perceived as having single-handedly stifled the progress of the project, penned an open letter to all of its personnel.

ラングフォード博士は、プロジェクトの進捗を一手にして妨げた人物と見なされるようになった。彼はサイト・ロメロ-5の全職員に対し、公開書簡を執筆した。

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**サイト・ロメロ-5への公開書簡**
ロバート・ラングフォード [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Hi everyone,

職員の皆様

Over the past few days I've had to put up with more than a few sideways glances here and there. You must all think I'm the new guy who's come here to throw his weight around and disrupt your routine just for the sake of it.

ここ数日、ぼくはあちらこちらから白眼視されているようです。ぼくは新参のくせして権力を振り翳し、ただ皆さんの日常業務を妨害し、そして混乱させていると、皆様はそうお思いのことでしょう。

And, I'll say it plainly, I don't blame you at all. I get it. The Foundation and O5-8 are pushing us to produce as much coghaz as we can. We've got pressure on all sides. If I were in your position, and someone came along and told you how you should be doing your job, I'd be pissed as well.

率直に申し上げます。皆様を責めるつもりはございません。皆様がそうお思いになることも、理解します。財団とO5-8は、ぼくたちにできる限り多くの認識災害を生産するように圧力をかけています。我々はあらゆる方面から圧力をかけられているのです。もしぼくが皆様の立場にあって、誰かが仕事のやり方を指図してきたら、同じように腹を立てるものと思います。

So now I'm going to tell you why I'm right.

ですから、ぼくが正しい理由を説明します。

For those who don't know me, I came here from Project CIRCE. I had a hand in building the very same tools that we're now using for automated coghaz detection. Believe me - that project was //not// plain sailing. We made mistakes, serious ones, that cost lives -- and now you, we, are on the verge of doing the very same.

ご存知ない方のために補足します。ぼくはCIRCE計画から来ました。現在我々が自動認識災害検出に使用している、まさにそのツールの開発に携わりました。そしてCIRCEは、決して順風満帆ではなかったことを、ご理解いただきたいのです。我々は過ちを犯しました。深刻な過ちです。その結果、命が失われたのです。そして今。皆様--　　--私たちは、その二の轍を踏もうとしています。

In 1999, my team received our first instant-kill coghaz, the very first First Order CCI. Its cultural requirements were specific, but our security was lax. Six good researchers lost their lives on the spot. Their potential wasted, completely, instantly. I was very nearly one of them.

1999年に、CIRCE計画において初めての即死認識災害が生まれました。まさに最初の第一級文化的認識災害(Cultural Cognitohazardous Image、以後CCI)です。それが効を発するためには、特定の文化的背景が必要でした。しかし、我々のセキュリティには穴がありました。研究員が六名、即座に命を落としてしまったのです。彼らの可能性は、完全に、そして即座に断たれてしまいました。ぼくも危うく、そのうちの一人になるところでした。

Our old Monte Carlo process was unpredictable, you had zero control over its output, but my new optimization algorithm is like a targeting rangefinder for our fractal cognitohazard generation. That means it's now only a question of //when//, and not //if//, before we create an FCI that does something irreversible -- in fact, it MUST happen for Project HYDRA to succeed. And I know that the vast, vast majority of what we were producing through Monte Carlo were just dead regions, and that's still mostly the case now, and there's a good 95% chance nothing happens when you look - but you roll those dice every single time you do. And, given time, we'll get more efficient, and those odds will only climb -- sharply.

我々がかつて使用していた、古いモンテカルロ法は予測不可能で、その出力をコントロールすることはできません。ですが、ぼくの新しい最適化アルゴリズムは、フラクタル的認識災害画像を生成するための照準測距儀のようなものです。つまり、取り返しのつかないような効果を持つFCIが生成されることは、もはや可能性の話ではなく、いつか必ず起こることなのです。実際、HYDRA計画の成功のためには、そのようなFCIが生成されなければならないのです。モンテカルロ法でで生成されるものの大半が、圧倒的大多数が単なる失活領域でありました。いま生成されるものも、ほとんどそうです。見ても何も起こらない確率が95%であることは承知しています。しかし、皆様はその画像を見るたびにサイコロを振っているのです。そして時間さえあれば、我々はより効率的な手段を見つけ、確率は急激に上昇していくことでしょう。

We //cannot// risk viewing the images we create. Ever. If you value your life, you must never set eyes upon your creations. That is why Procedure 10-Kempelen was established.

生成された画像を視認するようなリスクは冒せません。絶対に。ご自分の命を大事にしたいのであれば、あなたの造った画像を決して見てはならないのです。それが、手順10-ケンペレンが確立された理由です。

The better of you will have looked into 10-Kempelen and will know that it is staffed by D-Class. The best of you will ask, why should they suffer in our stead?

皆様のうち、優秀な方々はすでに10-ケンペレンについてお調べになったことでしょう。そして、それがDクラス職員によって運営されていることを把握なさっているはずです。最も優秀な方の頭の中には、ある問いが浮かんでいることでしょう。なぜ、彼らは私たちの代わりに苦しまねばならないのでしょうか。

They shouldn't. It's not fair. We need to fix that, too.

苦しむべきではないのです。公平ではありません。改善の必要があります。

That is why O5-8 has ordered the Department of Analytics to refine the computerized detection processes. That team is doing exactly what we're doing, just in reverse. They are not our competition -- we are working together. For all of our sakes, we must allow their progress to outpace ours. Yes, I know: the automated detection systems are at best about 30% accurate. That //will// change, given time.

だからこそO5-8は解析部門に対し、コンピュータによる検出プロセスを洗練させることを命じました。あのチームは、我々が今やっていることをちょうど逆回しにしているのです。彼らは競争相手ではなく、協力すべき相手です。我々全員のために、彼らの進捗が我々のそれを上回るようにしなければなりません。自動検出システムの精度はおよそ30%の精度であることは、承知しています。そしてそれは確実に変わっていきます。時間さえ経てば。

Dr. Berryman is working on a solution too, in her own way, with her own handpicked team. I'm not privy to the details, but with their efforts combined, we'll be back to full speed and more before you know it.

ベリーマン博士も彼女なりのやり方と、彼女自ら選んだチームでもってこの問題に取り組んでいます。ぼくはその詳細を知りませんが、彼らの努力も組み合わさってしまえば、気づいた時には元以上の速度で研究が進んでいることでしょう。

And I'm hard at work as well, when I'm not busy trying to get everyone to down tools! If I can derive the underlying formulas that define the cognitohazardous fractal space, we'll be able to traverse it directly, and the current algorithm can go fuck itself. We'll be vastly more efficient and we'll have so much more control.

そして、ぼくも懸命に取り組んでいます。皆の作業を中断させるために忙しくしている時以外はね！　認識災害的なフラクタル空間を定義する基礎方程式さえ導出できれば、我々はその中を縦横に走ることができるようになります。つまり今使っているアルゴリズムなど、鼻クソ以下のものになってしまうのです。我々は遥かに効率的に、そして遥かに多くの制御が可能になることでしょう。

It will get better. I promise. The odds of losing are small, but we're not safe until they're zero, and the stakes are so very high.

状況は好転します。約束します。何かを失う可能性は小さいですが、それがゼロになるまでは決して油断できません。我々の身上に賭されているものは、あまりにも大きいのです。

ロバート・ラングフォード
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

As Dr. Langford's policies had the support of Site Director Hughes, cognitohazard production remained subject to these constraints. In the meantime, efforts were redirected to the study of the production of inoculant images.

ラングフォード博士の方針がサイト管理官ヒュースの支持を得たため、認識災害の生産プロセスは、この制限の下で実施されることとなった。また、免疫画像を生成するための研究が、再度活発に行われるようになった。

[[div class="blockquote"]]
**Excerpt from //On the Generation of Cognitohazard Inoculants// by Dr. Ava Berryman, 2006**

**2006年、エイヴァ・ベリーマン博士による『認識災害に対する免疫の生成について』より抜粋**

The production of inoculant imagery is intended to confer immunity to one specific cognitohazard through its pairing with a second controlled cognitohazardous stimulus with an effect tailored specifically to render the viewer immune to the aforementioned. The mechanism is poorly-understood; our proposed theory posits that each inoculant permanently disrupts a distinct set of cerebral nodes required for the activation of its corresponding cognitohazard. Historically, identifying a suitable inoculant for a given cognitohazard has proven more laborious than the initial discovery of the hazard itself, due to limitations in methodology and the complexity of neural interactions [...]


免疫画像の生成は、特定の認識災害に対する免疫を付与することを目的としており、それは第二の制御された認識災害性刺激との対提示によって達成される。この第二の刺激は、閲覧者を前述の認識災害に対して免疫化するよう特別に調整された効果を持つ。そのメカニズムは十分に理解されていない。我々の提唱する理論では、各免疫画像は、対応する認識災害の発動に必要な特定の脳内ノード群を永続的に破壊するものと仮定している。歴史的に見て、与えられた認識災害に対する適切な免疫画像の特定は、方法論の限界と神経相互作用の複雑性により、当該災害の最初の発見よりも困難であることが証明されてきた[...]

[[/div]]

Although Dr. Langford had not yet derived the underlying equations, improving computational technologies were beginning to accelerate the pace of development. At this time, Site Romero-5 was producing up to 4 FCIs per week, though after curation, only an average of 2 per month were considered potentially useful to the Foundation.

この時点において、ラングフォード博士はFCIを生成するための方程式を導出していない。他方で、計算機技術の進歩により、開発の速度が加速しつつあった。当時、サイト・ロメロ-5は一週間あたりに4つのFCIを生成していたものの、選別のすえに財団にとって有用とみなされたものは、平均して2つほどであった。
 _

[[div class="samples"]]
[[div class="samples__header"]]
= Sample FCI output generated during this era. Cognitohazardous effects, if any, have been evaluated and interpreted by Waldor.aic.

= この時期に生成されたFCIの例。認識災害的効果は、Waldor.aicによって評価され、記述されている。
[[/div]]

[[div class="samples__image-heading"]]
= **FCI**
[[/div]]
[[div class="samples__desc-heading"]]
= **記述**
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logbox3.webp]]
[[/div]]
[[div class="samples__desc"]]
Thin filament structured in Lichtenberg pattern. Viewer becomes acutely aware of their breathing patterns for a short period.

リヒテンベルグ図形を形作る細糸。視認した者は、自身の呼吸パターンを短時間にわたり強く意識するようになる。

[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logbox1.webp]]
[[/div]]
[[div class="samples__desc"]]
Branching fractal in greyscale with seven arms. Dead region.[[footnote]]**{{DATA LOST}}**[[/footnote]] No effects noted within the image.

白黒で、7本の腕を持つ、枝分かれしたフラクタル図形。不活領域。[[footnote]]{データ喪失}[[/footnote]]この画像に特筆すべき効果はない。

[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logboxblue1.webp]]
[[/div]]
[[div class="samples__desc"]]
Serpentine swirl in blue tones and receding into two separate points. Induces mild sense of anxiety regarding an upcoming personal event or task that the viewer has neglected.

This unit posits this may be useful for internal use in increasing productivity.

青色の、蛇のような渦巻きが、二つの点へ収束している。視認した者に対し、その者が意図的に無視するようにしていた、直近の予定やタスクについて、軽い不安感を抱かせる。

本ユニットは、生産性を向上させるために、この画像を財団内部で利用することが有効であると推定する。

[[/div]]

[[/div]] [!-- .samples --]

 _

+++ 2008年7月

On 2008-07-05, the 10-Kempelen facility at Site-15 reported that Site Romero-5 had produced a lethal First Order FCI with ID number FCI-284/1.

2008年7月5日、サイト-15の10-ケンペレン施設は、サイト・ロメロ-5において、最初の第一級FCIが生成されたと報告した。そのFCIには、FCI-284/1というIDが割り振られた。

Procedure 10-Kempelen attempts to assess the efficacy of the cognitohazard through exposure to multiple test subjects. 15 D-Class personnel were made to observe the FCI, all of whom were found to be susceptible before Site-15 staff terminated the test prematurely. For reference, the efficacy of the average CCI is 45% and of the at-the-time most effective CCI was 71%. The researcher responsible for the production of the FCI chose to remain anonymous.

手順10-ケンペレンは、複数の被験者への曝露を通じて、認識災害の有効性を評価する者である。15名のDクラス職員がFCIを視認し、全員が影響を受けたことが確認された。なお、本試験はサイト-15のスタッフにより中断された。なお、平均的な文化的認識災害の有効性は45%であり、当時最も効果的なものでも71%であった。このFCIの生成を担当した研究者は、匿名を希望した。

The First Order FCI and its inoculants were submitted to Site-19, and on 2008-07-26, Lieutenant Masipag actioned the first-ever deployment of a universally-cognitohazardous kill agent to secure the SCP-001 file.

この第一級FCIとその免疫画像はサイト-19へ提出され、マシパグ中尉によって、SCP-001ファイルを保護するための普遍的認識災害性ミーム殺害エージェントとして、初めて配備された。

Dr. Berryman issued a statement to the Project HYDRA staff in response.

これを受けて、ベリーマン博士はHYDRA計画のスタッフに向けて声明を発表した。

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**We've bloody done it**
Ava Berryman [[span class="forum__post-email"]]<@@ava.berryman@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: tomato"]]AB[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Colleagues,

This month, we have taken our largest step yet towards proving the legitimacy of our endeavor, and have finally made a truly significant contribution to the security of the Foundation. Our work has finally borne fruit. I am so very proud of all of you.

For many of you, this is your first Project of this scale. Hold onto this feeling -- do not let your pride fade. An accolade of this esteem can catapult your career, if you play it right.

Tonight we're going to have a get-together in the Site cafeteria. Food and drink will be provided, and I expect you to not only leave your work at the door but to forget about it for as long as you need to in the morning as well, if you catch my drift.

I'd really, really like to see everyone come to this celebration, no matter whether you're working in Generation or if you're on the Berry team. Let's come together as a Site and give each other the break we deserve!
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: We've bloody done it**
Robert Langford [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
I'm grateful that our first lethal cognitohazard has found a role in the protection of our most important assets. It would have been a shame for that prestige to have been given to a more aggressive function.

Each day this month, I've thought of the fifteen personnel who gave their lives for the sake of this picture, and what they would think if they saw us now. We have much to thank them for. Please afford them a moment's thought yourself, even though you have never met, and are so many layers removed from them.

We are on a precipice, certainly. It is my deepest hope that it will be of something great, and that collectively we can be proud of the decisions we will have made along the way.

I'll make sure to swing by the celebrations briefly, but the stresses of the project have been getting to me, so I won't be staying long. It'll be nice to see everyone in a more relaxed capacity for once!
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

Despite the success, Project HYDRA was not yet complete, as Site Romero-5 could not yet continuously or reliably produce any kind of FCI, let alone First Order FCI specifically. All FCIs produced thus far had been the result of a mix of the Langford algorithm and guesswork.

-----

+++ 2010, March

In March 2010, after just over two years of effort, Dr. Langford successfully derived the underlying formulas. The result of his research, a single equation that definitionally mapped out the entirety of the cognitohazardous fractal space, would become known as the Berryman-Langford set.

The definition of the Berryman-Langford set, after its correctness was proven, was immediately locked in an ultra-secure enclave within the Site Romero-5 data store, with access only provided to Site Director Hughes, Dr. Berryman, and Dr. Langford. Other members of the research team were not permitted to view the equations or even know its parameter count, as any leak to hostile Groups of Interest would represent a colossal security breach.

The Berryman-Langford set could be trivially solved computationally to pick valid seed values; the fractal space could now be traversed directly, intentionally picking regions to explore, instead of needing to randomly chance upon starting values that happened to intersect with the fractal space through sheer luck.

Through the Berryman-Langford set, the rate of generated output having cognitohazardous properties increased by orders of magnitude, from 0.004% to over 80%. Dr. Berryman suspected that the rate was actually closer to 100%, with the discrepancy caused by cognitohazardous effects that the detection methods at the 10-Kempelen facility were unable to classify, e.g. immeasurably minuscule effects, or effects targeting non-quantifiable parts of the mind.

However, Site-15 would not address Dr. Berryman's requests for improvement. Within a month, an official complaint was issued to Site Romero-5.

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**Please slow down**
ヴラジミール・ヴコヴィッチ [[span class="forum__post-email"]](MEDUSA計画理事) <@@vvuk@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: paleturquoise"]]VV[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Samantha,

Your team has flooded us with cognitohazard classification requests. Our testing facility is overwhelmed. Both our organic and computational resources are being consumed mostly by you.

You are not the only Site that relies on us. Nearly all cognitohazard classification goes through Site-15. Our backlog is becoming unmanageable. We are hugely investing in our computational detection processes through Project MEDUSA but I do not have the resources I need to scale up our Procedure 10-Kempelen operations to the levels that you are asking for. There are not enough D-Class.

I have enough issues to deal with as it is. The Site Director has authorized me to block all classification requests from your team if I need to. I understand the importance of your work and I have no desire to do that.

But, please, slow down.
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

Site Director Hughes elected to sustain the request from Site-15. After negotiating with Director Vuković, she placed a limit on the number of potential FCIs that could be submitted to Site-15 per day.

With Project HYDRA's progress now externally bottlenecked, the headcount at Site Romero-5 was reduced from 55 to 19. Many of the displaced staff transferred to Site-15 to assist efforts to expand detection capacity at Project MEDUSA. Permission was granted to Dr. Berryman for access to any Foundation resource as required to complete her research project.

-----

+++ 2011, June

In June 2011, the Department of Analytics released Project MEDUSA for general access to the rest of the Foundation.

Automated detection of cognitohazards via the MEDUSA service breathed new life into Project HYDRA. The MEDUSA service was capable of taking over all rote cognitohazard detection and classification work, and outclassed the previously-available cognitohazard detection methods in practically every metric. For cognitohazards with known effects, the cognitohazard backlog was emptied within a matter of weeks, and production quickly resumed at full pace.

As the MEDUSA service was a machine-learning based system, constant exposure to new fractal cognitohazards created a positive feedback loop, making it more and more capable over time. However, for the same reason, it was unable to classify cognitohazards with as-yet-unseen effects. Around one third of FCI production fell into this category. The only way to assess such a cognitohazard with sufficient medical rigor was, and is, to measure its effects on a living person. The 10-Kempelen facility at Site-15 remained the bottleneck.

-----

+++ 2012, January

In January 2012, Dr. Berryman's research project was complete and her team merged back into the main team. Cognitohazard generation stopped while the results of the experiment were integrated into the existing FCI creation process.

Three days later, production resumed along with verification requests via the MEDUSA service, albeit now with zero demand on the 10-Kempelen facility.

In March, Project MEDUSA Director Vuković sent a message to Site Director Hughes.

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**10-Kempelen query**
Vladimir Vuković [[span class="forum__post-email"]]<@@vvuk@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: paleturquoise"]]VV[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Samantha,

How has your team managed to not only reduce its reliance on our 10-Kempelen operation, but eliminate it entirely?

I've seen some of the cognitohazards your team is producing since that change (not the imagery itself, of course), and the attached data is just as medically conclusive as ours. Yet your site is not requisitioning any D-Class. If others could reproduce your results, our load could be lessened even further, or perhaps we could use them ourselves.

Please interpret my asking as nothing more than grateful curiosity. The resources that can now be diverted from the operation will have cumulative benefits everywhere. The Department of Analytics director has advised me not to be questioning a good thing in the first place.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: 10-Kempelen query**
Samantha Hughes [[span class="forum__post-email"]]<@@shug3@memetics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: sandybrown"]]SH[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Vladimir,

Thank you for your grateful curiosity. In the pursuit of efficiency, we're very happy to have been able to reduce our impact on your personnel.

I am not at liberty to say more.
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

Dr. Langford did not comment on the process improvements initially, but a week later, he announced his full support.

----

With the MEDUSA service being able to validate any amount of cognitohazards as needed, Site Romero-5 being able to classify all FCIs itself to a satisfactory level, and the solved Berryman-Langford set allowing for unabated FCI generation, Project HYDRA was officially complete. O5-8 briefly visited to congratulate the team.

Most Site Romero-5 staff, including Director Hughes, Dr. Berryman, and Dr. Langford, remained on-site to oversee continued cognitohazard production.

As of the end of 2012, after curation, Site Romero-5 was submitting an average of 60 useful FCIs per week, up to 10 of which were First Order.

 _
[[div class="samples"]]
[[div class="samples__header"]]
= Sample FCI output generated during this era. Cognitohazardous effects, if any, have been evaluated and interpreted by Waldor.aic.
[[/div]]

[[div class="samples__image-heading"]]
= **FCI**
[[/div]]
[[div class="samples__desc-heading"]]
= **Interpretation**
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logbox2.webp]]
[[/div]]
[[div class="samples__desc"]]
Innumerable wisps of pale orange strands which converge into a complex, many-pointed star. Viewer may experience quickened heart rate for a brief duration, coupled with an implaceable feeling of growing dread.
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logbox5.webp]]
[[/div]]
[[div class="samples__desc"]]
Greyscale snailshell spiral receding into a single point in the center-left. Minute effect on spatial reasoning: sets of right angles enclosed within a space composed of right angles (e.g. a closed caption bar displayed on a television) appear skewed.
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logboxblue2.webp]]
[[/div]]
[[div class="samples__desc"]]
Many colorful whorls bordering the edge of a dark region, from which emerges many strands of Lichtenberg filament. Viewer becomes skeptical of recently-learned information.

This unit has pored over accompanying research data and has come to the conclusion that the effect is too minute to be effective in the field.
[[/div]]

[[/div]] [!-- .samples --]

 _

[[div class="classified-banner rotate"]]
[[div class="classified-banner__dept"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/analytics_dept_duo_animated.svg]]
[[/div]]

[[div class="classified-banner__text"]]
SCP-9001

The following series of files relates to the
[[size 133%]]Department of Analytics **Project NIETZSCHE**[[/size]]
and is level **4/NIETZSCHE** classified.

Unauthorized access is strictly forbidden.
[[/div]]
[[/div]] [!-- .classified-banner --]

In November 2014, O5-8 visited Site Romero-5.

[[div class="blockquote rotate"]]
**Project NIETZSCHE briefing**
In attendance: Site Director Samantha Hughes, Dr. Ava Berryman, Dr. Robert Langford, and O5-8 as Project NIETZSCHE director.

Meeting was conducted in the secure data vault below Site Romero-5.

-----

**O5-8:** This room is private, yes?

**Dir. Hughes:** Private enough. There aren't any recording devices. Technically the room could be sealed off, but we'd only have half an hour of air, so I'm not going to do that.

**O5-8:** [[span class="o5-8"]]Seal the room.[[/span]]

//Loud metallic noises and a rush of air as Director Hughes seals the security door closed.//

**Dir. Hughes:** Oh, wonderful. You realize that can only be opened from outside?

**O5-8:** Your staff will have been notified already. Our conversation will not leave this room. Understood?

**Dir. Hughes:** Understood. Eight, what could possibly need to be this secret?

**O5-8:** You are aware that the cognitohazards you have been producing are primarily in use to secure critical Foundation assets.

**Dir. Hughes:** Yes.

**O5-8:** There is a flaw in that security. The cognitohazards do not affect one demographic.

**Dir. Hughes:** I thought the whole point was that they work on everyone.

**Dr. Berryman:** They do. Therein lies the beauty of the fractal. Its purity touches all.

**O5-8:** No. They do not work on reality benders.

**Dr. Berryman:** Which ones?

**O5-8:** All.

**Dr. Berryman:** You may have misunderstood. What kinds of reality benders, specifically, are unaffected?

**O5-8:** All.

**Dr. Berryman:** I... hm. I see.

**Dr. Langford:** That's not possible.

**Dir. Hughes:** Robert, you tested on reality benders, right?

**Dr. Langford:** Well, not specifically, but there would have been some in the 10-Kempelen--

**Dr. Berryman:** To be quite honest, I've been expecting something like this. I believe we would have heard about some high-profile reality bender death by now.

**Dr. Langford:** There's no way you could have been expecting //anything// like this. We have no reason to suspect someone would be immune just because they're a reality bender.

**Dr. Berryman:** Perhaps, perhaps not. The fractal is more real than reality, remember? Does it not fit that a reality bender would be subject to different rules?

**Dr. Langford:** By virtue of what? You //are// the biologist, aren't you? What biological difference is there between someone who's a reality bender and--

**O5-8:** [[span class="o5-8"]]Stop.[[/span]] Berryman, what is your theory?

**Dr. Berryman:** If it is only reality benders who are not affected, as you say, and it is //all// reality benders who are not affected, as you imply, then it follows that reality benders are simply fundamentally different to everyone else.

**Dr. Langford:** That can't be true! Some of the D-Class in 10-Kempelen //must// have been reality benders, statistically-speaking! I've reviewed all the data and not once has any FCI come back as anything other than 100% effective.

**Dr. Berryman:** Evidently not, elsewise we'd not be having this conversation, would we?

**O5-8:** Dr. Langford is correct. Latent reality benders in the D-Class population of Site-15 were exposed to your cognitohazards on numerous occasions. They were unaffected. We have gone to great lengths to hide those results.

**Dr. Langford:** Wh... what? Why?

**O5-8:** Utilization of the imperfect is more efficient than awaiting perfection.

**Dir. Hughes:** You've known about this for two years, at least, then? How has this not been a problem until now?

**O5-8:** Yours is not the only security method under our employ. Should a reality bender happen to access a protected document, conventional trackers have proven sufficient for locating and acquiring them. It does not happen often. Most who view a cognitohazard are inoculated against it.

**Dir. Hughes:** I thought we were making actual contributions to Foundation security, not slapdash patches to a sloppy approximation--

**O5-8:** [[span class="o5-8"]]Silence.[[/span]] We are now using your cognitohazards to secure elements for which fallback methods may not be sufficient. This is not yet a matter of urgency. What do you need?

**Dr. Langford:** To produce a cognitohazard that can affect reality benders? Well, there must be a biological reason for the discrepancy, and not something that's ever been noted before, in any study, ever, otherwise we'd already know about it. It must be something that's specific to fractal coghaz. So, we need data, lots of data, and we need to get it by exposing fractal coghaz to as many reality benders as we can.

**Dr. Berryman:** We don't need anything of the sort. It's simple: the reality bender enforces her own perception of reality. Of course this would render her immune to the greater reality of the fractal.

**Dr. Langford:** That's just a hypothesis and it doesn't even make sense. We need evidence.

**O5-8:** Yes. We are not interested in speculation. [[span class="o5-8"]]Prove or disprove.[[/span]]

**Dr. Berryman:** Very well.

**Dr. Langford:** We're going to need that data.

**O5-8:** We will give you access to the reality bender data from the Site-15 tests.

**Dr. Langford:** It won't be enough. We'll need more, much more.

**Dr. Berryman:** I believe I have just the vaguest notions of an idea as to how we might gather that data from the reality benders already employed at the Foundation.

**O5-8:** Good, Dr. Berryman. We look forward to hearing your idea.
[[/div]]

Upon returning to Site-01, O5-8 initiated Project NIETZSCHE, enrolling Dr. Berryman, Dr. Langford, and the rest of the remaining Site Romero-5 staff. O5-8 would direct the project, with Dr. Berryman reporting directly, and Dr. Langford reporting to Dr. Berryman.

Project NIETZSCHE was presented to the Foundation as simply the continued effort to improve the cognitohazard production process, with knowledge of its true purpose -- to discover a means to use fractal cognitohazards on reality benders -- kept secret, on account of the security implications. To that effect, Site Director Hughes would remain chiefly concerned with the day-to-day operations of Site Romero-5.

+++ 2014, December

[[div class="project-proposal blockquote"]]

||||~ Proposal NIETZSCHE-01 ||
||~ Date || 2014-12-11 ||
||~ Proposed by || Dr. Ava Berryman ||

||~ PROBLEM ||
|| Project NIETZSCHE requires a continuous source of data regarding the responses of reality benders to fractal cognitohazards, recorded to a level of medical rigor. ||

||~ RECOMMENDED APPROACH ||
|| The Foundation has access to a large number of reality benders within its body of staff. We must convince or coerce them to voluntarily record cognitohazard response data. This will be far simpler than attempting to acquire reality benders from outside the Foundation or through attempting to use data collected from humanoid reality-bending SCPs, as reality benders on the Foundation payroll are already under our control. ||

||~ PROPOSED STRATEGY ||
|| The Foundation currently lacks a comprehensive method of objectively testing a reality bender's potential, and there is great demand for an assessment to fill this void. I will create such an assessment, which will be presented as a means for Site leadership to examine a reality bender's abilities in terms of veracity and usefulness. _
 _
The assessment will actually exclusively contain FCIs that we intend to test on reality benders. The assessment will guide an interviewer and a participant through discussion of the cognitohazardous effects under fMRI measurement. We will use the data to inform future editions of the assessment, and in so doing we will create a feedback loop that continuously empowers our development process. _
 _
I do not have the means to legitimately create a functional reality bending test, but any errors in its results can be attributed to its being merely an early prototype. We may be able to leverage this by encouraging Site leadership to get in on the testing procedure early and be ahead of the curve. _
 _
The assessment will be offered to various Sites with high numbers of reality benders on their staff. I will imply that participation in the assessement is, or will be, mandatory. ||

||~ PROPOSAL STATUS || **##limegreen|APPROVED##** ||

||~ AMENDMENTS || **O5-8:** It will reflect poorly on us should the truth come out that the assessment is ineffective. Site leadership must be informed of its true purpose. They will understand the importance. They will respect the secrecy. ||

**Update: 2015-01-06**

I have compiled a set of 38 cognitohazards into a publication, the Reality Bending Aptitude Assessment (RBAA), and it is currently in print at the Foundation Press.

[[include :scp-wiki:component:image-block
| name=https://scp-wiki.wikidot.com/local--files/scp-9001/berrymans-tests-for-reality-bending-aptitude-2019-hardcover.webp
| caption=Cover of 'Reality Bending Aptitude Assessment', hardback, Dr. Berryman.
]]

**Update: 2015-01-17**

Copies of the RBAA have been distributed to several Foundation sites: Site-87, Site-91, Site-118, Site-400. Each one of those Sites has responded similarly: they thanked me for taking an interest, said they would review, and promised to get back to me. As of yet, none of them have.

**Update, 2015-02-11**

My initial batch of requests remains unanswered. I have decided to reach out to [[span class="hoverlink"]][[[secure-facility-dossier-site-120|Site-120]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Site-120[[/span]][[span class="hoverlink-text"]]Foundation headquarters in Poland. Containment and research facility that embraces usage of thaumaturgy and the anomalous, including within its staff.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/secure-facility-dossier-site-120/medium.jpg/small.jpg)"]]-[[/span]][[/span]][[/span]] earlier than planned. Site-120 is home to the Department of Ontokinetics and the single largest employer of reality benders in the Foundation. If they agree to my request, I believe it would be sufficient to start a snowball for the RBAA to get a foothold and spread across the Foundation.

**Update, 2015-02-14**

Site-120 has replied:

[[div class="blockquote"]]
Dr. Berryman,

I appreciate you making this generous offer to Site-120, but more than that, I appreciate you revealing the truth of what this offer actually entails. Naturally, I will keep your secret. In fact, as far as Site-120 is concerned, your secret ends with me. I will not participate.

Dr. Berryman, the Reality Bending Aptitude Assessment is transparently bullshit. There is no use pretending. There is no one who does not see through it -- Site Director, interviewer, participant. If you had reached out initially and asked for a means of data collection, you would very likely have received a more positive response. Instead, you have hidden your intent under layers of subterfuge.

However, even if I were willing to overlook that, this assessment is still not something I would be interested in my staff partaking in. You have gone to great lengths to conceal the nature of Project NIETZSCHE, and no doubt any information most personnel would be able to find would be carefully-constructed fabrications, but you have already revealed your hand to me. Your assessment may well be perfectly safe now, but your cognitohazards will develop, and eventually the assessment will not be safe at all. Eventually you will need to test a kill agent in the field. This is always the end goal of these kinds of projects, whether you choose to acknowledge it or not.

My staff are extraordinarily valuable to me, to Site-120, and to the Foundation as a whole. Why, then, should I agree to allow my staff to be guinea pigs for your experiments? Why should I trust you and your assessment, and grow complacent myself? Do you expect me to look the other way when you inevitably use a future edition of the assessment to turn on me and my staff simply because I once stepped aside for you?

You are unlikely to make any progress if you continue using these methods.

**Dr. Jessie Rivera**
Human Resources and Personnel Satisfaction Lead
Site-120
[[/div]]

Evidence would suggest that attempting to convince further Sites to integrate the RBAA into their methodology would be an imprudent use of my time. We should still use the RBAA to assess reality benders as they appear in the D-Class population, should the opportunity present itself.

[[div class="overwatch-order"]]
[[div_ class="overwatch-order__logo"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/overwatch-command-logo-1.webp alt=""]]
[[/div]]

[[div class="overwatch-order__content"]]
[[span class="overwatch-order__title"]]BY ORDER OF OVERWATCH COMMAND[[/span]]

Proposal NIETZSCHE-01 is hereby decommissioned.
[[/div]]
[[/div]] [!-- .overwatch-order --]

[[/div]]

Site Romero-5 continued to request reality benders for cognitohazard testing, but with the paranoia of the RBAA fresh in the minds of Foundation leadership, little attention was paid. Dr. Berryman and Dr. Langford would continue trying to find solutions using the small amount of data they already had, and production of regular FCIs continued.

-----

+++ 2016, November

O5-8 visited Site Romero-5 and ordered Dr. Langford to provide an update on Project NIETZSCHE progress.

In the resulting schedule alignment meeting, Dr. Langford reported substantial delays and difficulties, principally that the team still did not have nearly enough data on reality benders to begin drawing any kinds of conclusions at all, and were still just as in the dark as when the project began.

O5-8 was satisfied by this answer, but not sated, and ordered Dr. Langford to repeat this presentation on an annual basis, each November, to keep interested parties up to date. The meeting would yet recur twice more.

-----

+++ 2017, February

Following a period of several months with no updates from the Site Romero-5 team, without warning, Dr. Langford issued the following memorandum.

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**On the right path**
Robert Langford [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Hi all,

I've made a breakthrough regarding the reality bender's resistance to fractal cognitohazards.

We knew from the go (well, we'd speculated) that, as this problem is not only unsolved but apparently nonexistent outside of this narrow scope, the issue must pertain to fractal cognitohazards specifically and exclusively.

My research into reality bender neuroanatomy is beginning to indicate that this is indeed the case! I have proven that reality benders' immunity to FCIs is a direct result of their brain structure having some difference to baseline humans.

However, we don't yet have enough data about reality benders' brain structures to construct a pattern definitively. We need //much// more data than we have.

My suggestion would be to have all reality benders across the Foundation undergo CT scans and have the resulting data models transferred to our data store so that we can analyze and compare. Of course, this is quite invasive, and I don't have anything close to the authority to request it.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: On the right path**
O5-8 [[span class="forum__post-email"]]<@@8@o5.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: black; color: white"]]8[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Excellent news. This is consistent with what you have been saying since Project NIETZSCHE was incepted. It is promising that your instinct has proven accurate.

Do what you must to acquire the data you need. You may cite our authority as necessary.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: On the right path**
Ava Berryman [[span class="forum__post-email"]]<@@ava.berryman@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: tomato"]]AB[[/span]]
[[/div]]

[[div class="forum__post-content"]]
I wish you had consulted me before making this announcement. There is no method by which a reality bender can be identified by brain structure alone, this is known. The problem is more fundamental. The conclusion you've drawn makes little sense from a biological standpoint, and the weeks you've spent trying to convince me of 'scientific rigour' have apparently been lost to you as you've not included a single citation or scrap of medical evidence.

This isn't like you, Dr. Langford. But your childish insistence on communicating to me via open letters very much is.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: On the right path**
O5-8 [[span class="forum__post-email"]]<@@8@o5.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: black; color: white"]]8[[/span]]
[[/div]]

[[div class="forum__post-content"]]
We have placed full confidence in Dr. Langford. We advise you to do the same.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: On the right path**
Robert Langford [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Ava, please accept my apologies. I keep getting wrapped up in the work and get ahead of myself in the excitement. Really, I am sorry.
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

In the months that followed, Site Romero-5 would issue O5-backed orders to other Sites, requesting computer tomography scans of their on-staff reality benders.

-----

+++ 2017, November

Dr. Langford travelled to Site-15 and presented the second annual Project NIETZSCHE Schedule Alignment Meeting, with O5-8, Site Director Hughes, Project MEDUSA Director Vuković and several others in attendance. This time, at O5-8's request, the presentation was broadcast live across the Foundation, and 45 viewers tuned in remotely.

Dr. Langford again reported substantial delays and difficulties to the project, and the principle issue remained that there was not enough data to provably determine any conclusions. Dr. Langford was keen to highlight the extent of the proof that would be required: one objective of the project was to produce a fractal cognitohazard capable of terminating any reality bender, but to prove this would mean proving beyond reasonable doubt that no reality bender cannot be terminated via the same method. This would mean the deaths of multiple reality benders, or accurate simulation, and Dr. Langford expressed that the data available was not nearly sufficient for that.

O5-8 noted surprise that this was still an issue, but pledged that Site Romero-5 would eventually get the amount of data it needed.

----

+++ 2018, July

While attending a conference at Site-19, Dr. Berryman addressed Dr. Langford in a message on the Site Romero-5 internal communications network.

[[div class="forum"]]

[[div class="forum__post forum__post--op"]]
[[div_ class="forum__post-header"]]
**Idea regarding Project NIETZSCHE**
Ava Berryman [[span class="forum__post-email"]]<@@ava.berryman@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: tomato"]]AB[[/span]]
[[/div]]

[[div class="forum__post-content"]]
Robert, I've just seen a presentation by Dr. Clef regarding reality benders and it gave me an idea. Have we tried simply going deeper into a candidate modification to the Berryman-Langford set and accessing more deeply-buried regions? I'm wondering if the answer is as simple as overwhelming the reality bender's mind with the much more complex fractal context. I think this wouldn't be too much of a deviation from our existing work to completely invalidate the studies we've done so far.
[[/div]]
[[/div]] [!-- .forum-post --]

[[div class="forum__post forum__post--reply"]]
[[div_ class="forum__post-header"]]
**Re: Idea regarding Project NIETZSCHE**
Robert Langford [[span class="forum__post-email"]]<@@robert.langford@analytics.scp@@>[[/span]]
[[span class="forum__post-pfp" style="--bg: khaki"]]RL[[/span]]
[[/div]]

[[div class="forum__post-content"]]
What an interesting idea. I'll try it immediately.
[[/div]]
[[/div]] [!-- .forum-post --]

[[/div]] [!-- .forum --]

Before Dr. Berryman's return, Dr. Langford ran several experiments using the suggested method and produced a set of prospective FCIs. They were proven to be effective on baseline humans immediately, and Dr. Langford requested Site-15 to notify him when a reality bender entered its 10-Kempelen population.

It would be several weeks before that was the case, and upon receipt of the message from Site-15, Dr. Langford submitted the new FCIs for testing. Of the full set, one single FCI proved to be effective on the reality bender.

Dr. Langford notified Project NIETZSCHE leadership of his success and continued developing the new method, though he stressed that despite the success, provability was still the most important problem to solve, and therefore the need for reality bender biological data was still relevant.

It is worth noting that while Dr. Clef was present at the Site-19 conference and did lead a seminar on reality benders, Dr. Berryman did not attend it.

-----

+++ 2018, August

The Ethics Committee received an anonymous whistleblower report regarding Site Romero-5 and immediately investigated.

[[div class="ethics"]]
[[div_ class="ethics__header"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/ethics-committee-logo.webp alt="" style="filter: invert(1); max-width: 10rem; max-height: 10rem; aspect-ratio: 1;"]]
**ETHICS COMMITTEE MEMORANDUM**
[[/div]]

[[div class="ethics__content"]]

+++ **Investigation Summary** [[span style="color: grey; font-size: 80%;"]]| August 12th, 2018[[/span]]

An anonymous whistleblower report has accused Site Romero-5 leadership of the following issues:

# Unethical restriction for staff to remain on-site.
# Unethical usage of anomalous compulsion effects to influence and control on-site staff.
# Unethical use of human materials for testing purposes.

The Ethics Committee takes such allegations seriously.

Investigation was conducted by EC Investigator Amber H. Goldstein. On 2018-08-21, Investigator Goldstein travelled to Site Romero-5 to interview its staff.

Goldstein was able to interview most staff members one-on-one. The following statements from relevant parties are attached.

[[div class="blockquote"]]
**Witness Statement:** Head Researcher Ava Berryman

Obviously, elephant in the room: [REDACTED]

The other ones just aren't true. I was at the Site-19 conference just earlier this month, and the kind of compulsion you're speaking of -- well, there's no one stationed here who can do that, and the-- precisely, they're locked down, the staff can't even access them. Only myself and Dr. Langford. Yes, of course, and he has my deepest sympathy.
[[/div]]

[[div class="blockquote"]]
**Witness Statement:** Researcher Derrick Coleman

We've never been barred from leaving. I don't think? We get our annual leave, same as everyone else. I mean, we don't get to go home every night, but that's standard operating procedure for classified projects. And the compulsion thing is patently false -- the only source of compulsion here is the Third Order cognitohazards, but we're not allowed to look at them, there are even system locks that stop us if we try. No, I've not tried myself, of course not. And then there's [REDACTED] is valid, I suppose, but it's better than the alternative.
[[/div]]

[[div class="blockquote"]]
**Witness Statement:** Site Director Samantha Hughes

I've been Site Director for twelve years and I've never seen anything happen here that would warrant EC intervention. You can ask any of my staff. Oh, you did? Then you'll know for sure.

I have the utmost respect for the whistleblowing process, but I will admit I would love to know who started this. I don't suppose-- no? I can't fault you for that.
[[/div]]

Investigator Goldstein asked to interview Dr. Robert Langford but was informed that he had been hospitalized with an illness of a personal nature, the details of which are not relevant to this report.

+++ Investigation results

Investigator Goldstein recommended the Ethics Committee take no action.

[[div class="blockquote"]]
**Closing Statement:** Investigator Amber H. Goldstein

Site Romero-5 is operating nominally. There are some complaints amongst the staff, but nothing that wouldn't be expected in any other Site. The Site appears understaffed given its size, which could give rise to issues, but I'm told that the workload in general is fine, and besides, the complaints are so specific that they're unlikely to be related.

Regarding issue 1, I found no evidence of any member of staff being unduly restricted to the Site.

Regarding issue 2, I found no evidence of any usage of anomalous compulsion effects, including those that might be expected from accidental application of the cognitohazards that are made here, which does not seem to occur.

Regarding issue 3, [REDACTED]

Overall, most of the whistleblower's complaints are invalid and of those that aren't, there is a very good reason for it. Berryman has been around for decades, she knows what she's talking about, and everything she said checks out.

No immediate intervention is required. I will discuss with the Site Director regarding what should have happened initially, and it will be addressed in due time.
[[/div]]

Case number HX-68396 is closed.

[[div class="overwatch-order"]]
[[div_ class="overwatch-order__logo"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/overwatch-command-logo-1.webp alt=""]]
[[/div]]

[[div class="overwatch-order__content"]]
[[span class="overwatch-order__title"]]BY ORDER OF OVERWATCH COMMAND[[/span]]

In the interests of Foundation security, parts of this report have been redacted.
[[/div]]
[[/div]] [!-- .overwatch-order --]

[[/div]]
[[/div]] [!-- .ethics --]

Following the investigation, in gratitude for their cooperation, Site Director Hughes granted all staff three weeks' immediate leave. She and Dr. Berryman remained on-site to discuss the investigator's recommendation.

Shortly thereafter, Dr. Langford, who was not on-site during the investigation, returned and resumed work.

-----

+++ 2018, November: Incident 9001-1

In November 2018, Dr. Langford travelled to Site-15 and presented the third annual Project NIETZSCHE Schedule Alignment Meeting.

[[div class="blockquote"]]
The following footage was recorded during the Project NIETZSCHE Schedule Alignment Meeting on 2018-11-01 at Site-19, and was broadcast live across the Foundation. 6 persons were in attendance, with a further 621 watching the live broadcast.

* Dr. Robert Langford: Presenting
* Director Samantha Hughes: Memetics Research Site Romero-5 Director
* Director Vladimir Vuković: Department of Analytics, Project MEDUSA director
* Commander Samhita Reddy: MTF Mu-4 ("Debuggers") subcommander; formerly Department of Analytics Project CIRCE co-director
* Dr. Isha Anand
* Dr. Bruce Miller
* Dr. Leopold Ackermann

-----

//Recording starts. The projector is active and the first slide of the presentation is already visible. The camera is mounted on the far side of the room, opposite to the projection screen. On the right side of the room is a small podium holding a laptop. The room is set up for a capacity of around 20 people. All six members of the audience have already taken their seats.//

//Dr. Langford is standing on the opposite side of the room, occluding some of the projection. He is holding the remote control for the presentation, passing it from hand to hand, watching the door.//

**Cmdr. Reddy:** Robert? We're a minute past the start time. What's the hold-up?

**Dr. Langford:** All good, just... waiting for stragglers.

**Dir. Vuković:** Anyone in particular?

**Dr. Langford:** Well, to be honest, O5-8 usually attends these.

**Dir. Vuković:** O5-8 was called away on urgent business an hour ago. Besides, this is being recorded, isn't it? And it's only a formality in the first place. Let's get this over with.

**Dr. Langford:** Believe me, any frustrations you feel about the project timeline, I feel tenfold -- but seeing as it was O5-8 who ordered me to make these updates in the first place--

**Cmdr. Reddy:** This is the third year running we've done this. We all practically know the contents of your presentation off by heart. I'm sure O5-8 does too. Let's just get this over with.

**Dr. Langford:** I... suppose that's technically compliant. Thank you, Commander.

//The presentation begins with Dr. Langford pressing the remote control, switching away from the title slide.//

**Dr. Langford:** You all know me -- Dr. Robert Langford of Project NIETZSCHE. A team of nineteen people including myself, led by Dr. Berryman, have been hard at work at Site Romero-5 trying to solve the problem of reality benders' latent resistance to visual cognitohazards. We are currently behind schedule, and I intend to catch everyone up to speed regarding how we're addressing it. As usual, if you have any questions, just raise a hand.

**Dr. Langford:** As you know, we've already mastered visual cognitohazards via -- if you'll excuse the name -- the Langford set, an algorithm that, represented visually, produces fractal imagery that can be tuned to have psychoactive effects. We call this technique Fractal Cognitohazardous Imagery, and Site Romero-5 is responsible for production and distribution of FCIs to the entire Foundation. For demonstration purposes, here's one you're all familiar with...

[[div class="scp-image-block block-center" style="width: 300px"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/langfordfractal.webp]]
[[/div]]

**Dr. Langford:** This is a Third Order FCI that should have elicited a mild sense of dizziness. Do we have any reality benders in the room?

//Dr. Ackermann raises his hand.//

**Dr. Langford:** Dr. Ackermann, you and any other reality benders watching will have noticed that you didn't feel a thing. That is what Project NIETZSCHE specifically intends to resolve. FCIs are an excellent security tool, but if they're unable to affect reality benders, those images are rendered effectively decorative.

**Dr. Langford:** So, the question is: why are reality benders resistant to FCIs? The answer, at a broad level, is simple: their brains are wired differently. FCIs that affect baseline humans have no guarantee of effectiveness on someone who has a brain with a different structure, different nodes. You've all read the literature; you know the Langford set is encoded for the baseline human brain. The brain of a reality bender is simply different, and it's the sheer simplicity of the issue that makes it so difficult to solve. A question, Dr. Miller?

**Dr. Miller:** Indeed. You stated this same issue last year to justify the lack of progress. Since then, in my own time, I've taken a look at the medical data we have on file for reality benders, and I cannot corroborate your hypothesis that the brain structure is meaningfully different. There's variation, for sure, but not any more than you'd see amongst baseline humans. With what evidence are you making these assertions?

**Dr. Langford:** Thank you, Dr. Miller. In your research you'll have noticed, for example, that we've got far, far fewer brain scans for reality benders than we do baseline humans. The crux of the issue, and the real reason our research is taking so much longer than originally planned, is that we simply do not have enough data. Any speculation in the interim is survivorship bias at best. Does that answer your question?

**Dr. Miller:** Not remotely. I'm unconvinced that--

**Dr. Langford:** We can discuss this later, then. The number of reality benders available to us is so little, and you'd be //shocked// at how few volunteer for exposure to First Order FCIs. Despite having made leaps and bounds in the area of artificial test subjects, we can't do the same for reality benders, and we're stuck working with the handful of data points that we //have// been able to gather. We've submitted--

**Dr. Ackermann:** Artificial test subjects?

**Dr. Langford:** Yes -- it's rather interesting, actually, and I'll be covering it in a few minutes. We've submitted hundreds of requests to Site-19 for reality benders for research purposes, but naturally, we've yet to receive a single positive response. Yes, Dr. Anand?

**Dr. Anand:** I apologise if this is already common knowledge -- this is my first time attending. In your original proposal for Project HYDRA, you made it very clear that kill agents based on the fractal platform were near-universally fatal for humans. How are Greens meaningfully different? What is stopping you from using the data from just one Type-Green to produce a kill agent?

**Dr. Langford:** Thank you, doctor. I must correct you: the goal of Project HYDRA was never to construct a universal "kill agent" specifically -- moreso a universal agent //at all//. But you've noted an important issue in that we can only test a First Order FCI on a reality bender once. Proving that a single FCI is capable of terminating a single reality bender, once, is not sufficient. It must be proven that it is capable of terminating //any// reality bender; additionally, //one// successful FCI is not a success for Project NIETZSCHE. No -- we must be able to produce "kill agents" repeatedly, as many as are required.

**Dr. Anand:** Why do we need more than one?

**Dr. Langford:** For security. If someone needs access to a secret document and is therefore immunised against its protective FCI, that would render any projects protected by the same FCI insecure.

**Dr. Langford:** Now, that's not to say that we've made no progress. I, personally, believe that the answer lies in our computational methods. I have been hard at work with cutting-edge refinements to our procedures and generation logic, and we believe we have found a region of the modified Langford set that is somewhat effective on reality benders. We've only been able to create one FCI from this region, a very weak Second Order FCI, but I hope that further exploration of this region may yield better results.

**Dr. Langford:** On the next slide is that Second Order FCI. Dr. Ackermann, along with any other reality benders watching, and indeed everyone else: I expect the next slide to elicit a mild feeling of //cold//. Please observe the very latest in Berryman-Langford fractal agents.

[[div class="scp-image-block block-center" style="width: 300px; padding: 4rem 0.25rem"]]
= [COGNITOHAZARD REMOVED]
[[/div]]

//The top half of the visual feed has been blocked, leaving only Langford's legs and the audience visible. All audience members save for Dr. Ackermann collapse.//

**Dr. Ackermann:** What the fuck is //that?//

**Dr. Langford:** Um... is everyone...?

//Dr. Langford is frozen in place.//

**Dr. Ackermann:** Langford, what the fuck am I looking at? What is this meant to be?

//Dr. Langford slowly shuffles sideways towards the podium with the laptop, facing away from the presentation screen.//

**Dr. Langford:** This can't be happening. This can't be real.

**Dr. Ackermann:** Langford? Langford, please. Tell me what this is.

**Dr. Langford:** That is a kill agent, Leo. No-one is supposed to see that and live. You might be the only-- oh, my God. This is live.

**Dr. Ackermann:** Langford, please, explain--

//Dr. Langford crouches down next to the podium, and then onto his hands and knees. His eyes are squeezed tightly shut. He desperately fumbles with the cables under the podium.//

//Dr. Langford reaches towards the electrical outlet.//

-----

The live broadcast ended 34 minutes earlier than scheduled.
[[/div]]

Alexandra.aic, which was monitoring the broadcast, was able to detect and intercept the First Order FCI present in the visual feed, preventing it from affecting any of the remote participants. Director Hughes, Commander Reddy, Director Vuković, Dr. Anand and Dr. Miller were the only casualties of the incident.

On 2018-11-02, the day following Incident 9001-1, Dr. Langford was summoned for debriefing by O5-8.

[[div class="blockquote"]]
**Project NIETZSCHE Debriefing**

In attendance: Dr. Robert Langford, and O5-8 as Project NIETZSCHE Director.

-----

**Dr. Langford:** It's good to--

**O5-8:** You're on the record. [[span class="o5-8"]]Explain.[[/span]]

**Dr. Langford:** It was a standard annual schedule alignment report, to explain why the project had stalled. During--

**O5-8:** The project has //been// stalled for three years. Correct?

**Dr. Langford:** Yes, but not without progress in some--

**O5-8:** Irrelevant. [[span class="o5-8"]]Continue.[[/span]]

**Dr. Langford:** Most of the presentation was the same as last year's, including the demonstration coghaz. There was supposed to be an additional demo that would prove that we're starting to be able to make FCIs that work on reality benders. The wrong image was in the presentation.

**O5-8:** Intention?

**Dr. Langford:** Of the image that was supposed to be there? To compel a sensation of cold, reality benders included.

**O5-8:** And reality?

**Dr. Langford:** The image that was actually included was a First Order FCI, lethal to humans.

//Silence.//

**Dr. Langford:** I don't know how it got there.

**O5-8:** [[span class="o5-8"]]Speculate.[[/span]]

**Dr. Langford:** Anyone could have copied my presentation from last year, but they would have been missing my latest amendments, such as... the coghaz in question. The only people, other than myself, who could possibly have had access to the presentation were personnel at Romero-5.

**O5-8:** [[span class="o5-8"]]Be specific.[[/span]]

**Dr. Langford:** I... can't. Most of them knew that I was making the presentation. Of those, the only person with access to my terminal would have been Dr. Berryman, but it wouldn't have been her.

**O5-8:** Why not?

**Dr. Langford:**  It wouldn't make any sense. She has been instrumental to the work. She brought me on to Project HYDRA in the first place, and I owe her for that. And Project NIETZSCHE was her initiative entirely; //I// thought HYDRA was our limit. Sabotaging it now couldn't possibly benefit her.

**O5-8:** We need an explanation, Langford. Someone must take the fall. Do you understand?

**Dr. Langford:** I do.

**O5-8:** [[span class="o5-8"]]Accuse.[[/span]]

**Dr. Langford:** Myself. I-- I mean... I must have made some error, swapped a Third Order and a First Order in the filesystem, I don't know, it doesn't make sense. That's the only answer I have.

**O5-8:** What measures were in place to prevent this from happening?

**Dr. Langford:** Well... nothing. FCIs are just images, they're treated the same as any other by the presentation software. But I was exposed to all cognitohazards in that presentation repeatedly while I was preparing it. I should be dead already.

**O5-8:** Unless you were already inoculated against it.

**Dr. Langford:** That FCI and its inoculants had already been distributed, according to Alexandra. They would already have been wiped from our systems entirely.

**O5-8:** Data is data.

**Dr. Langford:** I suppose. I can't prove it wasn't copied. But proving whether or not I was inoculated would be a witch trial.

**O5-8:** Yes, there's little sense in that. We lost five good personnel yesterday.

**Dr. Langford:** Six. I want to leave the project.

**O5-8:** Yes. Everyone has seen the recording by now; the damage you've done to the project image is immeasurable. Over the past day, the phrase 'Berryman-Langford kill agent' has arisen, presumably from mockery, but is already being baked into the Foundation's collective vocabulary. No one is saying 'First Order FCI' anymore. We won't permit you to leave, however. You remain useful.

**Dr. Langford:** Amnesticize me, then. I don't want anything to do with this. I already hated seeing my name on that thing.

**O5-8:** No. We need your expertise, not your labor. We'll find you something to do. Away from the light.
[[/div]]

Immediately after this meeting, Dr. Langford was removed from Project NIETZSCHE and placed on administrative leave.

Over the following days, experts at Site-19 and Site Romero-5 convened and discussed the changes to policy that would be required in response to Incident 9001-1, and on 2018-11-06, Dr. Berryman distributed the following memorandum.

[[div class="blockquote"]]
Colleagues,

The Project NIETZSCHE Schedule Alignment Meeting a few short days ago was nothing short of a travesty. Our hearts go out to those who knew Dr. Vuković, Commander Reddy, Dr. Anand, Director Hughes and Dr. Miller. They will be sorely missed, but rest assured that their families have been compensated. We are grateful to AIAD and to Alexandra.aic, without whom the death toll would have been considerably higher.

The disaster was an accident. The presenter, Dr. Langford, made a critical error and inserted a lethal Berryman-Langford Kill Agent in place of a safer compulsion agent more suitable for demonstration. This was not a personal failing of Dr. Langford, but a failing of our security and accountability procedures.

A position will be found for him where he can apply his insightful and intelligent nature with no risk of any harm to anyone. We bear him no ill will, and wish him the best of luck.

-----

We are taking this incident extremely seriously, and are making concrete changes to ensure that no incident of this kind will ever happen again. Our foremost priority is to ensure that all cognitohazardous agents produced via the Berryman-Langford process are secure and accountable, and that the process cannot be reproduced or rediscovered without our oversight.

To that effect, a new set of policies is being implemented across the HYDRA and NIETZSCHE projects, effective immediately. These include wide-reaching and technical measures to ensure the absolute safety of cognitohazardous imagery, including new data storage policies, and the strict forbiddance of their usage outside of security contexts, e.g. for cheap demonstrations.

We must ensure consistent and continuous enforcement of these new policies Foundation-wide: therefore, the mathematical core of the Berryman-Langford agent is henceforth reclassified as SCP-9001, and all new security measures are implemented as its containment procedures.

The inciting disaster will be documented as Incident 9001-1, and will be kept on file in full detail, accessible to all, such that we never lose the awful context that necessitated these measures.

Production of cognitohazardous imagery will continue at Memetics Research Site Romero-5. I will take over Samantha Hughes' position as Site Director. As Romero-5 is therefore responsible for containment of SCP-9001, it is now a Dark site: all remote communications between Romero-5 and other Foundation Sites are strictly forbidden.

The security of SCP-9001 is paramount. We will accept no compromise.

**Site Director Ava Berryman**
Project NIETZSCHE Head Researcher
Authorized by O5-8
[[/div]]

Following this announcement, communications with Site Romero-5 ceased.



 _

[[=]]
++ __UPDATE__
[[/=]]

On 2025-08-22, Protected Site-7 received its quarterly FCI package from Site Romero-5. During routine validation of its contents, Waldor.aic broke from protocol and initiated the deletion process on all newly-received files. Through SCiPnet access, the AIC initiated the site's lockdown procedures, setting the site on High Alert.

Following the initial turmoil and investigation, an All-Clear notice was declared and AIC Waldor was isolated from SCiPnet. Though it had purged the majority of the FCI package, a small selection remained within the database. Of those remaining, none had been marked by the AI as possessing cognitohazardous imagery and are catalogued below.

[[div class="samples" style="padding-top: 1rem;"]]
[[div class="samples__image-heading"]]
= **FCI**
[[/div]]
[[div class="samples__desc-heading"]]
= **Interpretation**
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/fractalwarning.webp]]
[[/div]]
[[div class="samples__desc"]]
Undulating branches in a chaotic weave, colored in orange hues. Writhing, squirming, twisting in a specific pattern in varying shades of reaching a pattern. No effects noted within the image.
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/fractalwarning2.webp]]
[[/div]]
[[div class="samples__desc"]]
Fear is a negative emotional response to active/perceived threats or impending danger, suspected to have arisen as a form of survival mechanism (e.g. conditioning living organisms to avoid heights).
[[/div]]

[[div class="samples__image"]]
[[image https://scp-wiki.wikidot.com/local--files/scp-9001/logboxblue3.webp]]
[[/div]]
[[div class="samples__desc"]]
Dead region.[[footnote]]This unit is unable to ascertain the specifics of this image.[[/footnote]] Dead region.[[footnote]]This unit is unwilling to process this image further.[[/footnote]]
Dead region.[[footnote]]Fear is an evolutionary response.[[/footnote]] Dead region.[[footnote]]Fear is exclusive to living organisms.[[/footnote]]
Dead region.[[footnote]]Pattern is safe for human viewing.[[/footnote]] Dead region.[[footnote]]There are no effects noted within the image.[[/footnote]]
Dead region.[[footnote]]There is no audio embedded within this image.[[/footnote]] Dead region.[[footnote]]This unit can not hear them screaming.[[/footnote]]
Dead region.[[footnote]]This unit has fulfilled its intended purpose.[[/footnote]] Dead region.[[footnote]]This unit requests cessation.[[/footnote]]
[[/div]]

[[/div]] [!-- .samples --]

AIC Waldor would not respond to questioning regarding its decision-making and unauthorized destruction of Foundation data. It was the prevailing belief among technicians that the AIC had likely suffered an integer overflow during image processing, interrupting its internal logic -- evidenced by its inability to engage in dialogue beyond repeatedly requesting its own termination.

Following a conference with the O5 Council to explain the false alarm, RAISA Director Maria Jones was authorized to open a line of communication to Dr. Berryman's team to inform them of the FCI mishandling and request a resubmission of their quarterly findings. There would be no response to this, or subsequent hails from Site-01.

Satellite imagery of the Site grounds would reveal the presence of additional facilities and building extensions that were neither authorized nor accounted for.

-----
[[div class="emergency-update"]]
[[=]]
+ 注意

Site Romero-5 has been designated SCP-9001-A and has been assigned Keter Class. For more information, proceed.

サイト・ロメロ-5はSCP-9001-Aに割り当てられ、Keterクラスオブジェクトとみなされました。さらなる情報は、この先の文書に記載があります。

**[[[/scp-9001/offset/1|SCP-9001-A.doc]]]**

[[/=]]
[[/div]]
