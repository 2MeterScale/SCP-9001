[[include :scp-wiki:component:hoverlinks]]

[[include :scp-jp:theme:black-highlighter-theme]]
[[include :scp-jp:theme:jakstyle]]

[[module css]]
/* Jakstyle modifications */
/* Recover default selection styles */
::-moz-selection, ::selection {
    background: Highlight; color: HighlightText;
}
#header h1 a::before { -webkit-text-stroke-width: 3px }
#header h2 span::before { -webkit-text-stroke-width: 2px }
div.page-rate-widget-box { margin-bottom: 0.25rem }
[[/module]]

[[module css]]
.equation-number {
  display: none;
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

.hover span { display: none; }
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

/* Better image block positioning from component:croqstyle */
@media (max-width: 550px), (min-width: 768px) and (max-width: 850px) {
  .scp-image-block:is(.block-right, .block-left) {
    float: none;
    margin-inline: auto;
  }
}

.explo-root {
  /* How deep the most deeply-nested explo block is. Topmost block is 0. */
  --max-nest-depth: 11;

  /* Desired width of the most deeply-nested explo block. */
  --crush-width: 8ch;

  container-type: inline-size;
  --border-width: 4px;
  --padding-inline: calc((50cqw - (var(--crush-width) / 2) - (var(--border-width) * var(--max-nest-depth))) / var(--max-nest-depth));

  @media (max-width: 600px) {
    --border-width: 3px;
    --crush-width: 7ch;
    margin-inline: -3vw;
   }
}
.explo {
  border: var(--border-width) solid #444444;
  margin-block: 1.5rem;
  padding-inline: var(--padding-inline);
  padding-block: 0.5rem;
}
.explo--room {
  box-shadow: 0px 1px 6px rgba(0, 0, 0 , 0.2);
}
.explo--threshold {
  background-color: rgba(0, 0, 0, 0.2);
  border-style: dashed;
}

.explo-rising {
  text-align: center;
  margin-block: -1em;
}
.explo:has(> .explo-rising:last-child) {
  border-bottom-color: transparent;
  padding-bottom: 0.25rem;
}

body { overflow-x: hidden }
.berryman {
  background-image: url(http://scp-wiki.wikidot.com/local--files/scp-9001/berrymanfractal.webp);
  background-attachment: fixed;
  background-position: center;
  background-size: 100vw auto;
  max-width: none !important;
  width: 100vw;
  position: relative;
  left: calc(50% - 50vw);
  font-family: monospace, monospace;
  color: white;
  text-align: center;
  padding: 0.1rem 0;
  box-shadow: inset 0px 2px 4px rgba(0, 0, 0, 0.6);
  min-height: 4rem;
  align-content: center;
  font-size: 1.1em;

  span {
    background-color: rgba(0, 0, 0, 0.6);
    border-radius: 3px;
    padding: 1px 8px;
    text-shadow: 0px 0px 6px black;
  }
}
.berryman--angrier {
  background-image: url(http://scp-wiki.wikidot.com/local--files/scp-9001/Berrymanspiral2.webp);
}

.explo strong, .blockquote strong {
  color: rgb(230, 230, 230);
}

#main-content hr {
  height: 1px;
  border-top: 2px solid #777;
  border-bottom: 1px solid #777;
  margin-block: 1rem;
  background: none;
}

.conprocs {
  border: thin solid #f005;
  background: #ff000005;
  padding-inline: 1rem;
  border-radius: 4px;
  position: relative;
}
.conprocs::before, .conprocs::after {
  content: "";
  height: 0.3rem;
  left: 0;
  right: 0;
  background-image: repeating-linear-gradient(135deg, darkred 0ch, darkred 1ch, crimson 1ch, crimson 1.75ch, darkred 1.75ch);
  position: absolute;
}
.conprocs::before { top: 0 }
.conprocs::after { bottom: 0 }

#footer { background: transparent }
@media (min-width: 901px) {
  #container {
    background-image: url(http://scp-wiki.wikidot.com/local--files/scp-9001/lichten.webp), url(
http://scp-wiki.wikidot.com/local--files/scp-9001/lichten-flip.webp);
    background-position: calc(50% - 40rem) calc(100% + 20rem), calc(50% + 40rem) calc(100% + 20rem);
    background-repeat: no-repeat;
    background-size: auto 100rem;
  }
}
@media (max-width: 900px) {
  .footnotes-footer {
    background-image: url(http://scp-wiki.wikidot.com/local--files/scp-9001/lichten.webp), url(http://scp-wiki.wikidot.com/local--files/scp-9001/lichten-flip.webp);
    background-position: calc(50% - 30vw) calc(100% + 20rem), calc(50% + 30vw) calc(100% + 20rem);
    background-repeat: no-repeat;
    background-size: auto 100rem;
  }
}
[[/module]]

[[include :scp-jp:info:start]]
翻訳責任者: [[*user 2MeterScale]]
翻訳年: 2025
著作権者: [[*user S D Locke]]、[[*user Croquembouche]]、[[*user PandoraNuker]]
原題: Fractal
作成年: 2025
初訳時参照リビジョン: 52
元記事リンク: https://scp-wiki.wikidot.com/scp-9001
[[include :scp-jp:info:end]]

-----

[[table style="border: none; width: 100%;"]]
[[row]]
[[cell]]
[[size 125%]]**アイテム番号:** SCP-9001-A[[/size]]
[[/cell]]
[[cell style="text-align: right;"]]
[[size 125%]]###f00d|**レベル2/9001**##[[/size]]
[[/cell]]
[[/row]]
[[row]]
[[cell]]
[[size 125%]]**オブジェクトクラス:** Keter[[/size]]
[[/cell]]
[[cell style="text-align: right;"]]
[[size 125%]]###f00d|**Classified**##[[/size]]
[[/cell]]
[[/row]]
[[/table]]

-----

[[div class="scp-image-block block-center" style="width:100%;"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/hammerdown.webp alt=""]]
[[div class="scp-image-caption"]]
機動部隊ニュー-7("下される鉄槌")の打撃部隊による、サイト・ロメロ-5に対する、初期の攻撃
[[/div]]
[[/div]]

-----

[[div class="conprocs"]]
[[span style="color: white; background: #f008; padding: 3px 5px 1px; border-radius: 3px; text-transform: uppercase; font-weight: bold; margin-left: -2.5px"]]緊急収容プロトコル:[[/span]] An Exclusion Zone has been established 3km from the event horizon of SCP-9001-A, and is enforced by an array of Scranton Reality Anchors. As of this writing, the local supply of anchors has been exhausted; additional materials from Site-118 are currently en-route.

SCP-9001-Aの事象の地平面から3kmの位置に立入禁止区域が設定され、当該地域には多数のスクラントン現実錨が展開されています。本稿執筆時点において、現地における現実錨の備蓄は枯渇しており、サイト-118からの追加資材の輸送が進行中です。

Agent Troy Lament has assumed the role of General Commander of Task Forces in the region, operating out of Forward Operating Base Panloque, established outside the bounds of the SRA array. Operatives from Mobile Task Forces [[span class="hoverlink"]][[[task-forces#eta-10|Eta-10]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Eta-10 ("See No Evil")[[/span]][[span class="hoverlink-text"]]Specialists in circumventing/containing perceptual hazards. Eta-10 uses specialized equipment (such as the "SCRAMBLE" goggles) in order to protect its agents from anomalous effects triggered or expressed through sensory perception[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Eta10.png/small.jpg)"]]-[[/span]][[/span]][[/span]], [[span class="hoverlink"]][[[task-forces#theta-90|Theta-90]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Theta-90 ("Angle Grinders")[[/span]][[span class="hoverlink-text"]]Experienced pathfinders and wayfarers in areas where local topography does not align with conventional understanding of spacetime, such as iterative, recursive, and infinite zones. Theta-90 specialists are also tasked with diplomatic missions into non-hostile Nexus locales.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Theta90.png/small.jpg)"]]-[[/span]][[/span]][[/span]], [[span class="hoverlink"]][[[task-forces#epsilon-11|Epsilon-11]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Epsilon-11 ("Nine-Tailed Fox")[[/span]][[span class="hoverlink-text"]]Specialists drawn from across the MTF network, deployed to establish control of Foundation Sites experiencing breaches and/or occupation by hostile forces and GoIs. Famous for their efforts in combating a containment breach at Site-19.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Epsilon11.png/small.jpg)"]]-[[/span]][[/span]][[/span]] and [[span class="hoverlink"]][[[task-forces#zeta-9|Zeta-9]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Zeta-9 ("Mole Rats")[[/span]][[span class="hoverlink-text"]]An exploration team tasked with probing and mapping underground or ontologically unsound areas. Typically deployed as a first-line resource, Zeta-9 has a notoriously-high mortality rate. Despite this, Zeta-9 operatives are seen by many to be the most capable for exploration of any sort.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Zeta9.png/small.jpg)"]]-[[/span]][[/span]][[/span]] are being assembled into special teams for exploration of the Zone. MTF [[span class="hoverlink"]][[[task-forces#iota-10|Iota-10]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Iota-10 ("Damn Feds")[[/span]][[span class="hoverlink-text"]]Personnel embedded within law enforcement and similar institutions. As a public-facing entity, Iota-10 is usually tasked with intelligence-gathering, working alongside government agencies and local police. Iota-10 also serves as an early-warning for civilian anomalies.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Iota10.png/small.jpg)"]]-[[/span]][[/span]][[/span]] is tasked with diverting civilians from the area.

エージェント・トロイ・ラメントが当該地域の機動部隊総司令官に着任し、SRA展開領域外に設立された前線基地パンロケを拠点として活動しています。機動部隊 [[span class="hoverlink"]][[[task-forces#eta-10|エータ-10 ("シー・ノー・イーヴル")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]イータ-10 ("シー・ノー・イーヴル")[[/span]][[span class="hoverlink-text"]]知覚災害の回避/収容を専門とする。イータ-10は、感覚知覚を介して発現・誘発される異常効果からエージェントを保護するため、特殊装備（「SCRAMBLE」ゴーグルなど）を使用する。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Eta10.png/small.jpg)"]]-[[/span]][[/span]][[/span]]、[[span class="hoverlink"]][[[task-forces#theta-90|シータ-90 ("角度研削者")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]シータ-90 ("角度研削者")[[/span]][[span class="hoverlink-text"]]反復的、再帰的、無限的な領域など、局所的な地形が従来の時空理解と一致しない領域における、経験豊富な経路探索者および踏破者。シータ-90の専門家は、非敵対的なネクサスへの外交任務も担当する。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Theta90.png/small.jpg)"]]-[[/span]][[/span]][[/span]]、[[span class="hoverlink"]][[[task-forces#epsilon-11|イプシロン-11 ("九尾狐")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]イプシロン-11 ("九尾狐")[[/span]][[span class="hoverlink-text"]]MTFネットワーク全体から選抜された専門家であり、敵対勢力や要注意団体による侵害や占拠を経験した財団サイトの統制を確立するために配備される。サイト-19での収容違反への対処で有名。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Epsilon11.png/small.jpg)"]]-[[/span]][[/span]][[/span]]、そして[[span class="hoverlink"]][[[task-forces#zeta-9|ゼータ-9 ("メクラネズミ")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]ゼータ-9 ("メクラネズミ")[[/span]][[span class="hoverlink-text"]]地下または存在論的に不安定な領域の探査と地図作成を任務とする探査チーム。通常、第一次投入リソースとして配備されるゼータ-9は、死亡率の高さで悪名高い。それにもかかわらず、ゼータ-9の工作員はあらゆる種類の探査において最も有能であると多くの者に見なされている。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Zeta9.png/small.jpg)"]]-[[/span]][[/span]][[/span]]の工作員らが、区域の探索を目的とする特別チームとして編成されつつあります。機動部隊[[span class="hoverlink"]][[[task-forces#iota-10|イオタ-10 ("ポリ公")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]イオタ-10 ("ポリ公")[[/span]][[span class="hoverlink-text"]]法執行機関および類似の機関に潜入している職員。公的な存在として、イオタ-10は通常、政府機関や地方警察と協力して情報収集を任務とする。イオタ-10はまた、民間における異常存在の早期警戒としても機能する。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Iota10.png/small.jpg)"]]-[[/span]][[/span]][[/span]]は、当該地域から民間人を迂回させる任務を負います。

The Exclusion Zone's perimeter is to be enforced by Armed Mobile Task Force [[span class="hoverlink"]][[[task-forces#nu-7|Nu-7]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Nu-7 ("Hammer Down")[[/span]][[span class="hoverlink-text"]]A battalion-strength regiment of soldiers and combat/vehicle specialists. Deployed in events where Foundation facilities have been compromised, or when containment calls for the use of overwhelming force.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Nu7.png/small.jpg)"]]-[[/span]][[/span]][[/span]], who have been tasked with carrying out a controlled burn of the forest within the zone.

立入禁止区域の境界線は、武装機動部隊[[span class="hoverlink"]][[[task-forces#nu-7|ニュー-7 ("下される鉄槌")]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]ニュー-7 ("下される鉄槌")[[/span]][[span class="hoverlink-text"]]兵士および戦闘/車両の専門家からなる大隊規模の連隊。財団施設が危険に晒された場合、または収容に圧倒的な戦力の行使が必要な場合に配備される。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Nu7.png/small.jpg)"]]-[[/span]][[/span]][[/span]]によって確保されることになっており、同部隊は区域内の森林の計画的焼却を実行する任務を課せられています。

Living organisms attempting to cross the SRA boundary are to be summarily terminated. The remains of any affected lifeforms are not to be taken for research purposes -- they are to be deposited back within the bounds of the Exclusion Zone and incinerated.

SRA境界線を越えようと試みる生命体は、即時終了されます。当該地域の影響を受けた生命体を研究目的での回収することは、許可されていません。それら生命体は立入区域内に投棄され、焼却処分を受ける必要があります。

Should the area-of-effect expand beyond the Exclusion Zone, an All-Hands Notice is to be issued worldwide in preparation for a ZK-Class Reality Failure Scenario.

効果範囲が立入禁止区域を越えて拡大した場合、ZK-クラス:現実不全シナリオに備え、全世界の全職員に向けて通達が発せられます。
[[/div]]

**Description:** SCP-9001-A refers to an expanding region characterized by non-Euclidean geometry, spatial inconsistencies, and the elaborate growth and fractalization of complex systems.

**説明:** SCP-9001-Aは、非ユークリッド幾何学、空間的不整合、および複雑系の精巧な成長とフラクタル化を特徴とする、拡大領域です。

SCP-9001-A is expressed through the formation of vestigial facilities emerging from Site Romero-5, the shifting of local topography and meteorological conditions with a preference for fractal organization, and the induction of physiological mutations in living organisms within its area of effect.

SCP-9001-Aの発現は、サイト・ロメロ-5から出現する痕跡的な施設の形成、フラクタル構造を指向する局所的な地形および気象条件の変化、そしてその効果範囲内の生命体における生理学的変異の誘発といった形で現れます。

The means through which SCP-9001-A comes to infect a new system is currently unknown, as early observations have ruled out direct contact as a strict prerequisite. It is possible that transmission occurs through metaphysical, conceptual, or associative means. Research conclusions are not yet definitive due to the rapidly evolving situation.

初期の観測において、直接接触が厳密に必須条件ではないと判断されたため、SCP-9001-Aが新たなシステムに感染する手段は現在のところ不明です。伝播は形而上学的、概念的、あるいは連想的な手段を介して発生する可能性があります。状況が急速に変化しているため、当該オブジェクトに対する研究において、最終的な結論は示されていません。

SCP-9001-A came to the attention of the wider Foundation following the first-hand experience of Special Operative Saunders.

SCP-9001-Aは、特別工作員ソーンダースによる遭遇を経て、財団全体の注意を引くこととなりました。

**Discovery:** Special Operative Saunders was deployed to investigate the state of affairs following loss of contact with Dr. Berryman's team. S.O. Saunders was chosen due both to her immediate locality[[footnote]]S.O. Saunders had been embedded within the police force of the town of Willow Falls, located 10km south of Site Romero-5. She had been tasked with the investigation of a rash of missing-persons cases that had occurred over a 10-month period.[[/footnote]] and personnel CRV rating that would allow her to bypass protective cognitohazards embedded into signs posted along the sole access road.

**発見:** 特別工作員ソーンダースは、ベリーマン博士のチームとの連絡途絶を受け、事態の調査のために派遣されました。ソーンダース特別工作員が選抜されたのは、彼女が地理的に近接していたこと[[footnote]]ソーンダース特別工作員は、サイト・ロメロ-5の南10kmに位置するウィロー・フォールズの町の警察に潜入していました。彼女は、10ヶ月間にわたって発生していた連続失踪事件の調査を任務としていました。[[/footnote]]、そして当該地域に唯一アクセス可能な道路沿いにおける標識に埋め込まれた防護認識災害を迂回できるだけの認知抵抗値（CRV）を有していたこと、その双方によります。

-----

[[div class="blockquote"]]

= {{**映像ログ**}}

----

The video opens, askew, from the perspective of the passenger seat looking up at S.O. Saunders, driving with a nondescript expression. A flurry of trees can be seen beyond the driver's side window. As the vehicle shifts around a bend, bright specks of orange daylight play across the vehicle's interior, prompting Saunders to swing the visor down. A look of confusion crosses her face.

やや斜めになっている画面には、特務工作員ソーンダースが映し出されている。彼女は仏頂面を浮かべながらハンドルを握っていた。鬱蒼とした木々が、さながら一個の塊のようになって窓の外を流れてゆく。その枝葉の隙間から夕陽の光が漏れ、車内をまだらな橙色に染め上げていた。ソーンダースはサンバイザーを下ろした。彼女の顔に、困惑の色が浮かぶ。

Saunders hails Command, asking to double-check her positioning to confirm she's on the correct path. It is verified that she is. Rolling her eyes, Saunders implies incompetence on Command's part, owing to the fact that the access road was purported to be a direct line, whereas her current path is taking her down a long road with a subtle curve.

彼女は司令部を呼び出し、自身がいるべき場所にいて、正しい道を走っているかの確認を要請した。この進入路はまっすぐな道のはずだった。だが、違う。いま、彼女は微妙なカーブが続く、長い道を走っている。やがて正しい、との返答を得ると、ソーンダースはやれやれと言わんばかりに目を顰めた。司令部の手際の悪さは今に始まったことではない、とでも言いたげな態度であった。

Command notes the discrepancy. Saunders is asked to relay any peculiarities regarding her surroundings, but only notes that the road itself is in disrepair, with overgrown foliage and weeds encroaching on either side of the blacktop. It is as she's explaining this to Command that she trails off, leaning forward with a confused expression.

司令部も、その不一致を記録す流。続けて彼女に対し周囲の異変についての報告を求めた。道が荒れ果て、アスファルトの両脇から野放図に草木が伸びている。それ以外、特筆すべきことはない。そう言い終わらないうちに、彼女は口篭って、訝しげな表情を浮かべながら身を乗り出した。

The flurry of trees begins to slow until the vehicle comes to a complete stop. Saunders flashes a quick glance towards the camera and shifts into park. There is a momentary jostling of the camera's field of vision as Saunders places her helmet on and exits the vehicle.

流れゆく木々の速度が緩やかに落ちてゆき、やがて車が止まる。ソーンダースはカメラに軽く一瞥をくれると、ギアをパーキングに入れた。映像がわずかに揺れる。彼女はヘルメットを装着し、車の外に出た。

From her perspective, it can be seen that thick, gnarled root systems of surrounding trees have fully disrupted the roadway, causing it to fracture and splinter, with one nearby root growing around and dislodging a deer-crossing sign. It appears as if the road had not been used in decades.

そこは、まるで何十年も放置されていた廃道のようだった。アスファルトは粉々に砕け、道路は裂けてしまっている。周りの木々から伸びている、太く節くれた根が舗装を完全に破壊していた。あるいは鹿横断注意の標識に絡みつき、その支柱すら引き抜いてしまっている。

After brief deliberation, it is decided Saunders should continue on foot. She leans into the vehicle to retrieve her keys from the ignition, and closes the door behind her.

多少の議論のすえ、ソーンダースは徒歩で進むこととなった--　　--体を屈めてイグニッションから鍵を抜く。そのまま彼女は後ろ手にドアを閉じた。

Without the rumble of the engine, the near-silence of the surrounding wilderness comes into focus. There is no birdsong, nor chirping of insects. There is only a quiet creaking from an unknown source, likened by Saunders to that of old wooden floorboards. She sets off, stepping over the obstructing roots as she progresses.

エンジンの唸りが消える。鳥の囀りも、虫の鳴き声もない。ただどこかから聞こえる軋むような音がある以外は、静寂そのものであった。ソーンダースはこれを、まるで古い木の床板のようだと喩えた。行く先を遮っている木の根を踏みしめながら、彼女は歩みを進めてゆく。

Saunders continues for the next kilometer at a measured pace. Though near enough to the site on GPS that she'd presumably spot it in the distance, the curvature of the road only seems to increase as she progresses. The path ahead veers further and further to the left, limiting the length that can be seen. Further impacting visibility is the sheer depth of the canopy above, blocking out most sunlight. What little daylight that does break through is itself dimming as thick clouds roll over the area.

続く一キロメートルを、彼女は慎重な足取りで進む。GPS上の位置からすれば、サイトの建物が遠方に見えていてもおかしくはないところまで来ているはずだった。だが、道のうねりは激しくなるばかりである。続く道は左へ左へとさらに逸れていて、見通しが効かない。木の枝が天蓋じみて頭上を覆っている。わずかにその隙間から差し込む光も、厚い雲によって遮られてしまっている。辺りは薄暗い。

A blaring horn is heard in the distance. Quickening her pace, Saunders rounds the bend, coming to see a black sedan some distance ahead. It appears that the vehicle had flown off the road and crashed headfirst into a nearby tree. The windshield is marred in a cobweb of broken cracks. The driver's-side door is ajar. Though its plate cannot be seen, Command is able to identify that it would have belonged to one of the researchers on-site.

遠くから、けたたましいクラクションが響いた。ソーンダースは歩調を速める。曲がり道の先に、黒いセダンがあった。フロントガラスは蜘蛛の巣じみて砕け散っていた。それは道路から飛び出し、近くの木に正面から衝突したように見える。運転席のドアは半開きだった。ナンバープレートこそ見えなかったものの、この車両はサイトにいた研究員のものであると、司令部が特定した。

The horn slowly gets weaker as Saunders approaches, dying out completely as she comes near. There is a subtle 'click' as Saunders releases the safety on her sidearm. She steps carefully, silently, around the open door, wheeling around it and bringing up her weapon in one fluid motion.

ソーンダースが近づくにつれて、クラクションは小さくなっていく。車のすぐそばまで来たところで、その音は消えてなくなった。彼女はサイドアームの安全装置を外す。カチリ、と音がした。開いたドアの影に身を寄せ、息を殺す。彼女は一瞬で身を翻すと、銃口を車内に向けた。

The vehicle is empty. Its airbag, deployed in the crash, rests partially-deflated. There is a smattering of blood stains present upon the driver's seat and steering wheel and spattered randomly across the upholstery. Saunders scans the area, checks under the vehicle, and only then holsters her weapon. She reaches into the center console, rummaging about to find a personnel lanyard. The coloration indicates it had belonged to a Level-3 researcher, but the surface is marred and scratched, with particular emphasis on the researcher's portrait. The text has been rendered illegible.

誰も、車内にはいなかった。事故で膨らんだのであろうエアバッグは、半ばしぼんだまま垂れ下がっている。ハンドルから運転席、それ以外の内装に至るまで、車内のあらゆる所に点々と血痕が散らばっている。ソーンダースは辺りを見回し、車の下も確認してから、ようやく銃をしまった。彼女はセンターコンソールに手を突っ込み、職員証を探し当てた。色からして、それはレベル三研究員のものだ。しかし、その表面は傷だらけで、特に顔写真の部分はひどく削られているように見える。文字などはもはや読めたものではない。

It is as Saunders moves to pocket this that she looks up at the shattered windshield. A bloodied handprint has been pressed against the interior side. It possesses four additional digits.

それをポケットに仕舞おうとした時、ソーンダースはふと視線をフロントガラスへやった。血塗られた手形が、内側から押し付けられている。それには指が9本あった。

Command advises Saunders to turn back, as it has become apparent that the situation may call for a properly-equipped Task Force. Saunders however cites her tenured field experience, claiming that if site staff are in danger, then she's obligated to lend her services. Command moves to notify Site-01 as Saunders rushes off down the road. A low fog begins to sweep the area.

もはや状況は然るべき装備を備えた機動部隊を要する段階にあると判断した司令部はソーンダースに撤退を勧告した。しかしソーンダースは、長年の実地経験を根拠に「サイト職員が危険に晒されている以上、助力は自らの義務である」とこれを一蹴する。彼女が道へと駆け出す中、司令部はサイト-01への連絡を開始した。彼女の足元に、霧が立ちこみつつある。

[[div class="scp-image-block block-center"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/footage1.webp]]
[[/div]]

The curvature of the road steepens the further Saunders travels, becoming stark to the point that it appears as if Saunders is running in a circle. The fog increases in intensity, obstructing visibility and causing Saunders to nearly trip over unseen roots criss-crossing the road. It is as Saunders comes around the next bend that the thicket of trees begin to recede. GPS indicates her arrival. Saunders comes about to face Site Romero-5.

進むほどに道の湾曲が強まるものだから、やがてソーンダースは、まるで同じところを堂々に巡っているかのような錯覚に陥った。霧が濃くなっていく。彼女は何かにつまづいた。道の至るところを這っている木の根だ。それにすら気づけぬほどに、視界は悪い。曲がり角を行くにつれて、生い茂る木々がまばらになってゆく。GPSの信号は、彼女が目的地に到着してい流ことを示していた。ソーンダースはサイト・ロメロ-5を見据えた。

The air here is thick with occluding fog. All that can be seen throughout the site grounds are mere silhouettes of buildings, the bright fluorescence of their interiors being the only visible sources of light in the murk. From the woods behind her, there comes a pained cervine bleating. Saunders ignores it as she steps past the chain-link perimeter fence.

深い霧の向こうから、建物の影ばかりがぼんやりと見えてくる。あたりは薄暗い。その窓から漏れてくる眩い明かりが、唯一の光源であった。ソーンダースの背後の森の中から、鹿の苦しげな鳴き声が聞こえる。彼女はそれを気にも留めず、金網のフェンスを乗り越えて、サイトの敷地内へと足を踏み入れた。

[[div class="scp-image-block block-center"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/romerofog.webp]]
[[/div]]

There is a low rumble that shakes the area, sending Saunders to the ground. Looking up, Saunders captures the silhouette of the nearest building -- its shape contorts and extends, jutting outward to the left of the frame, forming a branch that connects to a separate facility. Bright pinpricks open up along the length of this new addition, quickly widening and taking the shape of new windows. The earth continues to quake as buildings further off in the distance repeat this process.

低い地響きが走り、ソーンダースは地面に叩きつけられた。そのまま彼女は上を見た。すぐそばの建物が歪み、伸びていく。画面の左端からも飛び出たそれは、やがて別の施設と繋がる枝となる。枝に光の点がいくつも見えた。それはやがて大きくなり、新しい窓となる。遠くに見える建物もまた、同じように姿を変えていく。地鳴りはなお止まらない。

Just as suddenly as the shifts occur, they come to a standstill. Saunders shakily stands up. The complex before her, moments before a scattering of various facilities, seems to now be a single continuous complex. Command is able to verify this via satellite imagery: though somewhat obscured by increasing cloud cover, an overhead perspective of the site confirms that the buildings have indeed interlocked. They have taken on the shape of a spiral.

静寂が訪れた。始まった時と同じように、その変化は唐突に終わった。ソーンダースは震える足で立ち上がる。目の前には、一つの巨大な構造物があった。つい先ほどまでは、施設が点在していた場所であった。司令部も衛星画像で確認をとる。いくらか雲がかかってしまっているものの、そこにはひと繋がりになった建物が写っていた。それは、螺旋を象っていた。

Saunders finally admits that the current state of affairs is beyond her ability to personally resolve. Deciding that finding a capable off-road vehicle would be preferable to heading backwards on-foot, she convenes with Command to determine the approximate location of the site's vehicle bay. She sneaks off counter-clockwise around the site, sticking close to the perimeter fence. Dark shapes within the site cross in front of the windows, and Saunders doubles her pace.

もはや自分の手には負えない。ソーンダースはついに認めた。徒歩で引き返すより、オフロード車を探した方が賢明だと判断する。彼女は司令部と連絡をとり、車両格納庫の大まかな位置を確認した。フェンスに身を寄せながら、彼女は施設の外周を反時計回りに、慎重な足取りで進んでいく。窓の向こうを黒い影が横切った。彼女は歩を速める。

With assistance from Command, Saunders is directed to approach the contiguous structure. There is a large garage door on the face of the wall here. Saunders approaches the keypad beside the door, withdraws the lanyard she'd acquired and swipes it -- access is granted. The door begins to raise. Saunders swears loudly as its heavy, metallic rattling harshly breaks the silence of the site grounds. From somewhere out of frame there comes a deafening, protracted noise with the cadence of an air raid siren. It is distinctly human in origin; a blending of many voices that rise and fall in a cacophonous wail.

司令部の誘導に従いつつ、彼女は建物の一角にたどり着く。壁面には巨大なガレージドアがあった。その脇にあるキーパッドに、先ほど回収したIDカードをかざす。アクセスが許可された。ドアが上がり始める。重い金属の動く音が静寂を無慈悲に引き裂く。ソーンダースは悪態をついた。遠くから空襲警報じみた不快な音が響く。それは間違いなく人間の声だった。無数の声が混じった、不協和音の慟哭が辺りに満ちてゆく。

Saunders curses again, dipping below the door before it is fully opened. The interior of the vehicle bay is well-lit. Rows of personal vehicles line either side of the chamber. Saunders rushes past a vast majority of the fleet, composed of modern top-of-the-line models, towards an older-model Jeep near the back. Swinging into the cabin, Saunders reorients herself beneath the steering column to begin hotwiring it. The feed darkens as she works.

ソーンダースは再び悪態をついた。半開きのシャッターに、自身の体を滑り込ませる。車両格納庫は明るい。その両脇には、個人用車両がずらりと並んでいる。最新鋭の車には目もくれず、奥にあった旧式のジープへ駆ける。ソーンダースはその運転席に飛び乗った。ステアリングコラムの下で屈む。彼女は回線のショートを試みる。その作業の間、映像が暗転する。

The sound of her haggard breathing is drowned out by a shrill wail, closer than the first.

彼女の荒い息遣いを、甲高い叫び声がかき消した。先ほどよりも、近い。

The feed alights with a spark, and there is a rumbling of the engine. Saunders excitedly shouts, quickly rights herself, and shifts into drive. She peels out of the parking space just as the door at the end of the garage bursts open -- she does not turn to see what has entered.

暗い映像の中で、火花が散った。エンジンが唸り声を上げる。ソーンダースは喜びの声をあげながら、素早く体を起こし、ギアをドライブに入れる。ガレージの奥のドアが破られるのとほぼ同時に、彼女は駐車スペースから急発信した。何が入ってきたのだろうか。彼女にそれを確かめる余裕はない。

Saunders navigates out of the garage and into the fog-laden site grounds. Dark, roughly-humanoid shapes can barely be made out as she speeds through towards the entry gate. As she slows to align with the access road, the vehicle is struck from the side. Glancing over her shoulder, a human arm can be seen latched onto the back of the Jeep. A second arm rises above it. A third. Each reaches farther in turn, sprouting many clasping hands that find purchase and work to pull the entity aboard.

ガレージを抜け、霧に覆われた敷地へと飛び出す。新入ゲートへと向かって疾走する。その最中、霧の向こうでは人じみた名状し難い影がいくつも蠢いている。連絡道路に出るために速度を落としたその瞬間、車体が横からの衝撃を受ける。彼女は肩越しに後ろを確認した。ジープの後部に人間の腕が1本、喰らい付いている。その上から2本目、さらに3本目。腕から腕が生え、そこからまた腕が生える。無数の手が伸びては車体にしがみつき、その腕の主人を乗り込ませようと試みる。

Saunders turns her focus to the road ahead as she passes the perimeter fence, brandishing her sidearm and blindly firing three shots, which elicits an inhuman shriek. She steals a glance backwards -- the creature has been dislodged. She grunts with satisfaction, turning back ahead, only to find herself rapidly approaching a massive shape in the middle of the road. Headlights fall across a furred hide a half-second before she crashes at-speed into the beast.

ソーンダースは前方の道に意識を集中させた。境界のフェンスを通過する。そのさなか、彼女は前を向いたまま、腕を後ろに突き出して、サイドアームを後ろに向かって3発撃った。人ならざる金切り声が上がる。ちらと後ろを振り向く。異形は振り落とされていた。ソーンダースは安堵のため息を漏らした。前を向く。道を塞ぐ巨大な影がある。ヘッドライトが毛皮の塊を照らしたコンマ5秒後、彼女は猛スピードでその獣に衝突した。

Saunders is ejected from the vehicle, striking the ground and rolling several times before coming to a stop. From her position on the ground, the bulky frame of a deer becomes visible. It struggles to bring itself to a stand on six legs. A pair of heads, each encumbered by a complex tangle of antlers, rear back and weakly bleat before the beast collapses, dead. Command calls out to Saunders, shouting her name over the mic repeatedly, but she is unresponsive.

ジープから、ソーンダースが放り出される。そのまま彼女は地面に叩きつけられて、いくらか転がったあと、静止した。巨大な鹿の体が、彼女の視界を覆った。それはもがきながらも、6本の足で立ちあがろうとしている。複雑に絡み合った角を持つ、その二つの頭が点を仰ぎ、弱々しい鳴き声をあげた。その巨体は崩れ落ち、動かなくなった。息絶えたようだ。何度となく、司令部がマイク越しにソーンダースの名を呼ぶ。しかし、応答はない。

After a moment, there is movement. Saunders coughs. She groans, turning herself over to lie on her back. Looking down, a sharpened end of a bone now juts from her left leg. She screams as the bone can be seen to shift, splitting along its end, forking in two directions which themselves split and grow and fork. Her pained screams are drowned out by the wailing chorus of approaching figures. Saunders desperately looks about the area -- and spots the glint of her sidearm a few meters away.

ソーンダースの咳が、しばしの沈黙を破る。彼女はうめき声をあげ、仰向けとなった。視線を落とすと、左足から鋭く尖った骨が突き出しているのが見える。それが軋み、先端から二つにさけ、さらにその先が枝分かれしていく。ソーンダースは絶叫した。その悲鳴は近づいてくる者らの、合唱じみた慟哭にかき消されていく。ソーンダースは必死にあたりを見回す。数メートル先で、サイドアームが鈍く光っている。

She drags herself towards it as Command attempts to reassure her as to her survival, promising that help is on the way. Saunders calls their bluff, noting that there is no chance for salvation and calling for Command to rain hellfire on the site. The wailing grows closer, each voice in itself a dozen anguished cries. Saunders grabs her weapon, rights herself up against a nearby tree, and waits.

助けは向かっている、と司令部の励ましの声を背に、彼女は銃へと這っていく。それでくる助けなど気休めだ、と彼女は一蹴した。救いはない、と彼女は断じる。このサイトごと地獄の業火で焼き払ってしまえ、と彼女は叫んだ。幾重にも重なった慟哭が近づいてくる。その一つ一つすら、幾重にも重なった、苦痛にあえぐ叫びのように聞こえる。銃を掴んだソーンダースは、近くの木に寄りかかり、そして、待った。

Humanoid figures emerge from the fog on either side of the Jeep, cast in full silhouette against its headlights. Nothing more than their incomprehensible shapes can be made out -- torsos that split into multiple trunks, too-many arms extending from a single frame -- all converge on Saunders as she raises her weapon. She places two shots into the closest figure, dropping it. The third shot misses, taking out one of the Jeep's headlights. A rapid trio of shots strike yet another entity but does not halt its advance.

霧の中、ジープの両脇から影が現れる。ヘッドライトの逆光を受け、その輪郭だけが浮かび上がっていた。複数に分かれた胴体、それぞれの体から伸びる夥しい数の腕--　　--名状し難い実体が、銃を構えるソーンダースへと殺到する。彼女は最も近い実体に向けて2発撃ち、その動きを止めた。3発目は実体に命中することなく、ジープのヘッドライトを一つ割った。立て続けに3発、別の個体に命中する。しかし、その前進は止まらない。

Hazy outlines resolve into clear figures as they close in. The face of the nearest figure, draped in a labcoat, opens a maw encircled by many rows of overgrown teeth and lets out a wail. Its dozen hands point towards the camera, its fingers flowering with new digits, and there comes a final gunshot. The feed falls to the ground.

距離が詰まるにつれ、ぼやけた輪郭が明確な像となってゆく。白衣を纏ったすぐそばの実体の顔が裂ける。その口の中には、幾重もの歯列があった。叫び声が放たれる。無数の手がカメラに向けられた。指先から新しい指が、まるで花のように咲き乱れた。最後の1発が撃たれた。カメラが地面へと向けられる。

The remainder of the footage captures the ground as Saunder's body is dragged back towards the site.

残りの映像には、サイトへと引きずられてゆくソーンダースの体から、地面のみを映したものが記録されていた。

-----

[[/div]]

Emergency containment procedures would quickly be established following the receipt of this footage.

緊急収容プロトコルは、この映像を受信したのち、速やかに策定されました。

Initial attempts at an aerial assault on the facility were thwarted by hostile lifeforms, leading to the loss of twelve members of Nu-7. As containment teams scrambled to establish the Exclusion Zone and Forward Operating Base, Agent Lament would be sent by O5-8 to recruit Dr. Langford: a former researcher at Site Romero-5 and co-architect of SCP-9001.

当該施設への航空攻撃は、敵性生命体の妨害により失敗に終わり、結果として機動部隊ニュー-7の隊員12名が殉職しました。収容チームによる領域封鎖および前線基地の設営が急がれる一方、O5-8は、サイト・ロメロ-5の元研究員にしてSCP-9001の共同設計者でもある、ラングフォード博士の身柄を確保するために、ラメント司令官を派遣しました。

[[div class="blockquote"]]

**映像記録9001-1**

**関係者:**
* ロバート・ラングフォード上級研究員(機動部隊エータ-10顧問、MEDUSA計画顧問、サイト-15所属)
* エージェント・トロイ・ラメント(統合任務部隊パンロケ総司令官、前線基地パンロケ所属)

**はしがき:** SCP-9001-A収容の試みに関する、ラングフォード博士に向けたブリーフィング。

**<記録開始>**

//Commander Lament consults the seating chart on his tablet, looking for Dr. Langford's desk on the open floor plan. Dr. Langford is standing beside his standing desk, wearing a t-shirt, shorts, and a pair of headphones. Approaching from behind, Dr. Langford can be seen typing Python Tensorflow code into a Sublime editor. Commander Lament calls out to him, then taps his shoulder. Dr. Langford turns around and takes off his headphones.//

タブレットに表示されている座席表を見ながら、ラメント司令官は、目的の人物を探した。広々としたオフィスフロアの片隅、スタンディングデスクの傍に、ラングフォード博士はいた。彼はTシャツに短パンというラフな格好で、ヘッドフォンをつけている。背後から近づくにつれて、彼がSublimeエディタにPythonのTensorFlowコードを打ち込んでいることがわかる。ラメントは声をかけ、その肩を叩いた。ラングフォード博士は振り返り、ヘッドフォンを外した。

**Dr. Langford:** Ah, my apologies. Can I help you?

**ラングフォード博士:** おや、失礼。何かご用がおありで？

//Commander Lament extends his hand.//

ラメント司令官が手を差し出す。

**Cmdr. Lament:** Troy Lament. Containment and Recovery Specialist.

**ラメント司令官:** トロイ・ラメントだ。収容および復興スペシャリストの。

//Dr. Langford accepts. There is an awkward beat of silence as Lament awaits his response.//

ラングフォード博士は握手に応じる。ラメントは彼の返事を待った。奇妙な静けさが、二人の間を流れる。

**Cmdr. Lament:** ...and you're Robert Langford?

**ラメント司令官:** そして君が……ロバート・ラングフォード？

**Dr. Langford:** Right, yes. Sorry. Can I ask what this is about?

**ラングフォード博士:** ええ、はい。これは失敬。それで、これはどういうことなんです？

//Dr. Langford gestures towards a nearby bright green couch.//

ラングフォードは、脇に置いてある黄緑色のカウチを指し示した。

**Dr. Langford:** Please, take a seat.

**ラングフォード博士:** さあ、お座りになって。

//Commander Lament shakes his head. He remains standing.//

ラメント司令官は首を振る。彼は立ったままだ。

**Cmdr. Lament:** I understand you mostly help Eta-10 these days?

**ラメント司令官:** 最近は、イータ-10の補助に回っているようだな？

**Dr. Langford:** That's right.

**ラングフォード博士:** ええ。

**Cmdr. Lament:** And before that you were a Senior Researcher for Project HYDRA at Site Romero-5, correct?

**ラメント司令官:** それ以前は、サイト・ロメロ-5でHYDRA計画の上級研究員をやっていた。そうだな？

//Dr. Langford stops smiling.//

ラングフォード博士の表情から、笑みが消える。

**Dr. Langford:** That's… correct. That prior experience is why I'm now attached to Eta-10 and MEDUSA.

**ラングフォード博士:** ええ……そうです。その経験があったからこそ、ぼくはイータ-10とMEDUSAのお付きになったわけですが。

**Cmdr. Lament:** You have combat training?

**ラメント司令官:** 戦闘訓練を受けたことは？

**Dr. Langford:** Excuse me?

**ラングフォード博士:** 戦闘訓練？

**Cmdr. Lament:** You consult for a Mobile Task Force, don't you.

**ラメント司令官:** 機動部隊の顧問をやっているから、もしかしたらと思ってね。

**Dr. Langford:** You're right… although truth be told, I could probably use a few more laps around the track or pool we have around here.

**ラングフォード博士:** ええまあ、その通りですが………打ち明けた話、この辺のランニングトラックとか、プールとかを何周かするのが関の山ですよ。

**Cmdr. Lament:** Excellent. That'll do.

**ラメント博士:** 素晴らしい。それで十分だ。

**Dr. Langford:** Do for… what exactly did you want to discuss, Mr. Lament?

**ラングフォード博士:** 十分って……何に対して十分なんです？　ラメントさん。

**Cmdr. Lament:** Perhaps showing is better than telling.

**ラメント司令官:** ご覧いただいた方が、話すよりも速かろう。

//Commander Lament hands his tablet to Dr. Langford. A video-player fills the screen.//

ラメント司令官は、タブレットをラングフォード博士に手渡した。画面にビデオプレイヤーが映っている。

**Cmdr. Lament:** Play it.

**ラメント司令官:** 再生してくれ。

//[The video is filmed from the perspective of a helicopter flying through the night sky  -- several more are seen in the distance ahead. The sounds of shouting passengers are drowned out by the heavy thumping of rotors.]//

[映像は夜空を飛ぶヘリコプターの視点から撮影されている。前方遠くにさらに数機飛んでいる。乗員たちが何かを叫ぶが、それはローターの重い音によってかき消されてしまう。]

//[Scanning the wooded expanse below, little can be made out as the region is mired in fog. As the perspective tilts, it comes into view -- buildings atop buildings, a veritable skyscraper whose floors are a confusing knot of interlocking facilities haphazardly growing from one another. A second helicopter circles around the side of the tower; its side-mounted machine gun fires at obscure figures crawling out from its windows.]//

[眼下に広がる森林は霧に覆われている。そのせいで見通しはほとんど効かない。映像が傾く。建物の上の建物。無秩序に成長し、連結した施設の不可解な結び目。それらの積み重なった、まごうことなき摩天楼が現れる。2機めのヘリコプターが塔の側面を旋回する。窓から這い出る不明瞭な影に向かって、その側面の機銃が発砲される。]

//[A third helicopter speeds by -- as it descends near the tower, its tailboom fractures into two. Its rotors suddenly multiply, splitting from five into ten and then into an indistinct mass of metal, and it goes down; crashing into the side of the tower. Numerous crawling figures on the tower leap off the sides like fleas and take to the air, swarming around the tower and heading towards the viewpoint.]//

[3機目のヘリコプターが高速で通りすぎ、塔の近くで降下する。そのテールブームが2つに割れた。ローターの羽は突如増殖する--　　--5枚から10枚へ、名状し難い金属の塊へ分裂する。制御を失ったそのヘリコプターは、塔の外壁へ衝突した。そこを多くの影が這っていた。それらはノミめいて飛び、空中に舞い上がる。塔の周りで群れをなしたそれらは、カメラの方へと殺到する。]

//[The perspective helicopter pulls back as the figures near, carried on the wind by reams of webbed skin that stretch between numerous arms. Four are downed by suppressive fire. A fifth flits about, avoiding the barrage and crashing into the windshield. Many lolling tongues extend from its throat, tearing into the cockpit.]//

[視点のヘリコプターが後退する。影が近づいてくる。それらは、いくつもの腕の間に広がる、水かきじみた膜で風に乗り、飛んでいるようであった。4体、制圧射撃によって撃墜される。だが5体目は弾幕を避けながらひらひらと飛び、フロントガラスに衝突した。その喉から垂れ下がる何本もの舌が伸び、コクピットを破壊した。]

//[The feed spins as the vessel goes down, cutting the transmission upon contact with the ground]//

[機体が墜落する。映像が回転する。地面と接触する。映像が途絶える。]

//Dr. Langford rolls away his chair, staring at the table.//

ラングフォード博士は椅子を回転させ、テーブルを見つめた。

**Dr. Langford:** That... that can't be real.

**ラングフォード博士:** 本当に……こんなことが？

**Cmdr. Lament:** Math wasn't my best subject, but I believe your site's coghaz's focused on fractals. And those freaky shapes we're observing are fractals. It's not a stretch. And it's //spreading//.

**ラメント司令官:** フラクタルが、君のところの認識災害の大元だ。数学は得意じゃなかったが、わたしにもわかるよ。あの動画に出てきた、気色悪いあれもフラクタルだ。しかもタチの悪いことに、ただ拡大してるわけじゃなく、感染を広げている。

**Dr. Langford:** What about Dr…

**ラングフォード博士:** あの、ベリーマ--　　--

//Dr. Langford buries his face in his hands, then curls the latter into fists. After a while, he looks up at Commander Lament.//

ラングフォード博士は、自身の顔を両手で覆った。そのまま彼は両手を握りしめる。しばらくしてから、ラングフォード博士はラメント司令官を見上げた。

**Dr. Langford:** I can understand why you came to me. I am willing to lend my expertise for the sake of the Foundation. But I must confess, this is a difficult subject for me.

**ラングフォード博士:** こうしてぼくのところに来られたわけが、わかりました。財団のためならば、喜んで力をお貸ししましょう。ですが白状すると、やはりなかなか辛いものがあります。

//Commander Lament nods.//

ラメント司令官が頷く。

**Cmdr. Lament:** I'm sorry to hear that.

**ラメント司令官:** お気持ちはお察しする。

**Dr. Langford:** Yeah… lots of memories. Not particularly… good ones either.

**ラングフォード博士:** ええ……思い出は、色々と。あまりいいものでもないですが。

//Dr. Langford bunches his fists again and looks at an empty chair, as if looking at someone absent. He frowns, then exhales. A few seconds pass.//

ラングフォード博士はふたたび両手の指を組み、空いている椅子を見た。ここにいるはずのない誰かを探しているかのようだった。彼は顔を顰めて、ため息をついた。数秒が過ぎる。

**Cmdr. Lament:** I mean, I'm sorry to hear that, because you'll be deploying to Site Romero-5 with a squad from my Joint Task Force.

**ラメント司令官:** 君はこれから、わたしの統合任務部隊とともに、サイト・ロメロ-5に対して配備される。本当に、お気持ちはお察しするよ。

//Dr. Langford's shoulders slacken.//

ラングフォードの肩が落ちた。

**Dr. Langford:** Um, come again?

**ラングフォード博士:** ええと、なんですって？

**Cmdr. Lament:** You will be deploying to Site Romero-5 with a squad from--

**ラメント司令官:** 君はこれから、わたしの統合任務部隊とともに、サイト・ロメロ-5--　　--

**Dr. Langford:** Absolutely not.

**ラングフォード博士:** お断りします。

**Cmdr. Lament:** Perhaps I was unclear. I am ordering you to deploy to--

**ラメント司令官:** お分かりでないか？　これは命令だ。サイト・ロメロ-5へ--　　--

**Dr. Langford:** I don't care.

**ラングフォード博士:** そんなこと。

**Cmdr. Lament:** You don't get to say 'no'. This is coming from the top. O5-8 wants you, specifically.

**ラメント司令官:** 君に拒否する権限はない。上からの命令だ。O5-8が君を指名している。

//Dr. Langford takes a deep breath.//

ラングフォードが深く呼吸をする。

**Dr. Langford:** I know full well the consequences of saying this, but whatever you do to me, you can't make me do it.

**ラングフォード博士:** やりませんよ。ぼくは。あなたがぼくに何しようが、ぼくはやりません。きっと何か沙汰が下るでしょうが、だとしてもです。

**Cmdr. Lament:** You will be taken and deployed on this mission regardless of your opinion, but it will make it a lot easier for everyone involved if you go willingly rather than forcibly dragged. Restrained if needed.

**ラメント司令官:** 君はこの任務に出るのだ。君の意見でどうこうなる話ではない。だが、強制的に連れて行かれるよりも、君が志願してくれた方が関係者全員の士気は上がるだろう。必要ならば、拘束させてもらうがね。

**Dr. Langford:** You don't understand what I witnessed at that Site. What we had to...

**ラングフォード博士:** お分かりなんです？　ぼくがあそこで何を見て、何をしなければ--　　--

//Dr. Langford falls silent, although he starts to shake.//

ラングフォード博士は黙った。そして、震え始めた。

**Cmdr. Lament:** You're right, I don't understand, and that's the thing. That site has gone radio silent for years except for scheduled package delivery. We have no idea what Dr. Berryman is up to, and now we see //this//.

**ラメント司令官:** その通りだ。わたしはわからない。それこそが問題なのだよ。定期的な物資配送を除けば、あのサイトと通信が途絶えてから数年だ。ベリーマン博士が本当は何をやっているのか、我々にもわからない。そんな時に、あの動画を見せられたものだからね。

//Commander Lament gestures at the tablet.//

ラメント司令官がタブレットを示した。

**Dr. Langford:** Wait… you've had no idea what she's doing, for years?

**ラングフォード博士:** つまり……ベリーマン博士の動向を、あなた方もご存知ない？

**Cmdr. Lament:** Exactly.

**ラメント司令官:** その通りだ。

//Dr. Langford sighs.//

ラングフォード博士がため息をつく。

**Cmdr. Lament:** But you, you worked at that specific site, on that specific project, for over a decade.

**ラメント司令官:** だが君は違う。君はあそこで、あのプロジェクトのために、10年以上働いてきた。

**Dr. Langford:** Look, I get that I worked at the site, but I haven't been there in over six years. I am just as in the dark as you all are. You have more up-to-date maps of the sites and more up-to-date project research notes.

**ラングフォード博士:** 確かにそうです。ぼくはあそこで働いてきました。ですがこの6年、ロメロ-5には行ってません。あなた方と同じで、ぼくも何も知らないんです。サイトの最新の地図とか、最新の研究動向については、あなた方のほうがお詳しいでしょう。

**Cmdr. Lament:** But you know //more// than anyone else.

**ラメント司令官:** でも、君ははるかに多くを知っている。

**Dr. Langford:** I'm not the only memeticist at the Foundation, I'm not even close to the best. I've field experience, sure, but I surely wouldn't be of use in--

**ラングフォード博士:** ぼくの他にもミーム学者はいます。それにぼくはとりわけ優秀なほうでもありません。確かに実務経験はありますが、そんなの何の役にも--　　--

**Cmdr. Lament:** How did Dr. Berryman like her coffee?

**ラメント司令官:** ベリーマン博士は、コーヒーをどう飲む？

**Dr. Langford:** Excuse me? I fail to see how that's releva--

**ラングフォード博士:** 失礼ですが、そのご質問は何の関係が--　　--

**Cmdr. Lament:** Answer the damn question.

**ラメント司令官:** 御託はいい。答えろ。

**Dr. Langford:** A single piece of broken-up Cadbury chocolate melted in, and half a creamer pod since the chocolate already had some milk.

**ラングフォード博士:** キャドバリー・チョコを一つ溶かし入れて、コーヒーフレッシュを半分だけ。チョコにミルクは含まれてますから。

**Cmdr. Lament:** Favorite novel?

**ラメント司令官:** 彼女の好きな小説は？

**Dr. Langford:** Snow Crash by Neal Stephenson.

**ラングフォード博士:** ニール・ステフェンソンの『スノウ・クラッシュ』。

**Cmdr. Lament:** Hobbies?

**ラメント司令官:** 趣味は？

**Dr. Langford:** Caring for weird-looking flowers and succulents.

**ラングフォード博士:** 変な形の花とか、多肉植物とかの世話です。

**Cmdr. Lament:** The truth is, Dr. Langford, the Foundation may have other memeticists, but its only expert on Dr. Berryman is you. And given how far the situation has progressed, we’re sure as hell going to need that.

**ラメント司令官:** そういうことだ。ラングフォード博士。確かに財団のミーム学者は君だけではない。だが、ベリーマン博士の専門家は君だけだ。状況はすでにかなり悪い。だから、君がどうしても必要なのだ。

//Dr. Langford stares at the floor for twenty seconds. He sighs, then speaks up in a whisper.//

およそ20秒の間、ラングフォード博士は床を見つめた。彼はため息をついて、消え入るような声で話しはじめる。

**Dr. Langford:** … When do I deploy?

**ラングフォード博士:** ……いつ、向かうのです？

**Cmdr. Lament:** We're oscar mike oh-nine-thirty hours tomorrow, Dr. Langford. Pack your bags.

**ラメント司令官:** 明朝0930に移動開始だ。ラングフォード博士、荷物をまとめてくれ。

**<記録終了>**
[[/div]]

Upon his arrival at FOB Panloque, Dr. Langford would be outfitted and deployed alongside the JTF. It was decided the team would utilize Site Romero-5's subterranean tram access in order to bypass above-ground hostiles. Their mission would consist of three discrete objectives:
# Find and extract the core of SCP-9001 from the production center.
# Determine the locus of the SCP-9001-A phenomenon and destroy it, if possible.
# Apprehend or terminate suspected rogue agent: Dr. Ava Berryman

ラングフォード博士は、前線基地パンロケに到着ののち、装備を支給され、統合任務部隊とともに出動することとなりました。本部隊は、敵性実体のいる地上を迂回するため、サイト・ロメロ-5の地下鉄道を利用し、サイトにアクセスすることが決定されました。また、本チームは、以下の3つを目的として、展開されます。

# 生産センターからSCP-9001のコアを発見し、抽出する。
# SCP-9001-A現象の発生源を特定し、可能であればそれを破壊する
# 離反したと疑われる職員、エイヴァ・ベリーマン博士を捕縛、または終了する

[[div class="explo-root"]]
[[div class="explo explo--room"]]
[[=]]
+ 探査ログ
[[/=]]

||~ Subject || SCP-9001-A ||
||~ Team Lead || Benton Torres, Captain, MTF Epsilon-11 ||

||~ 対象 || SCP-9001-A ||
||~ チームリーダー || ベントン・トレス隊長、機動部隊イプシロン-11所属 ||

||~ Team Members ||
|| **Warren Gooden**, Technician, MTF Zeta-9 ||
|| **Sebastian Gooden**, Rifleman, MTF Zeta-9 ||
|| **Typhlo**, Deprivate[[footnote]]Operatives who have undergone invasive neurosurgical procedures to prohibit their ability to see, hear, taste, and smell. Augmented mechanoreceptors allow Deprivates an alternative means of perception by way of acute awareness of vibrations.[[/footnote]], MTF Eta-10 ||
|| **Special Operative Nix**, Navigator, MTF Theta-90 ||
|| **Dr. Robert Langford**, Negotiator ||

||~ チームメンバー ||
|| **ウォーレン・グッデン**、技術者、機動部隊ゼータ-9所属 ||
|| **セバスチャン・グッデン**、小銃手、機動部隊ゼータ-9所属 ||
|| **ティフロ**、奪感者[[footnote]]侵襲的神経外科処置により、視覚、聴覚、味覚、嗅覚を剥奪された工作員。奪感者は、機械的拡張感覚器により、振動に対する鋭敏な感覚を獲得し、通常と異なる方法で外界を認識することができる。[[/footnote]]、 機動部隊エータ-10 ||
|| **特殊工作員ニクス**、案内員、機動部隊シータ-90 ||
|| **ロバート・ラングフォード博士**、交渉人 ||

||~ Equipment ||
|| 4 standard-issue M27 Infantry Automatic Rifles and additional magazines _
6 M45A1 Close Quarter Battle Pistols and additional magazines _
5 compact Martel Pitons[[footnote]]Experimental technology developed by researchers in the wake of the [[[SCP-1730]]] incident. Allows for point-to-point instant transportation of personnel between emplaced Pitons in areas where spatial shifts might otherwise inhibit extraction.[[/footnote]] _
//Nix:// M38 Designated Marksman Rifle and additional magazines _
//Nix:// Prismatic compass _
//Warren:// Portable Scranton Reality Anchor _
//Sebastian:// 24" machete _
//Torres:// Quantum Entangled Relay Device, tethered to H.E.C.O.R.[[footnote]](High Energy Concentration Orbital Railgun)[[/footnote]] ||

||~ 装備 ||
|| M27歩兵用自動小銃4丁および予備マガジン _
M45A1自動けん銃6丁および予備マガジン _
マーテル型ペグ[[footnote]][[[SCP-1730]]]事件を受けて開発された、実験的技術。空間変異により、通常の手順では脱出が困難となる状況下において、設置されたペグを中継点とすることで、人員の二点間即時転送を可能にする装備。[[/footnote]] _
//ニクス:// M38選抜射手用小銃および予備マガジン _
//ニクス:// プリズムコンパス _
//ウォーレン:// 携帯用スクラントン現実錨 _
//セバスチャン:// 24インチのマチェット _
//トーレス:// 量子もつれリレーデバイス。H.E.C.O.R.[[footnote]](High Energy Concentration Orbital Railgun: 高エネルギー集中型軌道電磁砲)[[/footnote]]に接続されている。 ||

-----

[[=]]
++ [記録開始]
[[/=]]

//The squad is traveling down a darkened flight of stairs through a concrete shaft. The door at its terminus opens into a dark, cavernous area. Automatic lights flicker on as they enter, revealing that they've entered a simple metro bored into the earth. Across from the entrance, a railway is set within a deep depression that trails off into the tunnel beyond. Within the station, shallow cracks run up the facade, support pillars, and across the ceiling, but otherwise the integrity of the chamber is holding up against topological restructuring.//

部隊はコンクリート製のシャフトを通り、暗い階段を下っていく。突き当たりにあるドアを抜ければ、まるで洞窟のような巨大な空間が現れた。自動照明が明滅している中、一行はそこに足を踏み入れる。地中をくり抜いて作られた、簡素な地下鉄の駅だ。入り口の向かいには線路があった。プラットホームは、線路よりもやや高い位置にある。その線路は、奥のトンネルへと続いている。駅構内の壁面や支柱、天井には浅い亀裂が入っている。だが、位相的再構築の影響を受けながらも、空間全体の構造は維持されているようだ。

//Lights along the tracks within the tunnel do not engage, leaving the tunnel itself mired in darkness. The tram is not currently present.//

トンネル内の照明は点灯せず、その奥は暗闇に包まれている。トラムの姿も見当たらない。

//The brothers, Warren and Sebastian, jog alongside the tracks towards a control booth on the far end of the chamber. Warren fiddles with the door fruitlessly until Sebastian pushes him aside.//

グッデン兄弟が線路脇を走って、ホームの奥にある制御室へと向かう。兄のウォーレンがドアをこじ開けようと悪戦苦闘するが、埒が開かない。やがて痺れを切らしたセバスチャンが、ウォーレンを突き飛ばした。

**Typhlo:** {{Echo mic check.}}

**ティフロ:** {{えこー、まいくちぇっく}}

**Torres:** What? I didn't even-- ugh. We're live, folks. Check your mics.

**トレス:** 何？　俺はまだ--　　--まあいい。お前ら生きてるな。マイクチェックしとけ。

**Warren:** Check.

**ウォーレン:** チェック。

**Nix:** Check, and cool it with the parlour tricks, Typh.

**ニクス:** チェック。ティフロ、そのお座敷芸も大概にしてもらえる？

//Warren steps aside as Sebastian shoulders full-force into the door, forcing it open.//

ウォーレンが身を引く。セバスチャンはドアに渾身の力で体当たりし、強引に押し開けた。

**Sebastian:** Woo! That's a check!

**セバスチャン:** しゃあっ！　チェック！

**Dr. Langford:** Uhm... check.

**ラングフォード博士:** あー……、チェック。

//Sebastian and team fan about the chamber while Warren enters the control booth.//

ウォーレンが制御室に入っていく一方、セバスチャンと他の隊員たちは構内に散開し、警戒態勢に入った。

**Torres:** Right. All golden. Warren, what've we got?

**トレス:** よし。全員OKだな。ウォーレン、どうにかできるか？

**Warren:** Looks like everything's still up and running. Tram's halted mid-way down the line. Last use was... about a month ago, according to the logs here. Looks like daily use up to that point, besides.

**ウォーレン:** 一応どれも動いてはいそうです。トラムが線路の途中で止まってて……最後に使われたのが先月。ここのログにそう書いてます。それまでは、日常的に使われていた、と。

**Dr. Langford:** Should have been for the Director's use only, and Berryman isn't the sharing type.

**ラングフォード博士:** どうにも管理官専門のトラムに思えます。ベリーマン博士が、これを誰かと共有していたとも思えません。

**Typhlo:** {{Mutiny?}}

**ティフロ:** {{叛乱カ？}}

**Dr. Langford:** Against Berryman? I don't think so. The woman could //smell// insubordination. No, if they were using this thing it was on her orders.

**ラングフォード博士:** ベリーマンに対してですか？　それはないでしょうね。反抗の気配を嗅ぎ取れるのですよ。あの人は。つまり誰かがこのトラムを使っていたとしたら、それは彼女の命令です。

**Sebastian:** Shit. Add that to the laundry list of questions for the doc'. //(louder)// Is the tram live or are we hoofin' it, Wally?

**セバスチャン:** こりゃ博士サマにお目通りしたら質問攻めにしなきゃいかんなあ。(大声で)なあウォーリーくんよ、トラム動いてんの？　それとも俺たちこっからお散歩？

//There is a loud, electronic *ding*, and a distant sound of mechanical whirring.//

ジリン、と大きな電子音が鳴った。遠くから機械の唸りが聞こえる。

**Warren:** For the latter half of the trip, maybe. Have to wait and see what was holding it up. For now though, it's headed in our direction.

**ウォーレン:** しばらくはトラムで良さそうだよ。少なくともこっちには向かってきてる。でも、なんで途中で止まってたのかは確かめなくちゃ。そこからは、お散歩かな。

**Torres:** Good work. Typhlo, can you get a read on our transport? I need you to check for occupants.

**トレス:** よくやった。ティフロ、トラムの様子はわかるか？　乗客が居るかどうかを調べてほしい。

//Typhlo drops onto the tracks, kneeling down to place a hand upon the rail.//

ティフロが線路に降りる。そして膝をつき、手を線路の上に乗せた。

**Typhlo:** {{Approaching at a rate of eighty kilometers per-hour. Arrival expected in two minutes. No movement on-board.}}

**ティフロ:** {{時速80きろめーとるデ接近中。オヨソ2分後ニ到着。車内ニ動体反応ナシ。}}

**Dr. Langford:** Are we to expect a lot of resistance?

**ラングフォード博士:** 多少の諍いは、覚悟しておくべきでしょうか。

//Warren rejoins the squad, offering a hand to Typhlo, and helps her up from the tracks. Nix, kneeling across the chamber, places down a Martel Piton. The flat device quietly hums as four small rods eject from its sides and anchor to the ground.//

ウォーレンが再合流する。彼はティフロに手を差し伸べて、線路から引き上げた。一方、構内の反対側ではニクスが膝をつき、マーテル型ペグを設置していた。扁平な装置が静かに震える。小さな杭が4本、その側面から飛び出て、地面へと食い込む。

**Nix:** Depends. Since we made first contact, there's been a lot of those creatures escaping out into the surrounding area -- Hammer Down has had its hands full.

**ニクス:** さあね。最初の接触以来、あの怪物どもは何体も周辺地域に逃げ出しているわ。"鉄槌"の連中が、対処しているようだけれど。

**Sebastian:** Makes ya wonder why we didn't pick up on this place sooner. S' like they went ape-shit the second their cover was blown.

**セバスチャン:** こいつらどうしてずっと隠れてられたんだろうなあ。俺たちがここ見つけた瞬間に、奴らプッツンときたみてえじゃねえか。

**Torres:** All of this is to say, we simply don't know. Ghost town, if we're lucky.

**トレス:** つまりな、俺たちもわからんのだ。運が良ければ、ただのゴーストタウンかもしれん。

**Dr. Langford:** And if we're not?

**ラングフォード博士:** 運が悪かったら？

//Dr. Langford stares into the darkness of the tunnel.//

ラングフォード博士は、トンネルの暗闇を見つめた。

**Typhlo:** {{Simple. There will be bloodshed.}}

**ティフロ:** {{簡単ダ。流血ガアル}}

//After a moment, lights become visible in the tunnel. The tram speeds towards the platform, slowing down and coming to rest before the team. The doors open, and the squad carefully enters with weapons at the ready. Warren makes for the controls.//

しばらくすると、トンネルの奥に明かりが見えてきた。トラムが高速で近づいてきているのだ。それはやがて減速し、部隊の目の前で静かに停止した。ドアが開く。隊員は銃を構えたまま、慎重に車内へ足を踏み入れた。ウォーレンは操縦席へと向かう。

**Torres:** Watch our speed, Warren. Last thing we need is for this to end up in training footage.

**トレス:** 速度には気をつけろよ、ウォーレン。訓練映像行きはごめんだ。

//The doors click shut, and the tram begins to move forward. A mechanical whirring persists throughout this portion of the video.//

ドアが閉まる。トラムが前進を始める。映像のこの部分には、機械の唸る音が含まれている。

**Warren:** ... Again.

**ウォーレン:** ……二度と、な。

**Dr. Langford:** Again?

**ラングフォード博士:** 二度と？

//Sebastian laughs, taking a seat by the door.//

ドア横の座席に座っているセバスチャンが、笑った。

**Sebastian:** Oh, our Wally here is a star! "So You've Entered a Non-Euclidean Zone" -- you know, **that** scene?

**セバスチャン:** こちらのウォーリーどのは名優であるぞ！　「さて、非ユークリッド空間に入ったわけだけど」ってシーン、みんな知ってるだろ？

**Nix:** No way.

**ニクス:** 本当に？

**Torres:** That was him?

**トレス:** 彼がそれを？

//Warren rubs his left shoulder.//

ウォーレンが、自身の左肩を撫でた。

**Warren:** Bone never did set right.

**ウォーレン:** 古傷が痛むね。

//Typhlo suppresses a snicker. Dr. Langford halfheartedly forces an awkward chuckle.//

ティフロが鼻で笑った。居心地を悪く感じたのか、ラングフォード博士はやや引き攣った笑みを浮かべた。

//The team waits in silence as the tram progresses. Intermittent fields of static momentarily interrupt the feed, but the connection remains sound. After a few minutes, Typhlo signals for Warren to stop, who acquiesces.//

全員が黙ったまま、トラムの進行を待つ。ときどき映像にノイズが走るが、通信は途切れない。数分が経つ頃、ティフロがウォーレンに合図を送った。ウォーレンはトラムを停止させる。

**Typhlo:** {{Obstruction ahead. We walk from here.}}

**ティフロ:** {{前方ニ障害物アリ。ココカラハ歩ク。}}

//The doors slide open, and a light fog drifts into the compartment.//

ドアが開く。薄い霧が車内へと入ってくる。

**Torres:** Unusual.

**トレス:** 奇妙だな。

**Sebastian:** Think it's toxic?

**セバスチャン:** 吸ったらヤバいか？

**Warren:** I could take off my mask and get a big whiff. Y'know. For science.

**ウォーレン:** マスクを取って深呼吸してみようか？　ほら、科学のためだ。

//Nix takes a knee, wafting her fingers through the fog.//

ニクスが膝をつく。彼女は指を霧の中であそばせた。

**Nix:** Just like in Saunders' footage. I thought it was just a meteorological effect.

**ニクス:** ソーンダースの映像にもあったわね。普通の霧だとは思ったのだけれど。

**Dr. Langford:** It likely is. The anomaly seems to be restructuring everything into fractal patterns. Could very well be that it is condensing and organizing water vapor in the same manner.

**ラングフォード博士:** おそらくはそうでしょう。ここの異常性は、全てをフラクタルに再構築しようとするものです。その流れで、水蒸気も同じように凝集されて、整列させられていると考えてもおかしくはありません。

**Torres:** Probably not something we want in our lungs regardless. Let's get moving.

**トーレス:** どっちにしろ、喜んで吸いたくはないな。先を急ごうか？

//The squad leaps out onto the tracks, navigating to the front of the tram, and begins walking. Through the low-laying mist, it becomes apparent that the rail ahead has been rent and twisted by the emergence of large tangles of tree roots, growing from all about the tunnel floor, walls, and ceiling. The sound of wooden creaking becomes audible. As the team moves between the roots, the ends of the nearest can be seen to gradually split and grow. There is little chatter as they travel the last few kilometers. Light is seen in the distance.//

部隊は線路へ飛び降り、トラムを放って前へと進んでいく。トンネルの壁を、天井を、そして床を割り、至るところから巨大な木の根が伸びている。低く立ち込める霧の中でも、前方の線路が歪んでいることはわかる。線路もその木の根に押され、捻じ曲がっている。どこかで木が軋んでいる。根の間を縫うように進む部隊の眼前、すぐそばの根の終端がゆっくりと裂け、枝分かれし、成長していく。残りの数キロを進む間、誰も口を開かない。やがて、遠くに光が見えてくる。

//The team exits the tunnel, emerging into the Romero-side metro cavern, identical to its counterpart on the other side of the tunnel save for more prominent wear on the facade and chamber walls. One by one, the team clambers up off the tracks and onto the platform. The fog here is heavier, permeating the air through to the ceiling, but is not thick enough to fully occlude sight. They cross the chamber towards a flight of stairs leading up.//

部隊はトンネルを抜け、ロメロ側の地下鉄駅へと出た。構造こそ来た時に通った駅と同じだが、壁面や柱の劣化はこちらの方がひどい。隊員たちは次々と線路からホームへと這い上がる。霧はこちらの方が濃く、天井まで立ち込めているが、視界を完全に遮るほどではない。一行は構内を横切り、上階へと続く階段に向かった。

**Dr. Langford:** We should be able to directly access the Director's office from here.

**ラングフォード博士:** ここから直接、管理官のオフィスへと出られるはずです。

**Warren:** Directly? Isn't that a little weird?

**ウォーレン:** 直接？　そりゃちょっと変じゃないかい？

**Torres:** Not if you're both paranoid and also very important. Not out of the ordinary for Directors to have emergency escape routes.

**トレス:** もしそいつが心配性のVIPならば、考えうる話だ。一人の管理官が、専用の緊急避難路を確保している--　　--これは、奇妙でもなんでもない。

**Dr. Langford:** Elevator just outside her quarters should get us access to most of the site. The FCI production facility was Sublevel 2, so not much of a jaunt should the elevators be down. Ah, here we are.

**ラングフォード博士:** エレベーターが、ベリーマン博士のオフィスのすぐ近くにあります。それで行きたいところには大体行けるはずです。エレベーターが動かなくても、FCI生産施設は地下2階ですから、大した登山にはなりませんよ。お、来てくれましたね。

//A set of large double doors bars entry -- Nix and Sebastian, ahead of the team, step aside for Torres to come through.//

巨大な両開きの扉が、侵入を阻んでいる。先行していたニクスとセバスチャンが両脇に退き、トレスが前に出る。

**Nix:** Compass is going wild. Be ready.

**ニクス:** コンパスがおかしいわ。準備を。

//Torres swipes a keycard with Level-5 access. The doors open silently, and a dense cloud of fog emerges from within. It subsides after a moment, allowing the squad to see within. Sebastian whistles loudly. Dr. Langford gasps. Nix trains her rifle ahead.//

トレスがレベル-5のキーカードを読み込ませれば、扉が静かに開いていく。中から濃霧が漏れ出た。それが薄まっていくにつれて、中の様子が確認できるようになる。セバスチャンが口笛を吹いた。ラングフォードがえずいた。ニクスはライフルを向けた。

**Torres:** What in God's name...

**トレス:** なんと……これは……

[[div class="explo explo--room"]]

//Before the team is a wide, open room bathed in fog. Over a dozen tall, plant-like trunks of varying skin tones are spread throughout the chamber. Each hosts a complex array of tendrils at its apex that weave with those of their neighbors, forming a canopy that partially blocks out the fluorescent lights. Each trunk pulses rhythmically, with twin-bulbs that are seen to emerge from a chest-high orifice. The bulbs of each instance inflate and deflate in synchronicity. Shelving across the walls, as well as deconstructed server racks, would denote that this area had once served as the Site's Data Storage Center.//

霧に包まれた広い部屋の中には、10本以上もの、木の幹にもよく似たものが立っていた。一見すると植物のようにも見えるが、その表面は、さまざまな色の人皮に覆われている。それぞれの頂点からは無数の触手が伸び、隣の幹のそれと複雑に絡み合っている。天井の蛍光灯は、一部それに遮られている。幹が脈打つ。リズミカルに。胸の辺りに開いた穴からは、一対の球根状の器官が覗いていた。全ての幹の球根が、同時に膨らみ、同時に萎む。壁際には棚が並んでいる。解体されたサーバーラックのようだ。かつてここは、サイトのストレージセンターだったのだろう。

**Dr. Langford:** I... I'm gonna...

**ラングフォード博士:** は、吐き……

**Torres:** Swallow it. I thought you said this was the Director's office?

**トレス:** 飲み込め。ここは管理官執務室だと、そう言っていたな？

**Sebastian:** Are those fucking //lungs//?

**セバスチャン:** すげえや、こりゃ肺か？

//Nix takes point as the squad carefully advances. Just as with the canopy above, the entities are rooted in place via a thin network of mycellium that is splayed over the floor. The instances collectively shudder as this network is crushed underfoot.//

ニクスが先頭に立ち、部隊は慎重に前進する。床には、菌糸の網が薄く張り巡らされていた。天井の触手と同じように、この網も幹をその場に固定していると見える。隊員の足が菌糸を踏み潰すたびに、全ての幹が一斉に震えた。

**Dr. Langford:** Pul-- //(gags)// pulmonary vasculature is inherently fractal. It makes sense something like that could come under influence.

**ラングフォード博士:** 肺けっ--　　--オエッ、肺血管系はもとよりフラクタルです。それが影響を受けるということは、理には適っていると思います。

//Dr. Langford pauses.//

ラングフォード博士が黙る。

**Dr. Langford:** And... yes. It //should// be her office.

**ラングフォード博士:** そして……ええ、ここがが彼女のオフィスのはずです。

**Nix:** Whole site must have been rearranged. I'll have to thread a line here.

**ニクス:** サイト全体がめちゃくちゃになってるみたいだね。とりあえずここで、経路を確保するわ。

//Closer inspection of the nearest trunk reveals that the open orifice is surrounded by displaced teeth, forced outward by the expanding bulbs. The remnants of the face -- eyes, nose and ears -- have been rendered vestigial, being stretched along the backside of the trunk. As the entities collectively exhale, there is a quiet sighing; a fine mist can be seen to extrude from their open pores.//

近くの幹をよく見てみる。胸の高さに開いた穴の周囲に、葉が並んでいるようだ。内側から膨らむ球根に押され、外側へと剥き出しになっている。目や鼻や耳も、かろうじてわかるくらいの痕跡に成り果てている。それらは引き延ばされて、幹の裏側に平たく張り付いている。全ての幹が、同時に息を吐いた。静かなため息のようであった。開いた毛穴から、薄い霧が滲み出てくる。

**Torres:** Were these researchers? Langford, you recognize anyone?

**トレス:** こいつら、元は研究員か？　知っている顔はあるか、ラングフォード？

//Dr. Langford shakes his head. Warren moves carefully towards one of the trunks.//

ラングフォード博士が首を振った。ウォーレンは幹のうち一つに向かって、慎重に進む。

**Warren:** This gas... some kind of terraforming?

**ウォーレン:** このガス……テラフォーミングでもしているのかな？

//Sebastian grabs his knife and attempts to puncture the nearest bulb; it rebounds off. Sebastian curses under his breath.//

セバスチャンがナイフを抜き、手近な球根に突き立てようとした。刃は弾かれた。セバスチャンが小さく舌打ちする。

**Torres:** Whatever they're doing, we can't let it continue. Typhlo, got anything?

**トレス:** これがなんであれ、即刻中断させねばならん。ティフロ、何かわかるか？

**Typhlo:** {{Heart rates at... six beats per minute. Likely depend on retaining a circulatory system. Could bleed them out.}}

**ティフロ:** {{心拍数ハ……毎分6回。コレデ循環系ヲ維持シテイマス。出血サセルコトハ可能ナヨウデス。}}

//At this, Sebastian slices deep into the trunk beneath its orifice. Torrents of crimson blood rush from the wound -- the rest of the congregation whines and shivers as the wounded instance seizes and falls still. The deflated bulbs hang limply from its orifice.//

それを聞いた瞬間、セバスチャンが動いた。彼は幹に開いている穴のすぐ下に深々とナイフを突き立てる。真紅の血が吹き出した。傷ついた個体が痙攣し、やがて動かなくなった。他の幹たちが一斉に震え、そして呻く。それは悲鳴のようにも思えた。萎んだ球根が、穴からだらりと垂れ下がっていた。

**Torres:** Warren. Sebastian. You two handle them. Make it quick. I'll get on top of manually disconnecting these servers just in case they're still capable of sending out kill agents. I want Langford and Typhlo to dig through those files, see what you can see. Or... well, you know what I mean, Typh.

**トレス:** ウォーレン、セバスチャン。そいつらをどうにかしろ。手早くやれよ。俺は念の為にサーバーを手動で切断する。もしかすると、まだ殺害エージェントを送信できる可能性があるかもしれない。ラングフォードとティフロはそのファイルを掘り返せ。見られるものは全部見ておけよ。それか……まあ、言ってることはわかるだろ。ティフロ。

**Typhlo:** {{Offense not taken.}}

**ティフロ:** {{ぱわはらハヤメテクダサイ。}}

**Torres:** And Nix, you make good on our way out.

**トレス:** それとニクス。脱出経路は確保しておけ。

//Nix nods and produces a second Piton, finding a corner clear of mycellium to set it up. The remaining squad spreads out and gets to work. The quietude of their labor interrupted only by bursts of pained moans as each instance has its throat slit in turn. It is as Sebastian terminates the final instance that Dr. Langford calls out.//

ニクスは頷き、2本目のペグを取り出すと、菌糸に覆われていない床面に設置した。他の隊員たちも散開し、それぞれの作業に取り掛かる。幹の喉が切り裂かれるたびに苦痛のうめき声が響くほかは、静かな作業であった。セバスチャンが最後の一本を始末したとき、ラングフォード博士が声を上げた。

**Dr. Langford:** Hey, come take a look at this.

**ラングフォード博士:** ちょっと、これ見てくださいよ。

//The team converges on Dr. Langford, currently digging into a cardboard box. From within, he begins pulling out personal effects; keys, cigarette lighters, a handgun and taser -- he then pulls out a wallet, passing it to Warren before retrieving and opening a small leather purse. Sebastian rummages through the wallet, pulling out and discarding a credit card, before selecting from within a driver's license.//

段ボール箱を漁っていたラングフォード博士のもとへ、チーム全員が集まった。ラングフォードはその箱の中から、誰かの身の回り品を取り出していく。鍵、ライター、拳銃にスタンガン――そして財布をウォーレンに渡した。続けて小さな革製の小銭入れを引っ張り出して、開く。セバスチャンは受け取った財布の中身を確認する。クレジットカードを引き抜いて放り捨て、そして運転免許証を抜き取った。

**Sebastian:** Don't see any Foundation ID. Is this a civilian? You recognize this face, doc?

**セバスチャン:** 財団のIDカードがねえなあ。民間人か？　なあセンセイよ、この顔わかる？

//Dr. Langford looks up from the purse, stares at the license for a moment, then shakes his head. Nix reaches out and takes it from Sebastian.//

ラングフォードは小銭入れから顔をあげ、運転免許証をしばらく見つめた。そして彼は首を横に振った。ニクスが横から入り、セバスチャンの手から免許証を取った。

**Nix:** I do. This guy wouldn't be Foundation, no. I dug into Saunders' assignment after watching her footage -- missing persons investigation in the town down the way. This'd be Ernest Graham, age 42, one of the first to go missing back in March.

**ニクス:** 知ってるわ。この人は確かに財団関係者じゃない。例の動画を見たあと、ソーンダースの任務--　　--つまり、町の行方不明者捜索なんだけど--　　--について少し調べたの。この人はアーネスト・グラハム42歳。最初期の行方不明者のうちの1人ね。

**Torres:** Shipment of D-class would have been received in January. Guess they got impatient.

**トレス:** 次のDクラス移送は、一月だ。それまで待てなかったんだろうな。

//Dr. Langford cocks his head, looking at Torres.//

ラングフォードは顔をあげ、トレスを見た。

**Dr. Langford:** D-Class? That's... odd. They shouldn't have need for any more D-Class.

**ラングフォード博士:** Dクラス？　変ですよそれは。Dクラスなんか必要ないんですから。ここは。

**Warren:** At least we know why the tram was so active.

**ウォーレン:** 少なくとも、あのトラムが動いてた理由はわかったね。

**Sebastian:** Fuckin' snack runs. I'll be damned.

**セバスチャン:** Dクラス定期配達便ってか。笑えるぜ。

**Torres:** Good to know, but if there's nothing else here for us, let's keep pushing.

**トレス:** そうみたいだな。めぼしいものがもうないようなら、先に行くぞ。

//Torres makes for the door opposite from that which they'd used to enter. A porthole reveals that it leads into a hallway that runs perpendicular from this perspective. Sebastian and Warren pull out their rifles. Torres swipes his access card, and the door slides upwards.//

トレスは入ってきたドアの反対側にあるドアへと向かう。覗き窓から見ると、その先に廊下があることがわかる。廊下はこの部屋に対して垂直に伸びている。セバスチャンとウォーレンがライフルを構える。トレスがアクセスカードをかざし、ドアが上へと滑り開く。

[[div class="explo explo--room"]]

//Sebastian and Warren enter first, turning about to check the right and left flanks, respectively. Nix and Torres follow suit, sidearms held in a low-ready stance. As Dr. Langford crosses the threshold, he stumbles off balance, being caught and righted by Typhlo.//

セバスチャンとウォーレンが先陣を切り、それぞれ右と左を確認する。ニクスとトレスがサイドアームをローレディに構えながら続く。ラングフォード博士が入口を跨ぐ。その瞬間、彼は体勢を崩した。ティフロが彼を素早く支える。

**Nix:** Another shift. Get used to the vertigo.

**ニクス:** 転移だ。酔いに気をつけて。

//The hallway on either side of the team can be seen to bend circularly in a shallow corkscrew -- raising up and away on their right, and descending deeper on the left.//

部隊の左右に伸びる廊下が、緩やかな螺旋を描いて曲がっている。右へ行くほど上へと登り、左へ行くほど深く下っていた。

**Torres:** I know things aren't how you remember, doctor, but any idea which--

**トレス:** 記憶と違うのはわかるが、博士。どちらに--　　--

//A protracted inhuman scheech emanates from around the bend high above. The squad communicates in hushed tones.//

はるか上方、螺旋廊下の向こうから、人ならざる叫びが響く。隊員たちは声を抑えて意思疎通を図る。

**Torres:** Down it is. Typhlo?

**トレス:** 下からだな。ティフロ。

**Typhlo:** {{Hard to get a read on. I'm catching reverberations but it is fuzzy. The shape doesn't make sense. It is alone, I believe, but it is large.}}

**ティフロ:** {{判別ガ難シイデス。反響音ハ聞き取レマシタガ、ぼやケテイマス。ソレニ、形モ奇妙デス。オソラク単体デショウガ、大キイデス。}}

**Dr. Langford:** Only one? Should we... well, you, take care of it?

**ラングフォード博士:** 一体だけですか？　我々……つまりあなた方で、対処するんです？

**Sebastian:**  Yeah, how large we talkin'?

**セバスチャン:** そうだな。大きさはどれくらいだ？

**Typhlo:** {{You are welcome to find out. I will remember your bravery fondly.}}

**ティフロ:** {{是非オ確カメニナッテクダサイ。貴方ノ勇敢サハ、後世ニ語リ継ギマショウ。}}

//Torres elicits an exasperated sigh. He silently signals for Sebastian to cover their rear, and takes point down the downward path. The curvature of the hallway is such that forward sight is restricted past 15 meters. Looking into portholes as they progress, it can be seen the team is moving past the personnel quarters. The porthole on the last is shattered. A bloodied labcoat hangs in shreds from its lip. Glancing inside, it becomes clear the occupant had used their bedding to barricade the door.//

トレスが呆れたため息をつく。彼は無言でセバスチャンに後方警戒を指示すると、自ら先頭に立って下り坂を進みはじめた。廊下は緩やかに曲がっている。そのために、およそ15メートル先までしか見通すことはできない。隊員たちは進みながらも、覗き窓を確認していく。職員居住区を通過しているようだ。最後の覗き窓が砕けていた。その縁には、白衣だったと思われる、血まみれの布切れがぶら下がっていた。中を覗き込んでみると、部屋の住人が寝具を使ってドアをバリケードしていた跡が見えた。

**Typhlo:** {{Tapping. Up ahead.}}

**ティフロ:** {{こつこつ鳴ッテイル。前方。}}

//Rounding the next bend, a crimson web of thin tendrils coats the ceiling, extending for a length of several meters. It does not react to their presence. The squad carefully advances through to a four-way junction.//

角を曲がった先の天井を、絡み合った細い触手の真紅の網が数メートルにわたって覆っている。それは部隊の接近に反応を示さない。隊員たちは慎重にその下を通り抜け、四辻の交差点に出た。

//To the left, the hallway is dotted with double-locking doors along its length -- D-Class cells. Though the floor here is level, further down the hallway is a fork, and down each hallway is itself another fork. There is a minor optical illusion where it is difficult to interpret the middle branches, as focusing on either set of hallways reveals that they should spatially overlap the hallways on opposing branches.//

左には、二重ロックのドアが長さに沿って点在する廊下が延びている。Dクラス独房だ。この地点の床は平坦だが、廊下の先で分岐しており、分岐したそれぞれの廊下も、さらに分岐している。軽度の錯視が生じており、中央の分岐部分を解釈することが困難である。いずれか一方の廊下群に視点を合わせると、それらは対向する分岐の廊下と空間的に重複していることがわかる。

//To the right, the hallway continues forwards for 5 meters, ending on a heavy steel door. Signage indicates it to be the disposal area. A red pictogram conveys "Fire Hazard" beyond. It is the crematorium. The squad looks between the given three paths.//

右には、廊下が5メートル先まで続き、重い鋼鉄製のドアで行き止まっている。標識によれば廃棄エリアである。赤いピクトグラムは「火災注意」を示している。火葬場だ。部隊は3つの経路を見比べる。

**Warren:** Cap?

**ウォーレン:** キャプテン？

**Torres:** I want to make a run down through the cells, see if we can't find any survivors. Don't want to risk the attempt with the hall looking like this, though. Warren, you have your anchor?

**トレス:** 独房を見て回りたい。生存者がいるかもしれないからな。だがこんなところに入るリスクも冒せない。ウォーレン、現実錨はあるか？

//Warren nods. From his rucksack, he withdraws a small, portable SRA. After a moment's calibration, he sets it down facing the D-class wing. The air before it ripples and waves as it powers on. During this, Nix works to place a third Piton beside the crematorium door.//

ウォーレンが頷いた。彼は背負い鞄から小型の携帯式SRAを取り出した。しばらく校正をしたのち、ウォーレンはそれをDクラス独房区に向けた。SRAの電源が入る。空気が波打った。この間に、ニクスは3本目のペグを火葬場の扉のそばに設置した。

**Torres:** Let's give the SRA a few minutes to stabilize the area. In the meantime, we can dig through Disposal. Might be something worth finding in what they were throwing away.

**トレス:** 数分もすれば、SRAが空間を安定化してくれる。この間に廃棄エリアを探ろう。もしかすると、奴さんらが何かいいものを捨てているかもしれない。

//As the squad moves to follow Torres, backwards glances reveal that the crimson tendrils are now gone.//

トレスに続いて、隊員が移動する。広報の様子が一瞬だけ画面に映った。真紅の網は消え去っている。

//The metallic door leading into the crematorium swings inward with a heavy creak. Several hospital stretchers are scattered randomly about the chamber, leather restraints hanging from their sides. The headrest and upper-portions of each are blackened with dried blood that runs down the legs and cakes across the floor. The blood is seen to have not pooled naturally; rather, it has spread across the floor in intricate patterns. A fire roars in the furnace at the far end of the chamber.//

火葬場へ通じる金属製のドアが、重い軋み音を上げながら内側へ開いた。室内には、病院用ストレッチャーが無造作に散乱している。その側面からは革製の拘束具が垂れ下がっていた。各ストレッチャーのヘッドレストと寝台は乾いた血で黒ずんでいる。血は脚部を伝い、床に固着している。血溜まりは自然にできたものではない--　　--それは床全体に、複雑な文様を描いて広がっていた。奥の炉では火が轟々と燃えている。

//Countertops along the left wall are scattered with an array of surgical instruments, including no less than four blunted bonesaws and several glass containers holding a blue fluid. The liquid within glows with a bioluminescent sheen.//

左の壁面に据え付けられたカウンターには、多数の外科用器具が散乱している。刃の鈍った骨鋸が4本以上、青い液体の入ったガラス容器が数個。容器内の液体は、生物に由来する光沢を放っている。

**Warren:** This is foul. What were these monsters up--

**ウォーレン:** こりゃひどい。奴ら一体何を企んで--　　--

**Dr. Langford:** Berry picking.

**ラングフォード博士:** 苺摘みです。

//The others exchange a glance as Dr. Langford walks to the canisters atop the counter. He beckons the squad over.//

隊員たちが顔を見合わせる中、ラングフォードは容器の置いてあるカウンターへと歩み寄り、手招きした。

**Dr. Langford:** It's what she called it. Not officially, of course. In formal terms it was simply "harvesting".

**ラングフォード博士:** 彼女はそう呼んでいました。もちろん非公式にですが。正式な文書では単に「収穫」とされているものです。

//From up close, it can be seen that the solution within each canister suspends a living human head. Their eyes dart about wildly. Their lips tremble wordlessly.//

近くから見ると、各容器の溶液の中には、人間の頭部が生きたまま浮遊していることがわかる。その目は激しく動き回っている。唇は無言で震えている。

**Warren:** And you were on board with this?

**ウォーレン:** 君も、こんなことをやっていたのかい？

**Dr. Langford:** It was the only way we--

**ラングフォード博士:** これしか方法が--　　--

**Sebastian:** Didn't realize I signed up to handhold some sick fuck.

**セバスチャン:** イカれたファック野郎のお守りが仕事だとは思わなかったぜ。

**Torres:** But you did sign up, so shut up.

**トレス:** でも君は志願した。そういう言い方はないよ。

**Dr. Langford:** You don't understand... it wasn't like this. The process was clean. Surgical. Pain-free. This? This is a devolution.

**ラングフォード博士:** 違うんですよ……こんなんじゃなかったんです。あのプロセスはクリーンで、正確で、苦痛もないものだったんです。ですがこれは……そんなのとは程遠い。

**Nix:** It would have also been done with Eight's blessing. Now we know why the main file was mum about Berryman's research.

**ニクス:** エイトの名の下で行われていた実験でしょうね。ようやくわかったわ。メインファイルで、ベリーマンの研究がボカされてた理由が。

**Warren:** How are they still... alive?

**ウォーレン:** こいつらどうやって……生かされているんだ？

**Dr. Langford:** Above my clearance. All we know is that so long as they remain in the solution, they'd remain viable subjects. We could safely and repeatedly expose them to First Order FCI, and they would be brought back to life each time.

**ラングフォード博士:** それはぼくのクリアランス外です。ひとつわかるのは、彼らがこの溶液の中にいる限り、生きていられるということだけです。それで我々は彼らに第1級FCIを見せて、そうして彼らは死ぬたびに蘇生されています。

**Dr. Langford:** "Finite cases of infinite suffering, as opposed to infinite cases of finite suffering." She... she made it sound like a mercy.

**ラングフォード博士:** 「有限の苦しみが無限にあるか、無限の苦しみが有限しかないか」彼女はそう言っていました。まるでこれが、慈悲であるかのように。

**Sebastian:** Finite my ass. How come she still needed fresh D-Class?

**セバスチャン:** 有限もクソもねえよ。なんであの女まだDクラスが欲しいんだ？

**Dr. Langford:** I don't know! I'm just as in the dark as you are.

**ラングフォード博士:** わかりませんよ！　ぼくも何も知らないんです。あなたたちと同じで。

//Torres sighs.//

トレスがため息をつく。

**Torres:** Regardless, the Foundation isn't going to get much use out of them anymore. Permission granted to abort testing.

**トレス:** どちらにせよ、財団はもうこいつらに用はない。本試験を中止する許可を出す。

//The brothers quickly work to smash the glass of each canister. The heads eyes writhe about madly for a moment before falling still. As the last one is shattered, a piercing alarm is heard from the hallway.//

グッデン兄弟が素早く各容器のガラスを叩き割る。中の頭部の目が一瞬激しく動き回り、やがて静止する。最後の一つが砕かれると、廊下から甲高い警報音が響いてくる。

//The squad rushes back out to the junction, Torres in the lead. He holds his arm out as he exits the Disposal room, causing those behind him to skid to a stop. Before them, smoke is pouring out from within the SRA's casing. The hallway beyond, once a single iterative branching set, is now a kaleidoscopic array of intertwining paths and impossible branches. The SRA is beeping loudly, rapidly, as its frame begins to shudder. Half the team exclaim and shout out various expletives. Warren rushes ahead to the device and quickly punches a series of digits into the anterior terminal.//

部隊は四辻へ駆け戻る。トレスが先頭だ。廃棄エリアを出た彼は腕を上げ、後続を急停止させた。目の前のSRAの筐体から、煙が噴き出している。その向こうの廊下--　　--先ほどまで規則的に分岐していた廊下は、今や絡み合う経路と不可能な分岐の万華鏡と化していた。SRAが大音量で、速く、甲高い警告音を鳴らしている。筐体が震え始める。チームの半数が叫び、悪態をつく。ウォーレンが装置へ駆け寄り、前面端末に素早く数字の列を打ち込む。

//The beeping stops. A green light is emitted from atop the device. There is a quiet hum as the SRA shuts down. The hallway ahead remains in its altered state. Warren turns to the team and dramatically bows. He affects a high-pitch voice.//

警告音が止まる。装置上部から緑のライトが点灯する。SRAがシャットダウンし、静かなハム音が響く。前方の廊下は異常な状態のままだ。ウォーレンがチームの方を向き、大仰にお辞儀をする。彼は甲高い声を出す。

**Warren:** "Wow, Wally!" "Good job, Wally!" "Quick thinking, W--"

**ウォーレン:** 「ワオ、ウォーリー！」「よくやった、ウォーリー！」「機転を効かせろ、ウォ--　　--」

//The ceiling tile above Warren bursts open. None can react in time as a mass of veins and capillaries rapidly descend, spilling to the floor and raising up to take the approximate shape of a human. From its coils, an array of tendrils lash out and ensnare Warren. Dr. Langford is frozen. Nix and Typhlo raise their arms but cannot get a safe shot off on the entity. Warren screams as he tries to wrestle himself away.//

ウォーレンの真上の天井タイルが弾け飛ぶ。反応する間もない。静脈と毛細血管の塊が落下し、床に広がった。それはやがて人間らしき形をとり、立ち上がる。その渦巻く体から、触手の束が鞭打ち、ウォーレンを絡め取る。ラングフォード博士が硬直する。ニクスとティフロが銃を構えるが、誤射の危険性があった。ウォーレンが叫びながらもがく。

//Sebastian rushes forward, knife at the ready, as Torres lines up a shot with his sidearm. The bullet strikes the entity, causing it to loose its grip just as Sebastian lunges, cutting a long swath of blood vessels along its side.//

セバスチャンがナイフを構えて突進する。同時に、トレスが拳銃で照準を合わせる。弾丸が実体に命中する。拘束が緩んだ。セバスチャンが飛び込み、側面の血管を切り裂く。

//Falling off balance, the entity leans back into the fractured hallway, pulling Warren along with it. As they fall beyond the threshold, it becomes apparent that the gravity there is askew, causing them not to fall to the ground, but down the hall.//

平衡を崩した実体が、歪んだ廊下へ倒れ込む。ウォーレンを引きずったまま。両者が境界を超える。そして、廊下の向こうへと落ちていく。地面ではなく。重力すらも歪んでいた。

[[div class="explo explo--threshold"]]
//As they cross the threshold, Warren and the entity are seen to similarly refract as if multiplying, falling down all branches of the hallway simultaneously. They strike the wall as they tumble. Reaching out, Warren manages to grab hold of the handle on the nearest cell door. The entity, having fallen further, clings to his leg. Warren looks out towards the team, shakily extending a free hand. Sebastian leans in, grasping the corner of the hallway for leverage, and tries to take his brother's hand, finding his fingers are just out of reach.//

境界を越える。ウォーレンと実体の像が歪んでいく。屈折していく。増殖していく。転がりながら壁に衝突する。全ての分岐路を、同時に落ちていく。ウォーレンが手を伸ばした。その手は至近の独房扉の取手を掴んだ。だが実体は落ちてゆく。それは彼の脚にしがみついている。ウォーレンは隊員を見た。そして震えながら空いている方の手を伸ばす。セバスチャンが身を乗り出して廊下の角を掴み、体を支える。そのまま弟の手を取ろうとするが、届かない。わずかに。

[[/div]]

//Sebastian pulls back into the crossroads.//

セバスチャンは四辻へ戻った。

**Sebastian:** Well? Fucking don't just stand there!

**セバスチャン:** おいこら、ボケっとしてんじゃねえよ！

//The team, excluding Dr. Langford, who now slides down the wall, shivering, work to form a human chain. Each is locked arm-in-arm, holding onto Sebastian as he descends into the hall.//

ラングフォード博士は壁際で座り込み、そして震えていた。彼以外の隊員は、それぞれ腕を組み合わせて人の鎖を作る。セバスチャンはそれを頼りにして、穴の中へと降っていく。

[[div class="explo explo--threshold"]]
//Sebastian is easily able to make contact, grasping his brother's hand tightly.//

セバスチャンは弟の手をしっかりと掴む。今度は思いの外簡単に届いた。

**Sebastian:** I got you! //(grunts)// I got him! Pull!

**セバスチャン:** 大丈夫だからな！　//(うめく)//　捕まえた！　引き上げろ！

//As Sebastian begins to pull Warren out, the entity spreads itself wide. Its vessels find purchase in the surrounding walls of the shaft. It pulls in kind with a greater degree of force -- Sebastian is dragged a half-meter deeper, with Torres now sliding halfway past the threshold.//

彼はウォーレンを引き上げようとした。その時、実体が体を大きく広げた。血管が周囲の壁に食い込む。実体はウォーレンを離さない。その剛力で、セバスチャンは半メートルほど引き摺り込まれた。トレスも道連れになりそうだ。彼の半身が、境界を越える。

**Torres:** Sunnuva bitch!

**トレス:** こんちくしょう！

//Warren continues to wrestle the entity as it climbs further up his leg. His hand slips from Sebastian's grasp; causing the human chain to rebound back with the force of their pulling. Nix grunts as she's thrown to the ground, Typhlo falling in her lap. Warren now clings only to the door handle. He glances down at the entity, then turns his gaze to the team.//

ウォーレンと実体はもつれ合った。それは彼の脚をさらに這い上がってくる。セバスチャンの手が滑った。彼の手はウォーレンから離れてしまう。力の行き場がなくなって、人間の鎖が後方に弾け飛んでしまう。ニクスが地面に投げ出されて呻き声を上げた。ティフロが彼女の上に倒れ込む。ウォーレンはかろうじて、ドアの取手だけにしがみついている。彼は実体を見下ろした。そして、隊員に顔を向ける。

**Warren:** It's... it's no use. Tell mom I said--

**ウォーレン:** もうダメだ……おしまいだ。ママに伝えてくれ。俺は--　　--

//Sebastian lets out a rage-laden roar and leaps into the shaft, falling past Warren and colliding into the tangle of veins, tearing into it with his knife. The vessels lose their grip on Warren as the struggling pair fall away deeper into the hallway.//

セバスチャンは怒りに満ちた咆哮を上げた。彼はナイフを抜き、歪んだ廊下の中へと飛び込んでゆく。ウォーレンすら通り越してしまうと、絡み合った血管の塊をそのナイフで切り裂いた。セバスチャンと実体はもつれあい、さらに深くへと落ちていく。血管が、ウォーレンから離れた。

[[div class="explo explo--threshold"]]
//Sebastian falls, entangled with the beast. He grunts as the pair painfully rebound off the sides of the shaft. All around them, the repeating pattern of the hallway and equally-spaced cell doors whiz by.//

そうして落ちていく最中、壁面に衝突し、跳ね返るたびに、セバスチャンは苦悶の声を上げた。ゴウ、と空気を切り裂く音を立てながら、両者は自己相似の廊下と、等間隔に並んだ独房のそばを通り過ぎていく。

//The entity worms its veins around Sebastian's mask, prying it from his face -- it flies off into the endless expanse above them.//

実体の血管がうねり、セバスチャンの覆面を引き剥がした。そしてそれは、無限に広がる空間の中へと消えていく。

[[div class="explo explo--threshold"]]
//Deeper still.//

深く、そして深く。

//Sebastian bites down hard on an artery as the tendrils work to strangle him, and is sprayed with a red mist. The entity loses its grip and latches onto the sides of the shaft as Sebastian continues to descend.//

実体が彼を絡め取ろうとする最中、セバスチャンはその動脈に噛みつく。噴き出た血は、まるで赤い霧のようであった。彼は実体の拘束から離れた。実体は壁面に掴まる。セバスチャンはひとり落ちていく。

//The walls fall away -- the setting dissolves into an inky black that presses in on all sides despite its seeming non-existence.//

壁が消え失せた。周りに何かがあるとも思えない。それでもなお、墨汁じみた何かが圧しかかってくる。

[[div class="explo explo--threshold"]]
//Deeper still.//

深く。そして深く。

//The speed at which the fading light above retracts would indicate that Sebastian has reached terminal velocity. Despite this, there comes a woolly scraping as friction with the surrounding darkness tears away at clothing.//

セバスチャンが終端速度に達した。はるか上にある明かりのすぼむ速度が、一定になったからだ。セバスチャンの衣服が引き裂かれていく。まるでやすりか何かに、体を擦り付けているかのようであった。

//At skin.//

皮膚も裂ける。

[[div class="explo explo--threshold"]]
//Deeper. Faster. Sebastian grunts and strains as he works to raise flayed arms over his head. Still, the surrounding space tightens. There is a resounding **crunch**. Sebastian screams as his body contorts, his limbs and torso caving inwards, covering the camera lens.//

より深く、より速く。身悶えしながらも、苦悶の声を上げながらも、セバスチャンはすっかり皮のはげてしまった腕を懸命に上へ伸ばす。空間が潰れていく。**圧壊**の音が響いた。セバスチャンは絶叫を上げた。体が捻れて、両手両脚があらぬ方向に曲げられている。カメラの映像が、四肢に覆われてしまった。

//A second **crunch**. Sebastian continues to scream.//

2度目の**圧壊**。セバスチャンは叫び続ける。

[[div class="explo explo--room"]]
[[=]]
**crunch**

**圧壊**

//Sebastian has stopped screaming. The sound of rushing wind is the only indicator that the perspective continues to descend.//

絶叫が止んだ。風を切る音だけが、落下を示唆している。

[[/=]]

[[div class="explo explo--room"]]
[[=]]
**crunch**
//The perspective begins to clear as Sebastian's remains come apart in tatters.//

セバスチャンの骸が、ばらばらに引き裂かれている。

**crunch**

**圧壊**

//A crack forms across the lense.//

レンズが罅割れる。

[[/=]]

[[div class="explo explo--room"]]
[[=]]
**crunch**

**圧壊**

The feed is lost.

映像が途切れる。

[[/=]]
[[/div]]

 _

[[div class="explo-rising"]]
//The//

彼の
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//clamoring of//

不鮮明な

[[/div]]
[[/div]]

[[div class="explo-rising"]]
//his anguished screams//

叫び声だけが
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//reverberate upwards and out//

名状し難い竪穴を

[[/div]]
[[/div]]

[[div class="explo-rising"]]
//through the impossible hallways and//

反響し、轟音となって

[[/div]]
[[/div]]

[[div class="explo-rising"]]
//echo up into the corridor where the team tries//

危険地帯にいるウォーレンを

[[/div]]
[[/div]]

[[div class="explo-rising"]]
//to pull Warren from his precarious position in the shaft.//

救出しようとする部隊まで響いた。

[[/div]]
[[/div]]

//With their collective might, they are successful in bringing Warren to safety.//

彼らは力を合わせて、ウォーレンを安全地帯へと回収することに成功した。

//Warren collapses on the ground, hyperventilating. He tears the mask from his face and vomits profusely. Nix works to fully disassemble the SRA's vital components, swearing repeatedly under her breath. She casts discarded materials one after another into the fractured hallway.//

ウォーレンは過呼吸を起こしながら蹲った。そして覆面をとると、大量に嘔吐した。ニクスは消え入るように悪態をつきながら、現実錨の重要部品を分解し、それを一つずつ、やぶれた廊下へと捨てていく。

**Nix:** This isn't good. Damnit, Captain, they have these things set up all around the site!

**ニクス:** こりゃダメだわ。キャプテン、奴らこんなのをサイト全体に仕掛けてるんじゃないの！

//Torres nods.//

トレスが頷く。

**Torres:** If the AOE spreads far enough, reaches the Exclusion Zone...

**トレス:** 異常空間がこれ以上広がって、立入禁止区域へ差し掛かったら……

//Dr. Langford stutters, unable to intelligibly speak.//

ラングフォードは言葉を失っていた。彼の口からは無意味な音しか出てこない。

**Typhlo:** {{That cannot be allowed to come to pass.}}

**ティフロ:** {{あれハ絶対ニ外ヘ出シテハイケマセン。}}

//Torres attempts to hail Command as Warren wipes his mouth. Typhlo extends a hand, helping him to his feet. Torres tries a second channel, then a third; each is a garble of static.//

ウォーレンが口を拭いている間、トレスは司令部と連絡を取ろうとする。ティフロがウォーレンに手を貸して、彼を立ち上がらせた。トレスは2個目、3個目のチャネルも使って連絡を試みる。しかし、どれも不通だった。

**Torres:** No dice. It's gonna be on us to stop this here and now.

**トレス:** こうなっちまったからには、俺たちがこれを終わらせないといかんな。

**Dr. Langford:** What if we can't? It's not like there will be a big "OFF" switch.

**ラングフォード博士:** それができなかったらどうするんです？　どこかに電源ボタンがあるってわけでもないでしょうに。

**Warren:** There's //always// a big "OFF" switch.

**ウォーレン:** あるんだよ。でっかい電源ボタンが。

//Warren affixes his mask.//

ウォーレンが覆面を付け直す。

**Warren:** On-site nuke. Bring the whole darn thing down.

**ウォーレン:** 核爆弾があるだろ。それで全部おしまいにできる。

//Nix tosses the empty shell of the SRA into the fractured hallway with a laugh.//

ニクスが現実錨の外殻をやぶれた廊下へ投げ入れ、笑った。

**Nix:** You really think we have those?

**ニクス:** 本当にそんなのあると思ってるの？

**Typhlo:** {{Site warheads are retained in files as a form of misinformation. We've not had those since the 80s, at least.}}

**ティフロ:** {{さいと地下ノ核弾頭ハ、アル種ノかばーすとーりーノヨウナモノデス。80年代以降、ソノヨウナモノハ運用サレテイマセン。}}

**Warren:** //(quietly)// Goddamnit, Seb. Got me again.

**ウォーレン:** //(小声で)//ちくしょう、またやっちまった、アニキ……。

**Torres:** You're on the right path though. We're not without our Hail Mary.

**トレス:** あながち間違いというわけでもない。切り札は、あることにはある。

//With this, Torres withdraws a small handheld device from a breast pocket. It is slender, and sports a single red button beneath a transparent guard.//

そう言いながら、トレスは小さめの携帯デバイスを、胸ポケットから引っ張り出した。それは細ながく、また赤いボタンがひとつ、透明な蓋の下で存在を主張している。

**Warren:** A detonator?

**ウォーレン:** 起爆装置ですか？

**Torres:** A transmitter. One whose "signal" is a quantum-entangled particle with that of a partner at Site-01. One push and this place has five minutes before everything in a ten kilometer radius is glassed.

**トレス:** 発信機だ。量子もつれを利用して、サイト-01にある兄弟機へ信号を送ることができる。このボタンを押せば、5分と経たないうちに、周辺10キロメートルが消し炭になる。

**Nix:** Orbital bombardment.

**ニクス:** 軌道爆撃だね。

**Warren:** Is that not functionally the same as an on-site nuke?

**ウォーレン:** サイト地下の核爆弾と、役割的には同じですね？

**Dr. Langford:** Well, if you want to consider the practicalities of it, then no. It may come as a shock to you, but not everyone is comfortable sitting on top of a literal nuke.

**ラングフォード博士:** 実用性の面でいえば、ノーです。核弾頭が足元にあるとなれば、人は落ち着けないものです。あなたがどうかはわかりませんが。

**Torres:** Even fewer would want to be the one to pull the trigger. Greater good can be a hard pill to swallow when self-preserva--

**トレス:** そしてそれを喜んで起爆しようとする奴など、いないと言ってもいいだろう。認め難いものだよな。自己の存亡を前にすれば、より大きな善というものは--　　--

//There comes a sound of pounding on tile, rapidly drawing near. From up around the main hallway there is a piercing chorus of screams from a dozen voices.//

床面を叩くような音が急速に近づいてくる。中央廊下の向こうから十数人の甲高い悲鳴が響く。それはもはや、合唱じみていた。

**Torres:** Shit!

**トレス:** クソが！

**Langford:** They're coming!

**ラングフォード博士:** 奴ら来ますよ！

**Typhlo:** {{Singular. **It's** coming.}}

**ティフロ:** {{単体デス。奴ガ来マス。}}

**Torres:** Either fucking way, move it!

**トレス:** どっちでもいい！　対処するんだ！

//The squad breaks out into a run down the main hallway. They round bend after bend, ignoring side-paths as they come across them: the cafeteria doors at the end of one hall lay forced open from within by a throng of twitching fingers that continuously branch and grow and branch again; a wing designated SL-2 cannot be sighted for the mass of hair that seems to grow from every surface, blotting out the lights within; the maintenance sublevel, choked by an over-abundance of twisting, knotted pipes.//

部隊は中央廊下を駆ける。次々と角を曲がっていく。脇道には目もくれない。その突き当たり、カフェテリアのドアが内側からこじ開けられた。絶えず枝分かれし、痙攣しながらも成長する指の群れによって。そしてSL-2なる区画は、あらゆる表面から生える大量の髪の毛に覆われている。それは内部からの光を、そして視界を遮っている。メンテナンス用の地下フロアは、捩れ絡み合う無数の配管で埋め尽くされている。

**Torres:** Fuckin' pipes.

**トレス:** ひでえ配管だな。

//The floor here transitions from smooth tile to rough metal railing. White walls fall away to grey concrete. The pounding and the wailing grow louder as the creature slowly gains on the squad. Dr. Langford, trailing behind and clearly winded, steals a backwards glance, catching an impression of the beast -- of broken, disjointed wrists splitting into too-many hands that smash into the ceiling, the walls, the floor; all crashing down with shattering force. Dr. Langford elicits a panicked whimper, desperately charging ahead to catch up to the others. A second glance. Grasping hands explode from palms, each finger itself becoming host to another in rapid succession.//

床が滑らかなタイルから、ざらついた金属へと切り替わる。壁の白い塗装はもはや剥がれ落ちていて、コンクリートの灰色が剥き出しになっていた。床を叩くような音と、何者かの絶叫が大きくなっていく。怪物が部隊との距離を、ゆっくりと詰め始めている。ラングフォード博士は、隊列から遅れ始めていた。息も絶え絶えに、彼は振り向いてしまった。ひしゃげた手首から生える無数の手が、天井を、壁を、床を粉砕させんばかりの力で叩きつけている。ラングフォード博士はか細い悲鳴を漏らし、皆へ追いつこうと必死に前に駆ける。彼は再び、後ろを見てしまった。一つ一つの手の平から、まるで爆発でもしているかのように、新しい手が生まれ出て、その指の一本一本が、また新たな手となっていく。それらは、ラングフォード博士へと殺到する。

[[div class="scp-image-block block-center" style="width: 100%"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/abomination.webp]]
[[/div]]

//Gone now is the overhead fluorescence that bathed the halls above; their flight is now lit by individual bulbs whose fixtures swing from the tremorous force of the advancing behemoth. Each shatters in turn as it comes across them. Drawing nearer.//

彼らの逃走を照らしているのは、今や剥き出しの電球だけだった。蛍光灯の光などという贅沢は、もはやここには届かない。迫り来る実体の引き起こす振動で、その一つ一つが振り子のように揺れている。実体が通るたびに、電球が順に爆散していく。それは、すぐそこまで来ている。

//Up ahead, Torres passes through an open bulkhead, skidding to a stop at a control panel on the opposing side. He is followed by Warren, who brandishes his rifle. A klaxon rings out as Torres pulls a lever, and the bulkhead doors slowly emerge from either side to close in the middle. Nix follows through third, withdrawing her rifle. In a single motion she turns about, assumes a kneeling position, and fires over Dr. Langford and Typhlo in three-round bursts. Typhlo does not adjust her course or react as she races to join the others. Dr. Langford, however, flinches in surprise, trips, and stumbles hard to the ground. He rolls onto his back, groaning and clutching his forehead.//

前方の開いた隔壁を、トレスが駆け抜ける。その勢いを殺しきれず、彼はブーツを滑らせながらも反対側の制御盤にたどり着く。小銃を構えたウォーレンが彼の背後へとやってくる。トレスがレバーを叩きつけた。けたたましい警報が鳴る。分厚い隔壁が唸りを上げながら、両側の壁面からせり出してくる。3番目にニクスが滑り込んだ。彼女は振り返ると同時に膝をつき、流れるような動きで銃を構える。三点バーストで放たれた銃弾が、ラングフォードとティフロの頭上を掠めていく。着弾の音に怯むことなく、ティフロはそのまま走り抜けた。他方でラングフォード博士は、その銃声に身がすくみ、足がもつれてしまう。彼は体勢を崩し、地面に勢いよく叩きつけられた。仰向けになると、彼は呻きながら、強打した頭を押さえた。

//Typhlo rushes to Dr. Langford's side as he weakly attempts to scramble backwards. From the darkness before them, innumerable fingers extend and cling to scaffolding only to be subsumed and overcome by yet others. It becomes apparent in this moment, as its limbs fracture into fresh iterations, that the behemoth has not simply been chasing after them. It was growing. From within its center emerge several gaunt, howling faces who each hold wide their maws, birthing from within perfect replicas that repeat the process in kind. A dozen sets of lifeless eyes peer out from a thick tangle of hair. The squad's shots do little to deter their recursive germination.//

逃げようともがくラングフォード博士のもとに、ティフロが駆け寄る。目の前の暗闇--　　--そこから無数の指が伸びては足場に絡みつき、さらに新しく生まれた指に飲み込まれ、覆われてゆく。その手足が分裂し、新たな姿かたちをとってゆく様を見れば、誰であろうと悟るだろう。あれはただ、迫ってきたのではなく、成長していたのだと。その中心から窶れた顔面が突き出る。苦しげに開かれた口、その仄暗い喉奥からまた同じ顔が生まれる。苦艱の声を上げながら、同じ顔が増殖していく。絡み合った髪の毛の奥深くから、十数対もの虚ろな瞳が、こちらを覗き込んでくる。隊員が銃撃をする。しかし、その無限再帰の増殖を止めるには、あまりにも心許ないものであった。

//With the bulkhead doors a meter apart, and Dr. Langford too stunned to escape, Typhlo grips about his collar and waistband. She hurls him forward and just past the closing doors. In the moments before the doors fully seal, Typhlo is seized and pulled airborne. Untold numbers of clawing, skewering fingers dig into every perceivable surface. In less than a second, every bit of her is separated from the next in a fountain of viscera. The bulkhead seals.//

あと数十センチで、隔壁が完全に閉じてしまう。しかしながら、ラングフォード博士は完全に呆けてしまっていた。ティフロが彼の襟首とベルトを掴み、閉まりゆく扉の向こうへ投げ飛ばす。扉が完全に閉鎖されるその瞬間、ティフロの体が宙に吊り上げられる。無数の指が、鉤爪が、杭となって彼女の体のありとあらゆるところに突き刺さり、食い込んでゆく。コンマ数秒で彼女の体は完全に引き裂かれる。臓物が宙を舞い、血の雨が降った。隔壁が、閉じる。

//Dr. Langford alone yelps as the bulkhead is struck repeatedly with force from the opposite side.//

隔壁の向こうから、凄まじい衝撃音が響く。一度とならず、何度でも。ラングフォード博士だけが、短い悲鳴をあげた。

//The squad takes the opportunity to catch their breath -- now visible in dissolving clouds in the chill of the room. Warren helps Dr. Langford up from his place sprawled on the scaffolding. They're in a darkened antechamber, lit only by rotating emergency lights inlaid across the ceiling from one end to another -- where a second bulkhead now slowly opens.//

部隊はようやく、息をつくことができた。部屋は冷え込み、吐く息が白い雲となっては消えていく。ウォーレンが、足元に倒れていたラングフォード博士を助け起こした。暗闇の中でも、ここが何かの控え室であることはわかる。天井の端から端まで、列をなして埋め込まれた非常灯が回転をはじめ、赤色の光が何度となく部屋の中を舐め回す。それが唯一の光源であった。そして、その光の照らす部屋の奥側で、2つ目の隔壁が、今、ゆっくりと開く--　　--

**Torres:** Where the hell are we, Langford?

**トレス:** ラングフォード、俺たちどこにいるんだ？

//Red light spills in from the crack of the opening door.//

隔壁の隙間から、赤い光が漏れた。

[[div class="explo explo--room"]]

**Dr. Langford:** We've... we've made it.

**ラングフォード博士:** やった……たどり着いたんですよ。

//The doors fully open to reveal the SCP-9001 production center. The space here is dark. The only source of light comes from a dozen terminals stretching across the eastern wall that makes up the bulk of the production apparatus. Isolated terminals atop several desks account for the remainder of the ancillary illumination. There is subtle movement in the darkness, accompanied by the sounds of frenetic typing and a haggard breathing.//

隔壁が完全に開き切ると、そこはSCP-9001生成センターであった。暗闇の中に沈む部屋の中、十数台の端末が光を放っていた。東側の壁一面に広がる、生産装置の画面であった。そのほかには、机の上にいくらか置かれている端末が、わずかにあたりを照らしているに過ぎない。暗闇の奥で、何かが動いた。憔悴しきった、荒い呼吸の音に混じって、狂いじみたタイピング音が聞こえてくる。

//Proceeding with caution, arms at the ready, Torres and Warren activate their torches. Splayed all about the floor is a collection of loose skin. Torres' light traces its way across the flesh of the abomination to where narrow limbs raise up from within its folds. Elongated fingers and toes multiply and iterate, extending towards various keypads throughout the command center, where it endlessly types a series of commands and prompts. The head of an aged male dangles upside-down in its center, supported by a willowy neck.//

銃を構えながら、トレスとウォーレンは慎重に歩を進める。両名はライトをつけた。床一面に散らばる、弛みきった皮膚の塊が、眩い光で照らされる。悍ましい肉塊の上を、トレスのライトが滑っていく。肉襞の隙間から伸びる、何本もの細長い手足をとらえた。間延びしたかのような指先と足先が、自己増殖を繰り返しながら、司令室のあちこちにあるキーパッドへと伸びている。そして、無数のコマンドとプロンプトを際限なく打ち込んでいた。やがてライトが、その中央に向く。柳の枝めいたしなやかな首に支えられて、年老いた男の顔が、逆さまにぶら下がっていた。

**Dr. Langford:** Dear God... Dr. Coleman?

**ラングフォード博士:** そんな……コールマン博士？

//The thing that had been Coleman strains its neck to turn and regard the approaching squad. It draws a rattling breath. Its lips purse. A sound that could be mistaken for "please" escapes its throat as Torres takes aim with his sidearm. It is struck between the eyes. The typing ceases.//

かつてコールマンであったのだろう「それ」は、何かを軋ませながら首を捻り、近づいてくる部隊の方を向いた。「それ」の喉奥から、声にもならない息が漏れた。かろうじて残っている意識が、その唇を動かした。トレスが、サイドアームの照準を合わせた。「頼む」--　　--ただのか細い音だったが、そう言ったようにも思える。銃弾がその眉間を正確に撃ち抜いた。タイピングの音が、止んだ。

**Torres:** Things are looking up, folks. That's one objective on a silver platter.

**トレス:** 上等だ、諸君。棚から牡丹餅ってところか。

//Nix shines his light across the room to a steel door on the far side. "ACCESS - L4 ONLY" is emblazoned across it in bold red letters.//

ニクスは、部屋の対面にある鉄扉へとライトを向けた。それは赤い太字で「要レベル4クリアランス」と印字されている。

**Torres:** What's in there?

**トレス:** 中には何が？

//Dr. Langford sighs.//

ラングフォード博士がため息を漏らす。

**Dr. Langford:** That would be our Kempelen facility.

**ラングフォード博士:** ケンペレン施設があるはずです。

**Nix:** Think we might be able to find Berryman in there?

**ニクス:** ベリーマン居るかな、この中に。

**Torres:** We'll find out in a minute. Warren: think you can extract SCP-9001?

**トレス:** 今にわかるさ。ウォーレン、SCP-9001を回収できるか？

**Warren:** Aye, chief.

**ウォーレン:** アイアイ、キャプテン。

//Warren clumsily scrambles over the remains of Dr. Coleman. He approaches one of the terminals and messily extracts Dr. Coleman's fleshy interfaces from the computer. The slimed tendrils slide out from the crevices with a sickening squelch. Warren withdraws a small fob and plugs it in. Torres motions for the others to follow him as he clambers over the bulk as well towards the opposite end of the room. Warren exclaims as the process completes, and rushes to join them.//

ウォーレンがどうにかこうにかコールマン博士の亡骸を乗り越え、端末の1つへと駆け寄ると、コンピューターに突き刺さっている肉質のインターフェースを無造作に引き剥がした。粘液に塗れた触手が隙間から滑り出た。ぐじゅり、と吐き気を催すような水音を立てながら。彼は懐から小さな暗号キーを取り出して、ポートに挿し込んだ。その間、トレスは部屋の反対側へ向かいながら、同じように肉塊を乗り越えていきつつ、他の者に追従するよう手振りで示す。やがて処理の完了を知らせる音が鳴った。ウォーレンが声を上げて、急いで部隊へ合流する。

//With Torres' access card, the door opens with a hiss. Bright lights within cause the team to wince as their eyes adjust.//

トレスのアクセスカードを以て、空気が抜ける音とともに扉が開いた。眩い光が漏れる。隊員たちは思わず目を細めた。まだ光に順応できていない。

//The door fully opens to reveal a massive, domed chamber; a twenty-sided room walled with stone columns that curve upwards, forming the dome, and a weaving pattern of interlocked stone tiles adorns the interior surface of the vaulted ceiling. The pale white of the fog outside is visible through a small circle of glass at the very top.//

扉の向こうには、正二十面体の巨大なドーム状の空間が広がっていた。それぞれの角に立つ柱は、上に向かうにつれて緩やかに湾曲し、そのままドームの骨格となっている。その内側を、複雑に組み合わさった石のタイルが埋め尽くしていた。それはまるで織物のように複雑で、緻密な紋様を描いている。はるか頭上、ドームの頂点には、小さな円形の天窓があった。そのガラスの向こうに、外界の青白い霧が見える。

//At the far side of the room is a double door of the same variety through which they had just entered. Lettering across the door reads "SUBJECT PERSEUS". On all other sides of the room, nestled between the columns, are recessed alcoves. Within each is a Berry canister, each containing a living human head suspended in the blue fluid. The caps of their skulls have been removed. Electrodes connect directly from grey matter to a series of wires that snake around furrows in the wall, leading them into an aperture leading to the SCP-9001 production center. As the squad maneuvers into the facility proper, it can be seen that with some regularity, the grey matter of certain instances has grown and refracted, bulging from their craniums. Some have grown to the point of fully subsuming the head in the solution, and others have cracked or shattered their canisters from sheer girth. Small screens attached to retractable arms are held before the eyes of each head within the canisters, all of which are blank.//

部屋の最奥には、今しがた潜ってきたものと同じような両開きの扉がある。その扉には、「ペルセウス対象」なる文字が刻まれていた。その他の壁面、石柱と石柱の間には、等間隔で壁龕が設けられている。それぞれの内側には、円筒形のキャニスターが鎮座していた。中を覗き込んでみれば、青い液体の中に生きた人間の頭部が浮かんでいることがわかる。その頭頂部は切り取られ、剥き出しの灰白質には、直接電極が突き刺さっている。そこから伸びる無数のワイヤーは、壁に刻まれた溝を蛇のように這い、SCP-9001生成センターへとつながっているのであろう空隙へと伸びていた。隊員が空間の中へと慎重に歩みを進めるにつれ、さらなる異常が明らかとなる。キャニスターに収められている頭部、そのうちいくつかの個体においては、脳そのものが異常な増殖と変質を遂げ、頭蓋骨から溢れてしまっている。脳組織が頭部全体を飲み込むまでに肥大化しているものもおれば、膨れる脳の圧力に耐えきれなかったのか、キャニスターそのものが粉砕されているものもある。全てのキャニスターには、拡張式のアームが取り付けられている。それぞれの頭部の眼前には小さなスクリーンが掲げられていた。だが、その画面はどれひとつとして、何も映してはいなかった。

//Underfoot, the floor is a mosaic, shards of glass and ceramic coalescing into a complex network of shapes and colors that makes the eyes water, polished to a shine. In the very centre of the room is a leather armchair and a wooden desk, atop of which is a tumbler and a bottle of Macallan, both empty. The room is a panopticon.//

緻密なモザイク模様が床面を埋め尽くしていた。輝きを放っていると錯覚するほどに磨き上げられたガラスや陶器の破片が、見る者の涙を誘うような複雑なネットワークを描いている。その中心に革張りのアームチェアと木机が、ポツンと置かれていた。机の上には空のタンブラーと、同じく空のマッカランが置いてある。とどのつまり、この部屋はパノプティコンなのだ。

**Torres:** This is how you define "finite"?

**トレス:** これが「有限」ってやつか？

//Dr. Langford does not respond as Warren charges ahead to Berryman's desk, digging into the drawers and coming out with a ream of documents. Torres forges ahead, strolling past Berryman's desk towards the opposite door. Dr. Langford, close behind, leans down to pick up a small object. It is a hair brooch decorated with clusters of small, white flowers.//

ウォーレンはベリーマンの机へと駆け寄り、引き出しを漁って書類の束を引っ張り出す。その間も、ラングフォード博士は上の空であった。トレスはそんな2人を意にも介さずに机の横を通り過ぎ、部屋の反対側にある扉へ落ち着き払った足取りで向かっていく。そのすぐ後ろにいたラングフォード博士が、ふと足をとめ、身を屈めて何か小さなものを拾い上げた。白く小さい花のいくらかあしらわれた、髪留めだった。

//Five large metallic instruments are braced around the circumference of the door ahead -- Containment-Grade Scranton Reality Anchors. The collection is currently inactive. Warren, catching up, points to a pull cord that runs alongside the perimeter of the door.//

前方の扉を取り囲むように、5基の金属製で大型な装置が設置されていた。オブジェクトの収容にも用いられるほどに上等なスクラントン現実錨--　　--現在は非稼働状態--　　--だ。追いついてきたウォーレンが、扉の周縁に沿って配置されているプルコードを指差した。

**Warren:** Emergency cord for the SRAs. Wanna watch out that nobody catches on that accidentally. We don't need that kind of problem right now.

**ウォーレン:** こいつを触ると、現実錨が起動しちまう。トチって引っかからないように注意してくれ。余計な面倒は御免だよ。

//Torres nods, approaching a keypad inlaid into the door's center. He swipes his card on the door's keypad to no effect.//

トレスは頷き、扉の中心部にあるキーパッドに自身のカードを読み込ませた。だが、何も起こらない。

**Torres:** Damn. Must be keyed to Berryman exclusively.

**トレス:** チキショウ。こりゃベリーマン専用か？

//Nix strays off to the edge of the room, peering into one of the glass canisters. Warren jumps in front of Torres.//

ニクスが部屋の端へ退き、キャニスターのひとつを観察している。ウォーレンがトレスの前へ割り込んだ。

**Warren:** Let me see. I know some of the default emergency access codes. If she was the lazy type, she'd not have thought to reprogram them. You'd be surprised how many researchers lean on keycards.

**ウォーレン:** ちょっと拝見。デフォルトの緊急アクセスコードがありましてね、もしベリーマンが不精者なら、そのコードがそのまま使われてるはずです。研究者の先生方は、キーカードに頼りっきりですからね。

//Warren swiftly types, eliciting electronic buzzes with each wrong guess. Dr. Langford crosses his arms.//

ウォーレンが素早くタイピングしていく。しかし、そのどれも正しいコードではなかった。ブザー音が何度も鳴る。ラングフォード博士は腕組みをしながら、その様子を見ていた。

**Dr. Langford:** No, not Berryman. She wouldn't just leave something out of her control.

**ラングフォード博士:** ベリーマンに限って、そんなことはしませんよ。何かを自分の制御の外に置くなんてことは。

//Nix calls out from the other side of the room.//

ニクスが部屋の反対側から呼びかける。

**Nix:** Her file was a bit sparse. Any relatives? Names of pets? Could try the sentimental angle.

**ニクス:** そんなこと言われてもねえ。血縁者は？　ペットとかいた？　何か感情的に重視していたものはある？

**Dr. Langford:** Not that she'd mentioned, no. Used to feel bad for her, you know, not really having anybody, but after working with her so long it became clear the only thing she cared about was- oh... oh, goddamnit.

**ラングフォード博士:** いや、いませんね。あまりこういうことは言いたくないんですが、本当にそういうのは何もないんですよ。一緒に仕事をしてからこっち、ベリーマンが大事にしていたものと言ったら--　　--そう、それだ。それだよ。

//Dr. Langford steps forward, knocking Warren's hand from the keypad. He enters the code.//

ラングフォードが前に出て、キーボードからウォーレンの手を退ける。そのまま彼はコードを入力した。

**Dr. Langford:** Oh-seven-oh-four-one-seven. The date of Berryman's initial proposal.

**ラングフォード博士:** ゼロ、ナナ、ゼロ、ヨン、イチ、ナナ。ベリーマンの最初の発表の日です。

//A green light flashes, and the door opens. Langford gasps.//

緑の閃光が走った。ドアが開く。ラングフォードは息を呑んだ。

**Torres:** Ho-ly shit.

**トレス:** おいマジかよ。

**Warren:** I think we've found our source.

**ウォーレン:** 発生源とご対面だね。

//The door opens into an expansive, dark space, far larger than the entire building, let alone the domed chamber, should permit. On the other side of the doorway, a single glass canister rests atop a pedestal, set atop a platform with a circumference of 9 meters. Beyond this, the interior walls are non-existent. Instead, the area around the platform is a void of space, through which multiple iterations of the same platform can be seen. There is a clear pattern of void-space and platforms extending out as far as can be seen in all directions, both above and below the team's perspective. Langford moves as if to enter, and is halted by Nix.//

扉が開いた。その先には、暗い空間が広がっていた。このドーム状の部屋は言わずもがな、建物全体よりも大きいとも思えるくらい、途方もなく広い空間だ。扉をくぐれば、直径およそ9メートルのプラットフォームが見えてくる。その中央の台座には、ガラスのキャニスターがぽつんと置かれていた。その周囲には、ただ虚無が広がっている。その虚無の中に、同じプラットフォームが無数に浮かんでいる。見上げても、見下ろしても、その虚無はどこまでも続いている。そして、プラットフォームは規則正しく配置されている。見える限り全ての方向に、果てしなく広がっていた。ラングフォード博士がそこに足を踏み入れようとしたものの、ニクスがそれを制した。

//Torres draws his sidearm. As he moves to line up a shot, a voice is heard all about them.//

トレスがサイドアームを抜いた。その照準をキャニスターに合わせた瞬間、辺り一体から声が響いた。

[[div class="berryman"]]
[[span]]Dear, dear Doctor Langford. So you've come back to me.[[/span]]
[[/div]]


[[div class="berryman"]]
[[span]]ああ、我が親愛なるラングフォード博士。やっと戻ってきたのね。[[/span]]
[[/div]]

**Dr. Langford:** B-Berryman?

**ラングフォード博士:** ベ、ベリーマン？

//Nix is struck hard by an unseen force. She is sent flying, crashing into several canisters along the back wall. The gun in Torres' hand crumples, tearing off his left index finger. As he reels in pain, Warren is sent flying sideways, colliding with Torres.//

ニクスが不可視の力で激しく弾き飛ばされた。その体は後方の壁に並ぶキャニスターに叩きつけられて、ガラスが砕け散る。同時に、トレスの手中でサイドアームが潰されて、彼の左人差し指が根本から吹き飛ぶ。その痛みに身を捩るトレスに、今度は横から吹き飛ばされたウォーレンが激突した。

[[div class="berryman"]]
[[span]]In a sense, yes. It's me.[[/span]]
[[/div]]

[[div class="berryman"]]
[[span]]部分的には、そうね。私よ。[[/span]]
[[/div]]

**Dr. Langford:** Ava, please, stop! Whatever you're doing here, I'm begging you, it has to stop!

**ラングフォード博士:** 何やってんですこんなところで！　もういいじゃないですか！　こんなこと、頼むからやめてくださいよ！

[[div class="berryman"]]
[[span]]Please, come in. It's alright. I just want to talk.[[/span]]
[[/div]]

[[div class="berryman"]]
[[span]]こっち来てちょうだい。大丈夫。お話をするだけだから。[[/span]]
[[/div]]

//The door's threshold stretches -- the half-meter of space extending and being drawn into a long hallway. The space beyond becomes obscured by the presence of a spiraling light that shimmers with each word Dr. Berryman speaks. The visual transfixes Dr. Langford for several seconds. He then approaches it.//

扉口が引き伸ばされていく。わずか半メートルほどだった空間が、今や長い廊下へと変貌してしまった。その奥には、螺旋を描く光があった。ベリーマン博士が声を発するたび、その光は優美に明滅する。ラングフォード博士は、その光景に魅入られてしまった。わずか数秒間ほどではあったが、彼は身動きすら取れなかった。やがて彼は、その光に向かって歩き始めた。

**Nix:** Langford, don't!

**ニクス:** やめて！　ラングフォード！

//Dr. Langford does not respond and continues walking. Gravity shifts: he is lifted from the ground and pulled towards -- falls towards -- the void that contains the spiral. The visual field is subsumed by the fractal's intense coloration.//

ラングフォード博士は応答せず、そのまま歩き続けている。重力が変わった。彼は地面から浮き、光を湛える虚無の中へと引かれていく--　　--否、落ちていく。映像は、フラクタルに飲み込まれた。

[[div class="explo explo--threshold"]]

//Light fills the field of view as it enters a dense region of the fractal; the duration of Dr. Langford's fall is indeterminate.[[footnote]]Subsequent viewings of the footage vary from a few minutes to several hours, with a corresponding change to filesize[[/footnote]] After a moment, the image resolves, revealing that he is lying on the carpet in an ordinary office. It contains a desk and several portable whiteboards bearing equations. Late afternoon sunlight streams in through a window, casting long shadows.//

フラクタル密度の濃い領域に入ると、光が視界を埋め尽くした。ラングフォード博士の落下がどれだけ続いたかは、定かではない[[footnote]]この映像の再生時間は、再生のたびに変動する。その長さは数分から数時間であり、これに応じてファイルサイズも変化する。[[/footnote]]。やがて映像が鮮明になり、彼の姿が映し出される。ラングフォード博士は、普通のオフィスの絨毯の上に、横たわっていた。机があり、方程式の書かれた可動式ホワイトボードも数台置いてある。窓からは遅い午後の日差しが差し込み、室内に長い影を落としていた。

**Dr. Langford:** Am... am I dead?

**ラングフォード博士:** 死んだのか、僕は……？

**Dr. Berryman:** Don't be daft, my dear fellow.

**ベリーマン博士:** ほら、ボケっとしてないで。

//Dr. Langford rolls over. A cabinet to the side is covered with a dense collection of flower bouquets and a leafless bonsai tree, which Dr. Berryman is watering. She has a pink dahlia flower pinned to her hair and is wearing a knee-length sundress with a lace pattern that seems to change as she moves. She sighs, puts down her spray bottle, and retrieves her labcoat from her chair, putting it on.//

ラングフォード博士が身を起こした。その脇のキャビネットには、色とりどりの花束がぎっしりと飾られ、葉のない盆栽もひとつ置かれている。ベリーマン博士が霧吹きを吹いて、その盆栽に水を与えていた。彼女の髪にはピンクのダリアが挿してある。身に纏うのは膝丈のサンドレス。その微細なレース模様が、彼女の動きに合わせて微妙に変化して見える。彼女は小さくため息をついて、霧吹きを置くと、椅子にかけてあった白衣を手に取って、袖を通した。

**Dr. Langford:** Dr. Berryman, is it really you?

**ラングフォード博士:** ベリーマン博士、あなたなのですね。

//Dr. Berryman smiles, although her eyes remain downcast.//

ベリーマン博士は、伏し目がちに笑った。

**Dr. Berryman:** Rob…

**ベリーマン博士:** ロバート……

//She crouches and offers Dr. Langford a hand. Dr. Langford rebuffs it and recoils away from her. She takes his hand anyway and helps him up, and he does not resist.//

ベリーマン博士は屈んで、ラングフォード博士へ手を差し出す。ラングフォード博士はそれを即座に拒絶し、座ったまま後ずさった。ベリーマン博士はそれを気にすることなく手を差し出して彼を助け起こそうとする。ラングフォード博士は抵抗しない。

**Dr. Berryman:** It's been so long, Dr. Langford. I'm not sure you'd believe me, but I really did miss you all this time.

**ベリーマン博士:** 本当に久しぶり、ラングフォード博士。信じてくれるかはわからないんだけれど、私本当に寂しかったのよ。

**Dr. Langford:** I don't.

**ラングフォード博士:** 信じません。

//Dr. Berryman tucks some hair behind her ear.//

ベリーマン博士が髪をかきあげ、耳にかけた。

**Dr. Berryman:** I'm sorry to hear that, but I can't say it's unexpected. What finally motivated you to come pay me a visit after all these years?

**ベリーマン博士:** あら残念。でもいつかは来てくれるんじゃないかって思ってたのよ。それで、どうして今になってここに来ようと思ったわけ？

//Dr. Langford gestures around them, although there are no fractal anomalies visible in the office besides Dr. Berryman's dress.//

ラングフォード博士は周囲を指し示す。だがベリーマン博士のドレス以外に、異常なフラクタルは観察できない。

**Dr. Langford:** Look around, Berryman. You should know better than me.

**ラングフォード博士:** 周りを見てくださいよ。僕なんかよりもよくご存知でしょう。

**Dr. Berryman:** I really don't.

**ベリーマン博士:** わからないわ。本当に。

//Dr. Langford sighs.//

ラングフォード博士がため息を漏らす。

**Dr. Langford:** The Foundation considers your research methods unsound, Dr. Berryman.

**ラングフォード博士:** ベリーマン博士。あなたの手法は不健全だと、財団は思っています。

**Dr. Berryman:** And you?

**ベリーマン博士:** で、あなたは？

**Dr. Langford:** I-- I…can't disagree.

**ラングフォード博士:** その--　　--否定は……できません。

**Dr. Berryman:** May I remind you that you were instrumental in the genesis of many of these methods, Dr. Langford. Your name is as embedded as mine in everything we've done, everything happening now, I just… //expanded// on them. They are all //our// methods.

**ベリーマン博士:** ちょっと補足させてもらうけど、あなたもその手法とやらを作るには不可欠だったのよ、ラングフォード博士。あなたの名前も、我々の成果には深く刻まれているわ。私の名前と同じくらい、ね。私はただ、それらを発展させただけなの。結局、これって私たちの作った手法でしょ？

**Dr. Langford:** That may be true, but it's irrelevant. That is all in the past. And what your methods are now, are a threat to consensus reality.

**ラングフォード博士:** それはそうですが、この期に及んでそんなことないでしょう。あなたの手法は、合意現実への脅威となっているんですよ。

**Dr. Berryman:** Reality as determined by mere consensus… really, Rob? So unambitious for the research partner I knew. Perhaps reality is determined by something more fundamental, more objective. Your Scranton Reality Anchor had its own expert opinion on what is real.

**ベリーマン博士:** 合意とやらが、現実を決めている……ロバート、それ本気？　あなたのこと、もっと大胆な人だと思ってたのに。現実って、もっと根源的で、客観的な何かが決めてるって私は思うわ。あなたよりも、そのスクラントン現実錨の方が、現実についてよくわかってるんじゃないのかしら。

**Dr. Langford:** I don't think the ordinary people you kidnapped would agree with its assessment.

**ラングフォード博士:** あなたがここへ攫ってきた普通の人たちが、そのご意見に同意するとも思えません。

**Dr. Berryman:** Ordinary people have no assessment at all, the same lacking they had upon the development of gunpowder, or electricity, or the atom bomb. They will come to have one after it's explained, developed, and allowed to enter their lives. But you and I, that is our duty.

**ベリーマン博士:** 意見なんて持たないのよ。普通の人たちは。火薬が開発された時も、電気が発見された時も、原爆が作られた時も、全部同じだったでしょう？　全部が開発されて、解説されて、生活の一部になってからようやく、普通の人たちは「意見」を持つの。でも、あなたと私には義務がある。

**Dr. Langford:** What you are doing is not duty, it's madness.

**ラングフォード博士:** あなたのあれは狂気ですよ。義務なんかじゃない。

**Dr. Berryman:** Tell me, Dr. Langford, what have you been doing all these years?

**ベリーマン博士:** じゃ教えて、ラングフォード博士。今に至るまで、あなたはどんなことをしてきたの？

**Dr. Langford:** Averting those same ordinary people's eyes //from// harm, not towards it. //Containing// dangers, not unleashing them. Helping to //protect//, like our mission.

**ラングフォード博士:** 人々を守ることです。危険から遠ざけてやること。決して危険を押し付けるんじゃありません。脅威は収容するものです。解き放ってはいけないのですよ。我々の仕事ですよ。それが。普通の人を守ることが。

//Dr. Berryman shakes her head.//

ベリーマン博士が頭を横に振った。

**Dr. Berryman:** Such wasted potential. If I had estimated you for less, I wouldn't have invited you to join Project HYDRA in the first place. But you aren't the only one who's wasted so much time.

**ベリーマン博士:** 才能の無駄遣いね。私がここまであなたを買ってなかったら、そもそもHYDRA計画に誘うこともなかったのよ。とはいえ、あなたがこれほどに時間を空費してしまったのは、あなた1人の責任というわけでもないけれど。

//Dr. Berryman begins boiling some water in a kettle and preparing some drinks.//

ベリーマン博士はヤカンで水を沸かし、飲料を準備している。

**Dr. Berryman:** I… deeply regret how I treated you at times in the past, Dr. Langford. I of course thought of you as a contributor, but I did not realize the true extent of your value, your indispensability to this project, until after your departure. And if you'll allow me to say it, I want to say I'm sorry.

**ベリーマン博士:** ラングフォード博士……あなたをあんなふうに軽んじるべきじゃなかったって、本当に後悔しているわ。共同研究者としてもちろん、あなたのことは大切に思っていた。けれど、あなたの本当の価値に気づいたのは、あなたがかけがえの無い方だとわかったのは、あなたがここを離れてから。聞き苦しいでしょうけど、謝らせてくれるかしら。

//Dr. Langford says nothing.//

ラングフォード博士は何も言わない。

**Dr. Berryman:** I will admit I was arrogant. I always understood more of what you did than what you did of mine. When we talked about our A-levels once, you freely admitted you thought me the more intelligent one. It was always my insights that progressed Project NIETZSCHE -- until it turned out that you solved the problem in secret, of course.

**ベリーマン博士:** 認めなければならないわ。私が傲慢だったことを。私にはあなたの研究が全部お見通しで、あなたは私の研究の表面しか理解していないと。かつてAレベルについてお話をした時、あなたよりも私の方が賢いのだと、あなたはいとも簡単に認めた。私の洞察こそが、NIETZSCHE計画を進めていたのだと、そう思っていたわ。それも、あなたがこっそりと問題を解決してしまったとわかった時に、崩れてしまったの。

**Dr. Langford:** I had to draw a line in the sand; I saw an opportunity to stop more deaths, and I took--

**ラングフォード博士:** ここまでという境界線を引くしかありませんでした。これ以上死人を出さないようにする好機だと思って、ぼくは--　　--

**Dr. Berryman:** I'm really sorry, Rob. I should have listened to you, valued you more. I truly, honestly believed that with you out of the picture and your hidden research finally in my hands, that I could complete it all myself. For a decade I tried everything, anything.

**ベリーマン博士:** 本当にごめんなさい、ロバート。あなたともっとちゃんとお話をして、あなたをもっと大事にするべきだったわ。あなたがいなくなった後、あなたが秘密裏に進めていたものがようやく私のところに戻ってきたと、私が自分でこれを完成させるんだと、そう思ったの。そこから十年ほど、取れる手は全部取ったわ。

**Dr. Langford:** But you couldn't, could you? One single data point from the algorithm wasn't enough. You needed to be able to reproduce it. You needed the fractal equation.

**ラングフォード博士:** でも完成しなかった。そうでしょう？　アルゴリズムの中で見つかった、ただひとつのデータポイントじゃ、あなたは満足しません。それを再生産するには、フラクタル方程式が要ります。

**Dr. Berryman:** Perhaps I was never as opaque to you as I might have thought. You're right of course. I was desperate. I saw opportunity, too, and I took it whenever I could, no matter how questionable its source.

**ベリーマン博士:** もしかするとあなたの方が、私をお見通しだったのかもね。そう、あなたの言うとおり。私は必死だった。私も好機を見つけたのよ。それでとにかくそれを掴もうとした。たとえそれがどんなに胡乱なものでも。

**Dr. Langford:** And that's how you fucked up the Site.

**ラングフォード博士:** それで、あなたはこのサイトをめちゃくちゃにしたんですね。

**Dr. Berryman:** It wasn't the intention, at least at first. The results were promising. I was finally starting to affect a reality bender's mind with Perseus, but when you use a fractal cognitohazard to scramble the mind of a reality bender, it turns out that you start to scramble reality itself.

**ベリーマン博士:** そうしようと思ったわけじゃないのよ。少なくとも最初は。結果も上々だったのよ。ペルセウスを使って、ようやく現実改変者に影響を及ぼせるようになった。でもフラクタル的認識災害で現実改変者の精神を混ぜっ返すと、現実そのものがぐちゃぐちゃになるみたい。

**Dr. Langford:** And this wasn't a sign to you to stop?

**ラングフォード博士:** それで、止めようとは思わなかったんです？

**Dr. Berryman:** One small impediment could never make me give up, not this close to the success of the project. To do so would be surrender by the Foundation to the anomalous, a concession to the incomprehensible, a betrayal of our philosophy and mission. I tried whatever I could, of course. More CT scans, more algorithms, more analytic functions. I fed the problem as many D-class as I could obtain… and then some. I stared at infinity as hard as I could for over ten years, I tried everything to reach out and touch it, in the process I even //became// a part of it. We attacked the problem so relentlessly that it expelled the fractals from their pages and their screens until they twisted the walls, the air, //me//. I could see them unfold before me like a wave, I could feel myself carried by them, I could even hear them sing their repetitious, yet crescendoing, song. I felt like I could finally walk that forbidden landscape myself and pick out ordinary fractal cognitohazards like shells and starfish from a battered shore, like I had become your algorithm. Yet there was still one prize beyond my reach. Always, //always// beyond my reach. Even after going this far, consequences be damned. Even after sacrificing everything, even myself, maybe even the world, until there was nothing left to offer: the solution to Project NIETZSCHE.

**ベリーマン博士:** 諦められるわけないでしょう。計画の成功を目の前にして、そんな些事なんか気にしてられないわ。そんなことしたら、財団が異常存在に白旗を上げることになるのよ。理解不能なものに対して屈服すること--　　--それって我々の使命への背信じゃない。だからなんでもやったわ。CTスキャン、アルゴリズム、解析関数……手に入る限りのDクラスを注ぎ込んだ。でも、それだけじゃ足りなくなったの。私はこの10年間、無限をずっと見つめていた。そこに手を伸ばして、掴もうとして……その果てに、私は無限に取り込まれてしまった。そうやって真剣に問題と向き合っているうちに、フラクタルが画面から溢れてきて、壁を捻じ曲げて、空気を歪めて、私自身すらも変えてしまった。それは目の前で波打ちながら広がって、私もその波に乗って、あの歌を聞かせてくれた。同じメロディーを繰り返しながら、だんだん高く、大きくなっていって……ついに向こう側で歩けるようになったの。禁じられた世界の中で、まるで波打ち際で貝殻とかヒトデとかを拾うみたいに、フラクタル的認識災害を集められるようになったの。あなたのアルゴリズムそのものになれたような気がしたわ。でも、それでもダメっだった。どんな犠牲を払っても、自分がどこかにいなくなっても、世界を危険に晒しても、失うものすら全部なくなっても、NIETZSCHE計画の答えだけは、どうしても……どうしても手に入らなかった。

//Dr. Berryman's shoulders crumple.//

ベリーマン博士の肩がすくむ。

**Dr. Berryman:** How, how, how is it possible? What's so damned //special// about reality benders? Why won't they just //obey// the rules everyone else follows? The rules everyone else //must// follow?

**ベリーマン博士:** どうしてそんなことが許されるの？　現実改変者の何がそんなに特別なの？　なんで黙ってルールに従ってくれないの？　彼ら以外が全て従わなくちゃならないルールなのに？

//She buries her face in her hands.//

ベリーマン博士は、手で顔を覆った。

**Dr. Berryman:** Of course I still firmly believe all anomalies have structure. But some are so complicated that they only reveal themselves to those with the right training, the right technical expertise, and more than that, the right insight. Non-universality of human experience is the one universal. At the end of all my efforts I finally came to the conclusion I had avoided all along: I couldn't replace you. My team couldn't replace you. My only recourse… is you.

**ベリーマン博士:** 全ての異常には仕組みがあるはずだと、今も確信してる。ただ、世の中には例外というものがあるのね。あまりに複雑で、選ばれた人にしか理解できないもの。訓練も、知識も、それだけでは足りない。生まれ持った洞察力が必要なものが。経験の非普遍性こそが普遍的なものだとしたら、あなたには私に見えないものが見えている。散々努力した挙句、私は結局現実を受け入れるしかなくなってしまったの。あなたの代わりはいない。私ではダメだったの。どんなチームを君でも、あなた1人には叶わなかった。結局のところ……あなたに頼るしかないのよ。

**Dr. Langford:** And what makes you think I'll help you this time?

**ラングフォード博士:** 今度はぼくがあなたの助けになると、どうしてそう思うのです？

//Dr. Berryman pours out the hot water into two cups: one for coffee with a melted piece of Cadbury chocolate and half a creamer pod, and one for Earl Grey tea with a squeezed lemon and three squeezes of honey. She walks over and places the teacup and saucer in Dr. Langford's hands, then sits on the edge of her desk next to him. She wraps her hands around the coffee cup, staring into it, and sighs.//

ベリーマン博士は熱湯を2つのカップへと注いだ。片方はキャドバリー・チョコを溶かし入れて、コーヒーフレッシュを半分だけ入れたコーヒー。もう片方はレモンを絞り、ハチミツをたっぷり垂らしたアール・グレイ。彼女はそれを持ってラングフォード博士のもとへ歩み寄ると、彼にティーカップとソーサーを手渡す。すぐ横のデスクへベリーマン博士が腰をかけて、コーヒーカップを両手で包みこんだ。彼女はその中を覗き込んで、ため息をついた。

**Dr. Berryman:** It wasn't all bad, was it, Rob?

**ベリーマン博士:** 悪い思い出ばかりじゃなかったでしょ、ロバート。

//Dust suspended in the sunlit air begins to curl into loose fractal patterns.//

空気の中で踊る埃が、太陽の光で照らされた。それは曖昧なフラクタル図形を描いている。

**Dr. Berryman:** You had many opportunities to leave the project. Yet every day you showed up to the lab, or to this office, and put your head together with mine, sometimes into the early hours of the morning, to work on these problems. Why?

**ベリーマン博士:** 計画から抜けようと思えば、あなたはいつでも抜けられた。でも、毎日研究室か、このオフィスに来てくれて、問題を解決するために、一緒に知恵を出し合った。早朝に来てくれたこともあったわね。それはどうして？

//Dr. Langford looks up at Dr. Berryman, but does not answer. Dr. Berryman picks up a stack of documents from her desk, and begins handing them to Dr. Langford one at a time. Each is a scientific paper beginning with "Ava Berryman, Robert Langford".//

ラングフォード博士はベリーマン博士を見上げた。だが、彼は答えなかった。彼女はデスクから書類をいくらか取り、それをラングフォード博士へ1部ずつ手渡していく。科学論文だ。それぞれの頭には「エイヴァ・ベリーマン、ロバート・ラングフォード」の文字がある。

**Dr. Berryman:** When I was younger, I would occasionally receive a silly mailer about "buying" a star for someone. Or when I first visited Paris, I saw the silly tradition of lovers engraving their names on locks and putting them in monumental places. But we have something far deeper than friendly pub stories or fleeting neurochemical nonsense. Our names are intertwined and stamped, weaved into something more fundamental than reality itself, more fundamental than the noosphere, something that existed before everything and will exist after its end. Something unbreakable and eternal. Friends fall out, families estrange, couples divorce, but us? There may be interruptions, long ones even, but in the end we will work together for as long as a fractal continues. Because that is what we are now: the Berryman-Langford set.

**ベリーマン博士:** 私たちの名前はね、絡みあって、ここに刻まれているのよ。現実そのものよりもさらに奥深くに、ノウアスフィアのさらにその下に。何もかもが存在する前からあって、何もかもが滅んだ後にも残るものに。まだ若かった頃ね、「星に誰かの名前をつけませんか」って馬鹿みたいなダイレクトメールを受け取ったことがあるわ。パリに初めて行った時も、恋人たちが名前の刻まれた錠前を橋なんかに引っ掛けるみたいな、馬鹿みたいな風習もあるじゃない。そんな御涙頂戴の居酒屋ばなしとか、脳内物質のもたらす一時の気の迷いとか、そんなものとはまるっきりレベルが違うの。友人はいずれ仲違いするし、家族ともいつか疎遠になる。恋人もいつかは別れるわ。でも私たちは違う。長いすれ違いもあったかもしれないけれど、フラクタルのあるかぎり、結局私たちは一緒に研究することになる。私たちは今や、ベリーマン=ラングフォード集合そのものなのだから……。

//Dr. Berryman writes an equation on the margin of one of the papers.//

ベリーマン博士が、論文の余白に方程式を書き込む。

[[math]]
z_{n+1} = z_n - \eta\frac{f(z_n)}{f'(z_n)} + c
[[/math]]

**Dr. Berryman:** It's that simple. It's taken me so long, but I've taken us as far as I can, Dr. Langford. The end of all these years, all these sacrifices, all this pain, it finally ends with just these three tiny parameters [[$ f, c, $]] and [[$ \eta $]]. The solution to Project NIETZSCHE is an impossibly distant galaxy for me alone, but for you it's at the tips of your fingers.

**ベリーマン博士:** たったこれだけなの。こんなに時間をかけて、私なりに精一杯やって、ようやくここまで来たのよ、ラングフォード博士。あらゆる犠牲も、耐え難い苦痛も、最後には結局、たった3つの変数に収まってしまう。[[$ f $]]と[[$ c $]]と[[$ eta $]]、たったこれだけなんだから。私にとってのNIETZSCHE計画の答えというものは、遥か遠くの銀河。でもあなたにとっては、手を伸ばせば届くようなものだったのでしょう。

//Dr. Langford takes a deep breath. Dr. Berryman smiles.//

ラングフォード博士が深いため息をついた。ベリーマン博士は笑顔を浮かべる。

**Dr. Berryman:** You're always so thoughtful. You always hesitate at first, but in the end, with enough encouragement, you come around to the right answer. At first I had resented this trait, but in the end, I have come to realize that same thoughtfulness is part of your value. It's what I need to solve this problem. So please, Rob.

**ベリーマン博士:** あなたはいつも思いやりに溢れていた。いつも最初にためらって、でも最後には勇気を以て正しい答えを掴み取る。最初の頃こそは鬱陶しかったけど、あなたなりによく考えてくれているってことがようやくわかったの。これもあなたの長所で、問題を解決するのに必要なんだって。だからね、ロバート……。

**Dr. Langford:** I'm so sorry, Ava.

**ラングフォード博士:** エイヴァ、ぼくは本当に後悔しています。

//Dr. Berryman raises an eyebrow.//

ベリーマン博士が片眉を上げた。

**Dr. Langford:** I'm so sorry for leaving you alone like this, struggling alone against an impossible problem in the face of all odds. Your tenacity is something I've always admired about you, but even for someone like you, doing it for this long must have been so hard for you. You must be so tired.

**ラングフォード博士:** あなたを1人でここに置いてきたことを、ぼくは本当に後悔しています。確かにあなたは強固な意志をお持ちです。ぼくもそれを尊敬しています。ですがこんな絶体絶命の中、こんな無理難題に1人で、しかもこれほどの長い時間向き合う……いくらあなたでも、難しいことだと思います。とてもお疲れでしょう。あなたも。

**Dr. Berryman:** … I am.

**ベリーマン博士:** ええ。

**Dr. Langford:** But you won't stop.

**ラングフォード博士:** でも止まらないんでしょう。あなたは。

**Dr. Berryman:** I can't, Rob. You know that.

**ベリーマン博士:** 止まれないのよ。わかるでしょ、ロバート。

//Dr. Langford sighs. He rolls his neck, surveying the room. There is no door.//

ラングフォード博士はため息をついた。彼は部屋のあちこちを見渡した。どこにも扉がない。

**Dr. Langford:** You're completely right, you know. You know me too well. Of course you must, given all the time we spent together here. I hesitate. I'm unsure. I really did not know what I would think or do when I finally found you, if I even would. But like you said, thanks to your help, I do now.

**ラングフォード博士:** そうですね、その通りです。あなたはぼくのことをよくお分かりだ。我々がここでともに過ごした時間を考えれば、それも当然でしょう。ぼくは躊躇うし、いつも迷ってばかりなんですよ。もしこうやってあなたを見つけた時、ぼくは何をすればいいのかずっとわからなかったんです。でも、今ようやくわかりました。あなたがぼくに気づかせてくれたんです。

**Dr. Berryman:** Thank you, Dr.--

**ベリーマン博士:** ありがとう、ラングフォ--　　--

//Dr. Langford pulls Dr. Berryman into a hug. Dr. Berryman reacts in surprise, not reciprocating.//

ラングフォード博士は、ベリーマン博士の体を引き寄せて、彼女を抱きしめた。ベリーマン博士は驚きの表情を浮かべながらも、抱擁を返さない。

**Dr. Langford:** I was so selfish. I'm so sorry my actions allowed this to happen to you for so many years. I'm sorry I wasn't there for you when you needed me. I'm sorry I can't fix it.

**ラングフォード博士:** ぼくは身勝手でした。ここから逃げたしたせいで、あなたに全てを背負わせてしまったんです。ずっと長い間、こんなにも。あなたが一番辛い時に、ぼくは居なかった。取り返しなんかつくわけないですよ。本当に……ごめんなさい。

//Dr. Berryman hesitates, then hugs Dr. Langford back.//

ベリーマン博士は躊躇いがちに、ラングフォードに抱擁を返した。

**Dr. Berryman:** It's okay. Time itself is a fractal here. Sit down and work with me, and we have a chance to start over.

**ベリーマン博士:** いいのよ。ここでは、時間そのものもフラクタルだから。一緒に働きましょう。やり直すチャンスなら、いくらでもあるわ。

//Dr. Langford pulls away. He picks up the research paper with Dr. Berryman's handwritten equation on it. He picks up a pen and begins writing --//

2人は抱擁を解いた。ラングフォード博士は論文を手に取った。ベリーマン博士の手書きの方程式が書かれているものだ。彼はペンを手に取り、何かを書きはじめる--　　--

[[math]]
{f(z)} =
[[/math]]

//-- but he finds himself crying. He looks up and regards Dr. Berryman's face.//

彼は、自分が泣いていることに気づいた。顔を上げて、ベリーマン博士の様子を見る。

**Dr. Langford:** Thank you, Dr. Berryman. I've finally made up my mind. I will serve the Foundation, as I should have done all those years ago.

**ラングフォード博士:** ありがとう、ベリーマン博士。ようやく心が決まりました。ぼくは財団に忠を尽くします。本当なら、何年も前に決めるべきだったのでしょうが。

//Dr. Berryman smiles.//

ベリーマン博士が笑顔を浮かべた。

**Dr. Langford:** We will finish Project NIETZSCHE, once and for all.

**ラングフォード博士:** 終わらせます。NIETZSCHE計画を。これっきりで。

//Dr. Langford grabs Dr. Berryman's laptop, hurls it through the window, and jumps out amidst the fractal-edged glass shards.//

ラングフォード博士は、ベリーマン博士のノートPCをつかみ、窓へと投げつけた。フラクタルの形に散った窓を乗り越えて、そのまま彼は外に飛び出ていく。

**Dr. Berryman:** Dr. Langford!

**ベリーマン博士:** ラングフォード博士！

//Dr. Berryman reaches out to him, although does not pursue. The space outside the office shimmers and dissolves -- revealing that Dr. Langford is still falling into the Berryman fractal.//

ベリーマン博士は手を伸ばした。だが追いはしない。オフィス外の空間は、燐光を発しながら解けてゆく。ラングフォード博士は、ベリーマン・フラクタルの中で落ち続けている。

[[/div]]

[[div class="berryman"]]
[[span]]I thought you might listen to reason. No matter.[[/span]]
[[/div]]

[[div class="berryman"]]
[[span]]理性的な話し合いができると思っていたのに。でももういいわ。[[/span]]
[[/div]]

//The facility around them rumbles.//

周囲の施設が振動する。

[[div class="berryman"]]
[[span]]You'll come to see things my way. We've all the time in the world, after all--[[/span]]
[[/div]]

[[div class="berryman"]]
[[span]]でもそのうち私と同じ結論に至るわ。何せ永遠に時間があるのだから--　　--[[/span]]
[[/div]]

//A gunshot rings out. There is a shattering of glass. The Berryman spiral sputters and vanishes with a deafening shriek, dropping Dr. Langford to the ground. He begins to scramble backwards from the Perseus chamber.//

銃声。ガラスの割れる音。ベリーマンの螺旋はバチンと音を立てながら消失した。けたたましい金切り音とともに、ラングフォード博士が地面に落ちる。彼は這いながらペルセウス室から遠ざかる。

//The canister hosting Subject Perseus has been shattered. There is a bloodied hole in the center of the subject's head. Looking back, Dr. Langford can see that Torres is propped up on the ground in the middle of the room, a bloodied hand shaking as he drops Warren's pistol. As the weapon hits the ground, Torres is wrenched sharply up into the air. He is instantly and effortlessly bisected -- his top and bottom halves collapse in a heap. With blood pooling about his severed waist, he withdraws a slender device from a breast pocket. With a shaking hand, clicks open its cap, and presses the exposed button. At last his hand falls, and he moves no more.//

ペルセウス対象を納めていたキャニスターは砕かれた。対象の頭部には、血の滲む穴が開いている。振り返ると、ラングフォード博士の目に映ったのは、地面に手をついているトレスの姿であった。彼は血まみれの手を震わせながら、ウォーレンの拳銃を取り落とした。銃が地面に落ちたその瞬間、トレスの体が勢いよく宙に引き上げられた。一瞬で、何の抵抗もできずに、彼は真っ二つに切断された。上半身と下半身が泣き別れになって、ドサリと地面に落ちた。腹部から血があふれる中、彼は胸ポケットから細長い装置を取り出す。彼は手を震わせながら、蓋を開き、露出したボタンを押した。やがて腕が力なく垂れ下がり、トレスは動かなくなった。

//Berryman's voice continues to shriek. Louder. Angrier. The spiral reappears in the Perseus chamber. Glass canisters all about the room shudder, and are pulled from their alcoves. Dr. Langford is swiftly and harshly pulled back towards the chamber. He barely manages to grasp the door's threshold as bits of paper and smaller materials whiz by.//

ベリーマンの声は甲高く、より大きくなっていく。その中に怒りが滲み出る。ペルセウス室の中に螺旋が再び現れる。部屋中のガラスキャニスターが震え、壁龕から引きずり出されてゆく。何かの力が、ラングフォード博士に有無を言わせることなく彼を部屋の中へと引きずり込んだ。書類の切れ端や小物が次から次へ飛び交う中、彼はかろうじて扉の敷居に捕まった。

[[div class="berryman berryman--angrier"]]
[[span]]You no longer have a choice, Robert. You will submit.[[/span]]
[[/div]]

[[div class="berryman berryman--angrier"]]
[[span]]あなたに選択肢はないのよ、ロバート。服従しなさい。[[/span]]
[[/div]]

//Dr. Langford strains to maintain his grasp on the threshold, ducking his head down as the pieces of Torres sail overhead and into the maw of the spiral. Nix can be seen in the distance, her rucksack caught on a metallic arm on the perimeter of the Kempelen facility. Warren is desperately clinging to the corner of Berryman's desk as it is slowly pulled in.//

ラングフォード博士は低く伏せながら、螺旋の中に吸い込まれまいと必死に踏ん張った。トレスの体の一部が、彼の頭上を舞い踊り、そのまま螺旋へと吸い込まれていく。遠方にはニクスの姿もあった。彼女のリュックがケンペレン施設端の金属アームに引っかかっているようだ。ゆっくりと引き込まれていくベリーマンの机の角に、ウォーレンはしがみついている。

[[div class="berryman berryman--angrier"]]
[[span]]You do want to play in the big leagues, don't you?[[/span]]
[[/div]]

[[div class="berryman berryman--angrier"]]
[[span]]大舞台に出るんでしょ。そうしたいと言ったのはあなたよね。[[/span]]
[[/div]]

//The air rushing past increases in intensity. A finger slips. A second. Dr. Langford looks up, just past the threshold. His left hand fully loses grip.//

風が強まる。指が滑る。一秒。ラングフォード博士は仰ぎ見た。敷居をまたいでしまう。彼の左手が、外れる。

[[div class="berryman berryman--angrier"]]
[[span]]This. Is. Your. Chance.[[/span]]
[[/div]]

[[div class="berryman berryman--angrier"]]
[[span]]これが、あなたの、チャンスなのよ。[[/span]]
[[/div]]

//Straining with all his might, Dr. Langford pulls against the gale-wind force. His free hand grasps just beyond the edge of the threshold. He clasps the emergency pull cord.//

暴風のような力の中、ラングフォード博士は全力で足掻く。彼は空いた手を敷居の向こう側へと必死に伸ばす。そして、彼はプルコードを掴んだ。

**Dr. Langford:** Ha! Get real!

**ラングフォード博士:** 食らえっ！　これが現実だあっ！

//He pulls. As the SRAs come online, he is dropped hard to the ground. The winds cease. The Berryman spiral howls in pain.//

コードを引く。現実錨が起動する。ラングフォード博士は地面に強く打ち付けられた。風が止む。ベリーマン螺旋は苦痛に悶えた。

//Looking into the chamber, the interior space is seen to glisten and ripple. The far-distant copies of the interior begin to fall away into darkness as the space collapses within itself. The Berryman spiral is seen to twirl violently, losing complexity, taking on physical form.//

室内を覗き込めば、内部空間がきらめき、波打っていることがわかる。遠方に見える無数の部屋が、次々と暗闇へ落ちていく。空間自体が、圧壊している。ベリーマン螺旋が激しく回転し、複雑性を失い、物理的な形を取り始める。

//The facility quakes with a mighty rumble as Berryman manifests in three-dimensional space. Her body is contorted, sporting numerous, branching limbs. Her faces are contorted in pain. There comes a series of sickening squelches as Berryman's limbs, in turn, crunch and snap and flatten, beginning at their terminus and working towards her torso. Her many mouths wail as her heads, too, bind together into a single layer.//

轟音とともに、施設が激しく揺れた。ベリーマンが三次元空間に姿を現す。その歪んだ体から、無数の腕が枝分かれしながら伸び、またいくつもの顔が苦痛に歪んでいる。何かの潰れる、水っぽい不快な音がした。彼女の腕は末端から順に潰れていき、折れ、平らになっていく。じきに胴体も潰れていった。複数の頭部も、平面の中へと押し込まれていく。無数の口が悲鳴を上げている。

//Nix and Warren arrive at a stunned Langford's side. The three stare on as the Perseus chamber regains its walls, aligning with its natural state. Berryman's body is splayed against the interior wall as if superimposed as a 2d image. She continues to scream as all parts of her body at once are drawn to a singular point in their middle. She is rendered a single, shrieking point. With a {{pop}}, the point vanishes into non-existence. Her wailing does not cease.[[footnote]]Review of this footage would verify that despite a supposed continuation of Dr. Berryman's sustained vocalization, said vocalization does not in actuality exist. Dr. Berryman, at this point in time, does not verifiably exist.[[/footnote]]//

呆然とするラングフォードの元にニクスとウォーレンが駆け寄った。3人は、ペルセウス室が通常の部屋に戻っていく。ベリーマンの身体が、まるで2次元の画像か何かのように、その内壁に張り付いていた。彼女は叫び続けている。その体のすべてが中央の一点へと引き寄せられていく。やがて彼女はただの点になった。ポン、という音とともにそれが消えてもなお、叫び声は止まらなかった。[[footnote]]この映像の検証段階においては、ベリーマン博士の持続的な発声が継続しているとされるにも関わらず、実際にはそのような発声は存在していないことが確認される。この時点において、ベリーマン博士は存在していない。[[/footnote]]

//The area continues to quake and tremble.//

この領域は、振動し続けている。

**Nix:** Langford -- turn away. We've got to get out, now -- Torres called in the strike! We've got two minutes until this place is hot plasma!

**ニクス:** こっちだラングフォード。早く逃げるよ。トレスが爆撃を要請した。あと2分でここは火の海だ！

//Dr. Langford nods, and the trio rushes out towards the SCP-9001 production center. They rapidly scramble over Coleman's remains, and head into the antechamber where Nix had set down a Piton. There is a **{{beep}}** as they approach, and the space above the device crackles with energy. One by one, they pass through.//

ラングフォード博士はうなずいた。3人はSCP-9001生成センターへと急ぐ。コールマンの死体を乗り越え、控え室へと向かう。ニクスによって、あらかじめペグが設置されている部屋だ。控えめなブザーの音が鳴った。マーテル式ペグを挟んだ向こう側の空間が、何かのエネルギーによってゆがめられた。一人ずつ、そこを抜けていく。

**{{zip}}**
[[/div]]

//Nix, Warren, and Dr. Langford each appear in turn in the space just before the crematorium. The long hallway before them is filled to capacity by the massive frame of the abomination. Fresh heads flower from the mouths of its many faces as they take notice of the team's arrival.//

ニクス、ウォーレン、そしてラングフォード博士は、火葬場の目の前に出た。すぐそばの長い廊下を、悍ましいものが埋めていた。夥しい数の頭、そのそれぞれの口からまた頭が生えている。それが、3名の到着に気づいた。

**{{zip}}**
[[/div]]

//The three are back within the fog-laden server room. Fleshy strands of mycelium extend from the remains of the withered trunks, whipping senselessly all about the area. A single instance across the room slowly rears back up. Its orifice widens, bulb swelling.//

霧中のサーバールームへと戻る。枯れ果てた幹から伸びる菌糸じみた糸が、至る所で無為に垂れ下がっていた。部屋の向こう側、幹のうち一本が背を向けたまま立ち上がった。その開口部が広がり、球根が膨らむ。

**{{zip}}**
[[/div]]

//They've reappeared back at the tram platform where the video had begun, far outside the bounds of Site Romero-5. Distant tremors cause more cracks to form along the chamber's facade. Without a word, they make a break for the stairs.//

そして、3名はサイト・ロメロ-5の遙か外側、トラム駅へとたどり着いた。動画の開始地点と同じ場所だ。遠く離れたところから地鳴りが伝わってきて、壁面にヒビが入っていく。特に言葉を交わすことなく、3名は階段へと向かった。

//Emerging through the tunnel that obscures the tram's entrance, Dr. Langford collapses. The sky is alight with fire as the woods all about Site Romero-5 burn in the night. There is a flash across the sky. Streaks of light descend from the air -- the shockwave hits them next, arriving with a deafening **{{boom}}** as a heavy cloud of dust and wind sweeps the area, knocking all to the ground with its force.//

トラムの入り口を隠していたトンネルから出るや否や、ラングフォード博士が倒れ込んだ。夜空が炎に照らされている。サイト・ロメロ-5周囲の森林がもえあがっているのだ。空に閃光が走る。光の筋が空から落ちてくる。そのとき、衝撃波がかれらを襲った。耳を聾するほどの爆音とともに、濃い砂塵嵐が一帯を覆った。全員が地面に倒れ伏した。

//The trio watch on as the shadowy towers of the distant site are seen to crumble into the earth. It is Warren who speaks up first.//

遠くで霞むサイトの塔が崩れて地に落ちる。3名がそれを見ているさなか、ウォーレンが沈黙を破った。

**Warren:** "Get real"?

**ウォーレン:** 『食らえ、これが現実だ』か？

**Dr. Langford:** I... I thought it was clever.

**ラングフォード博士:** その……なんか言わなきゃって思って……。

//The three share a laugh as the approaching sound of wheels draws near.//

3人が笑い合うなか、タイヤの音が近づいてくる。

[[/div]]
[[/div]] [!-- .explo-root --]

The surviving members of the task force were picked up by an MTF Iota-10 patrol and returned to FOB Panloque. Following a delivery of footage and recovered assets, including the extracted SCP-9001, the three were debriefed and allowed rest.

当該機動部隊の生存者は機動部隊イオタ-10の巡回隊によって回収され、前線基地パンロケへ帰還しました。施設より抽出されたSCP-9001を含む回収された各種資産と映像記録の提出後、3名は事情聴取を受け、休養を許可されました。

[[include component:image-block name=http://scp-wiki.wikidot.com/local--files/scp-9001/planethand.webp|caption=SCP-9001-A残骸を含む地割れ|width=300px]]

Due to the combination of sustained orbital bombardment and seismic activity caused by the collapse of unstable spacetime in the site's subterranean sectors, Site Romero-5 would collapse into the earth, forming a massive fissure. MTF [[span class="hoverlink"]][[[task-forces#gamma-5|Gamma-5]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Gamma-5 ("Red Herrings")[[/span]][[span class="hoverlink-text"]]Specialists in disinformation tactics and amnestic dispersal dedicated to preventing mass knowledge of anomalous events.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Gamma5.png/small.jpg)"]]-[[/span]][[/span]][[/span]] was tasked with manufacturing a verifiable history and public record of the fissure, including the retroactive forging of geological, stratifical, and archeological studies that were each seeded with Third Order FCI designed to compel disinterest.

継続した軌道爆撃、およびサイト地下セクターにおける不安定時空による地震により、サイト・ロメロ-5はほどなく倒壊し、巨大な地割れを形成しました。機動部隊[[span class="hoverlink"]][[[task-forces#gamma-5|ガンマ-5]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Gamma-5 ("燻製ニシンの虚偽")[[/span]][[span class="hoverlink-text"]]異常な事象が周知されることを防ぐための、誤情報拡散および記憶処理実施におけるスペシャリスト集団。[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Gamma5.png/small.jpg)"]]-[[/span]][[/span]][[/span]]は、この地割れに関する検証可能な歴史と公的記録のねつ造を任務として割り当てられました。これには、地質学、地層学、考古学的研究の遡及的偽造も含まれており、それらの研究には、それぞれ無関心を強制するよう設計された第3級FCIが仕込まれています。

Hume readings of the area would return to baseline over the course of 48 hours. Cleanup measures would begin in earnest on 2025/08/13 under the direction of Doctor Leary.

48時間の経過後、当該地域のヒューム値は標準値へ戻りました。事後処理は2025/08/13より、レーリー博士の指示の下で実施されます。

**補遺 - 回収された文書:**

During exploration of SCP-9001-A, the Task Force would acquire reams of research data and logs, including topographical analysis of the BL set which indicates regions of high-activity and delineating "dead" regions, shipping manifests outlining the transfer of D-Class personnel between 2019-2025, and handwritten notes authored by Dr. Ava Berryman. These have been transcribed and are reproduced below.

SCP-9001-Aの探索中、機動部隊は大量の研究データとログを回収しました。これには高活性領域と失活領域のを示すベリーマン=ラングフォード集合のトポロジカル分析、2019年から2025年にかけてのDクラス職員移送を概説した輸送記録、およびエイヴァ・ベリーマン博士による手書きメモが含まれます。これらは転写され、以下に記録されています。

[[div class="blockquote"]]
//[NOTE:] This page is torn and the top half is missing.//

[補足:] このページは破られており、上半分の行方はわかっていない。

//[...]// obviously insufficient. I'm not going to be able to keep up with demand if my Berries keep rotting on the vine. The solution helps, but all it does is keep them alive. Immortality is of no use if their minds are flayed and atrophied. Whatever effects the active regions instill -- they're not simply wiped away by rebirth. The research is no good if I don't have a fresh supply.

[……]は明らかに不足している。もし蔓に生っている「苺」がこれ以上爛熟するのであれば、需要に応えることはできなくなってしまう。例の溶液は確かによく効いている。だが、それはせいぜい被験体の生命維持くらいにしか役に立ってはくれない。精神に強い負担がかかって崩壊してしまっているならば、不死など無用の長物に過ぎない。認識災害を受けたことによる影響は、たとえ一度死んで復活したとしても幾らかは残り続ける。新鮮な供給がなければ、研究を進めることができない。

Worse-still, we may need to flush our oldest subjects. Peculiar habit of moving their lips whenever someone is present in the facility. Starting to get under people's skin. It's childish, really. A bit asinine. These are grown men and women who can spend eight hours a day, six days a week beside a bank of severed human heads, but they're spooked by involuntary muscle movement?

さらに悪いことに、最古参の被験体をいくらか処分する必要がありそうだ。施設に誰かがいるとき、それらはいつも唇を動かすという、奇妙な癖を身につけてしまった。職員たちも苛立ち始めている。実に幼稚で、馬鹿らしいとさえいえる。職員各位は1日8時間、週6日、人の生首の側で過ごすことができる成人男女なのだ。それが不随意な筋肉の運動に怯えるとは。

At least Perseus continues to bear fruit. Its eyes have glazed over like some of the old-timers, but it continues to be receptive to fresh FCI. All these years and its mind resists deterioration. Not that its mind will be of much use if it's blinded. Frustrating to think of what could be accomplished were we able to have even a second Bender. Alas.

少なくとも、ペルセウスは成果を出し続けている。古参被験体と同じく目は虚ろになっているが、新しいFCIに対する反応は維持している。これほど長年にわたって精神の劣化に抵抗し続けているとは驚きだ。もっとも、目が見えなくなってしまえば、その精神もあまり役には立たないだろうが。もう一体でも現実改変者がいれば何かできたかと思うと、実にもどかしく思えてくる。

I feel a migraine coming on.

頭痛がする。

[[/div]]

[[div class="blockquote"]]
Commotion today. Units B-17, H-47, and K-43 showed unusual fMRI readouts. Beckett, fool that he is, suggested that we might have stumbled on a new First Order, stupidly forgetting that K-batch is our control group and is explicitly only exposed to dead regions. I'll never understand how he made it this far in life.

今日は騒動があった。ユニットB-17、H-47、K-43が異常なfMRI値を示したのだ。愚か者のベケットは、我々が新たな第1級FCIを発見したのかもしれないと示唆した。K群は対照群であり、明確に失活領域のみに曝露されているという事実を間抜けにも忘れていたのだ。あの男がどうやってここまで生き延びてこられたのか、私には理解できない。

I had them taken down and shipped off to bio for testing. Results came back by early evening: PET scans revealed TDP-43 aggregates -- heavy protein folding. The readings were skewed because their minds were systematically being reshaped. Decided to reinstate B-17 and monitor the situation. H-47 and K-43 have been placed in cold storage.

私はそれらを検出プロセスから外し、検査のため生物学部門に送らせた。夕方早くに結果が戻ってきた。PETスキャンでTDP-43凝集体が確認された。重度のタンパク質折り畳み異常だ。彼らの精神が体系的に再形成されていたため、測定値が歪んだものと思われる。B-17の復帰を決定し、状況を監視することにした。H-47とK-43は冷凍保存に回した。

No correlation between the BL regions they'd been exposed to over the last year. No clear demographical similarities between subjects.

この変異と、過去1年間に曝露されたベリーマン=ラングフォード領域との相関関係は見られない。被験体間に明確な人口統計学的類似点もない。

And as this day is only getting better, I noted physiological changes with Perseus. Vortex veins in the scelera have seemingly become more pronounced. Brain-state nominal, for now, but I might have to beg O5-8 for a replacement soon.

さらに、ペルセウスに生理学的変化が確認された。強膜の渦静脈がより顕著になっているように見える。脳の状態は今のところ良好だが、間もなくO5-8に代替品を要請する必要があるかもしれない。実に儘ならぬ1日だ。

[[/div]]

[[div class="blockquote"]]
Seven more Berries displaying the same protein folding.

さらに7つの「苺」が同様のタンパク質折り畳み異常を示した。

Perseus' situation continues to devolve. A vein in the right sclera has seemingly distended, breaching the iris of the right eye. Between recent mishaps and the state of our star pupil, migraines have started getting worse. Constant ringing in my ears.

ペルセウスの状況は悪化の一途を辿っている。右眼球の強膜血管が膨張し、虹彩を侵食しているように見える。最近は悪運続きで、我らが優等生の状態も悪い。偏頭痛がひどくなってきた。耳鳴りも止まらない。

[[/div]]

[[div class="blockquote"]]
New shipment today, so we're finally back at full capacity. No time to celebrate this, though.

配送があった。やっとフルスペックで稼働ができる。これをお祝いできるほどの時間はないけれど。

Beckett collapsed. Happened right in front of me as I exited Perseus' cell. He'd been across the room helping to install replacement subjects when he suddenly went down. Idiot likely caught a glimpse of one of the Kempelen screens. Shame it wasn't First Order.

私がペルセウスの部屋から出てきたとき、私の目の前でベケットが倒れた。彼は部屋の向こう側で交代要員の設置を手伝っていたときに、突然崩れ落ちたのだ。愚かなことに、彼はケンペレン・スクリーンの1つを直視してしまったに違いない。第1級を見ていれば良かったのに。

Coleman insists Beckett simply hasn't gotten much sleep lately. Few on the team have. There's this shrill sound audible in the production center and Kempelen facility. We've not identified the source, but it'd explain the tinnitus, at least.

コールマン曰く、ベケットは睡眠不足だそうだ。実際、チームのほとんどが睡眠不足だ。生成センターとケンペレン施設で、何か甲高い音が聞こえるようになった。音の原因こそわからないが、この音が耳鳴りを起こしているとすれば、最低限説明はつく。

[[/div]]

[[div class="blockquote"]]
Hyperoxia -- oxygen intoxication. Beckett is stable in medical right now, but it appears that his body is taking in an excessive amount of oxygen. Had Parsons run an CT and sure enough, his pulmonary vasculature seems to have nearly-doubled in complexity.

ベケットは高酸素症、つまり酸素中毒らしい。彼の体は医務室で安定しているが、体が過剰な酸素を取り込んでいるようだ。パーソンズにCT検査を実施させたところ、案の定、彼の肺血管系の複雑さがほぼ倍になっていた。

It's clear now. The affected Kempelen subjects were situated within line-of-sight of Perseus' cell door. Checked to make sure the SRA array is still functioning, and everything comes up clear. Whatever's happening, it's not reality-bending. Not exactly. Even if Perseus wasn't kept in check with SRAs, he wasn't a particularly strong bender in life -- he couldn't so much as will his shoes tied together.

これですべてが明らかになった。影響を受けたケンペレン被験体たちは、ペルセウスの部屋のドアが見える位置にいた。SRAアレイがまだ機能しているかを確認したところ、それらはすべて正常であった。何が起きているにせよ、正確に言えば、これは現実改変ではない。たとえペルセウスがSRAで抑制されていなかったとしても、彼にこんなことができるとも思えない。彼は生前それほど強力な改変者ではない--　　--現実改変で靴紐を結ぶことすらままならないほどなのだから。

I'm going to need to get tested myself.

私自身も検査を受ける必要がある。
[[/div]]

[[div class="blockquote"]]
By all rights, I should be dead.

どうして私がまだ生きているのか、これがわからない。

Myself and near everyone who'd been in the Kempelen facility over the last several weeks. I've got it worst of the bunch -- my bean is damn-near the shape of a pretzel. Despite this, I feel fine. Ran a battery of cognitive assessments. All clear. "The very picture of perfect mental health" -- Parsons was always bit of a kissass, but I'll take whatever reassurance I can.

この数週間ケンペレン施設にいた私を含めたほぼ全員が、どうしてまだ生きているのだろうか。その中で私が一番ひどい状態だ。脳などほとんどプレッツェルの形になっている。それにも関わらず、体調は良好だ。認知機能検査を一通り実施したが、全て正常。「お手本のように完璧な精神状態」とは、パーソンズの言葉だ。良いお世辞だ。そんな言葉も、今となってはありがたい。

In other news, Beckett's up and running, quite literally, with a fervent energy the layabout's not displayed before. As if his body's simply adjusted to the excess oxygen intake. Even had a bright idea, for once. On his suggestion, we fed some recently-discovered Second Orders through B-17's monitor. No effect. So we tried a First Order.

他の変化もある。ベケットが文字通りに走り回っているのだ。あの怠け者が、今まで見たことのないほど熱心に働いている。まるで身体が過剰な酸素摂取に適応したかのようだ。珍しく良いアイデアまで出した。彼の提案で、最近発見した第2級をいくらかB-17のモニターに流してみた。効果なし。そこで第1級も試してみた。

Nothing. It's become immune.

何も起きない。免疫を獲得したのだ。
[[/div]]

[[div class="blockquote"]]
Almost a decade of dead ends, of painstaking trial-and-error, of pathetic, minuscule baby-steps; all washed away in a matter of weeks.

ほぼ10年間の行き詰まり、骨の折れる試行錯誤、哀れで微々たる歩み、それら全てが数週間で洗い流された。

About a third of our Berries have been affected by Perseus. Of them, not a one has shown any susceptibility to FCIs of any order. The staff, too, can now safely look at SCP-9001 readouts. It goes beyond mere immunity though. The affected staff can now directly identify active regions when traversing generations of the fractal plane! Over one-hundred First-Orders located within an hour, as well as matching inoculant-zones. It feels so natural. Like scanning the beach with a metal detector. One only has to listen closely. The swirls and lines call out. The shapes are practically screaming.

我らが「苺」の3分の1がペルセウスの影響を受けた。そのうち1つとして、いかなる等級のFCIにも感受性を示すものはない。職員も同様で、今やSCP-9001の出力を安全に視認できるようになっている。しかしそれは単なる免疫を超えていて、影響を受けている職員は、生成されたフラクタル平面を巡っているときに、活性領域を直接特定できるようになったのだ。1時間もしないで100を超える第1級が発見され、それぞれに対応する免疫領域も特定された。実に自然なことだ。金属探知機でビーチを探索していることと、よく似ている。ただ注意深く聞けば良いだけのことだったのだ。渦と線が呼びかけている。形が本当に叫んでいるのだ。

Gone away are the brute-force methods of the past, Perseus has given us the keys to true progress: on-demand FCI production. And if that's not enough, Perseus delivers on a second front: I tested some of the older CCIs we have on-file; across the board, they've shown zero effect on my staff.

過去の力任せな手法は去った。ペルセウスは我々に真の進歩への鍵を与えてくれた。オンデマンドでのFCI生産である。それだけでは不十分とでも言うように、ペルセウスは第二戦線でも成果を上げている。保存されている古いCCIをいくつか職員にテストしたが、効果が一切見られなかった。

The implications for wider Foundation use is staggering! With a moment's exposure, agents can be granted immunity to cognitohazardous influence. This is lives saved -- in the field, in containment, in research and study -- Perseus is going to change the way we operate.

財団全体に対する応用の可能性が、かなり広がった。現場においても、収容においても、研究と調査においても、一瞬の曝露で、エージェントに認識災害の影響への免疫を付与できる。これは命を救うということだ。ペルセウスは我々の活動方法を変えるだろう。

To think I'd be the architect behind not one but two Thaumiel-class anomalies. Decided to shut down Perseus' SRA array. Wasted power. Without their constant humming, it's much easier to hear the pattern.

1人でタウミエル級の異常を2つも設計することになるとは思わなかった。ペルセウスのSRAアレイを停止することにした。あの際限のない唸りさえなければ、形を聞き取るのがずっと楽になる。

The only bad news is even this incredible development //still// doesn't solve Project NIETZSCHE. No matter -- we must be close now.

唯一の悪い知らせは、この信じ難い発展をもってしても、NIETZSCHE計画の解決にはまだ至らないということだ。構わない。もう間近のはずだ。

[[/div]]

[[div class="blockquote"]]
I've started cycling in some of our Level 2 and 3 staff into the Kempelen facility. Physical mutations. Three of my Level-5's have developed polydactyly. The fingers are fully-functional, and none have reported any pain, but it may be best to start limiting exposure. We're not quite prepared to publish our findings to Eight just yet --it would only take one word to shut us down entirely.

レベル2とレベル3の職員をケンペレン施設にローテーションで配置し始めた。身体変異が起きている。レベル5職員のうち3名が多指症を発症した。指は完全に機能しており、痛みを訴える者もいないが、曝露を制限し始めた方がよいかもしれない。我々の発見をO5-8に発表する準備はまだ整っていない。結局のところ、あれは一言発するだけでこのすべてを停止できてしまうのだから。

Or... would Eight's words even affect us? What is Perseus //actually// doing?

だが、本当に停止できるのだろうか？　ペルセウスがやっていることの本質とは、何だ？

[[/div]]

[[div class="blockquote"]]
The sound is omnipresent. Not just within the fractal plane, but in the walls, in the eyes of my staff. In my dreams. It calls. The Prima Materia. The Unus Mundus. The very bottom of everything. It's getting hard looking at certain surfaces -- the walls, countertops, the ordered lines on reams of paper.

音が遍在している。フラクタル平面の中だけでなく、壁の中に、職員たちの目の中に。私の夢の中にも。それは呼んでいる。第一質料を。一つの世界を。あらゆるものの根源を。壁、作業台、紙束に印刷された整然とした線--　　--特定の表面を認識するのが困難になってきた。

Staring into the depths of the fractal plane is the only thing that alleviates the headaches. Figure we should leave Perseus' door open. The site could go for some remodeling.

フラクタル平面の深淵を見つめることだけが頭痛を和らげる。ペルセウスの扉は開けっ放しにしておくべきだろう。サイトには改装が必要だ。

90% of the Berries now display protein-folding. Running out of subjects to verify my team's findings. Cannot afford to reach out, not yet. Too soon since last D-class shipment.

「苺」の90%が現在タンパク質折り畳み異常を示している。チームの発見を検証する被験体が不足している。まだ外部に働きかけるわけにはいかない。前回のDクラス輸送から日が浅すぎる。

There has to be another way we can source fresh subjects.

新鮮な被験体を調達するための、別の方法があるはずだ。

[[/div]]

[[div class="blockquote"]]
Mutations progress. To our benefit. Coleman has taken on the work of five people. Runs the production facility himself. Others off Berry-picking.

我々にとって有益な方向に、変異が進行している。コールマンは5人分の仕事をこなすようになった。生産施設を一人で運営している。他の者たちは苺摘みに出ている。

Parsons found Beckett in Data Storage. Seems he found a good use for himself.

パーソンズがデータストレージでベケットを発見した。自分なりに有効活用法を見つけたらしい。

[[/div]]

[[div class="blockquote"]]
Starting to get the hang of it. Expose them in doses, careful not to water them too much. Prune a bit off here and there when limbs begin to grow unruly. Pity they need me so. That they'd grow wild if left to their own devices.

コツを掴み始めている。適量ずつ曝露させ、水をやりすぎないよう注意している。手足が手に負えなくなり始めたら、あちこち少しずつ剪定する。彼らがこれほど私を必要とするとは哀れなことだ。放っておけば野生化してしまうのだから。

I always did have a green thumb. I'm even better with twelve.

私はもともと園芸が得意だった。12本の指があれば、さらに上手になる。

[[/div]]

[[div class="blockquote"]]
One of our new subjects chanced an escape. He wasn't able to get far.

新しい被験体の一人が偶然逃走した。しかし遠くまでは行けなかった。

Lost in the halls. Running in circles. Couldn't navigate the space.

彼は廊下で迷っていた。同じ場所をぐるぐる回っている。空間を把握できないのだ。

Not like we can.

我々のようにはいかないのだ。

He can be made to listen, though. Hear how we hear. Beckett could use some company.

だが彼も聞けるようにできる。我々が聞くように聞けるようにできる。ベケットにも仲間が必要だろう。

[[/div]]

[[div class="blockquote"]]
Calls coming in now from Site-01. Hard to hear over the sing, sing, singing. Its sound merely joined the chorus. The harmonious tune. It's hard not to sing along with the others.

サイト-01から連絡が入っている。歌声、歌声、歌声に遮られて聞き取りにくい。その音もただ合唱に加わっただけだ。調和の取れた旋律。他の者たちと一緒に歌わずにいるのは難しい。

Harder yet not to scream.

叫ばずにいるのはさらに難しい。

Let them come.

来るなら来ればいい。

[[/div]]

 _

**Addendum:** On 2025-09-01, Dr. Langford filed a support ticket with IT. The ticket complained that any function he wrote would infinitely recurse until crashing with a RecursionError, even if obviously expected to terminate, while a high-pitched noise would be emitted from within the computer. Upgrading his outdated Python3 interpreter version, as suggested by IT, did not resolve the issue.

**補遺:** 2025年9月1日、ラングフォード博士は情報技術部門にサポートチケットを提出しました。チケットにおいて、彼は、明らかに終了することが期待される関数であっても、彼の書いた関数が無限再帰してRecursionErrorでクラッシュし、同時にコンピューター内部から高音のノイズが発せられるという問題を報告しました。ITの提案により旧式のPython3インタープリターをアップグレードしましたが、問題は解決されませんでした。

The following morning, Dr. Langford alerted site security that he had found a single bunch of carrot flowers growing from the chassis of his personal computer. After investigation, Site-15 was placed on lockdown for 6 hours, and all personnel were screened for fractal growths or obvious medical abnormalities before being allowed to leave the site. Dr. Langford was issued a new computer and desk; his old ones were contained for study.

翌朝、ラングフォード博士はサイト警備部に対し、個人用コンピューターのフレームからニンジンの花が一房生えていることを発見したと報告しました。調査の結果、サイト-15は6時間にわたってロックダウンされ、全職員がフラクタル状増殖や明らかな医学的異常の有無をスクリーニングされた後、サイト退出を許可されました。ラングフォード博士には新しいコンピューターと机が支給され、旧機器は研究のため収容されました。

Upon disassembly, it was found that a small amount of soil had been deposited into the chassis, from which the carrot flower had grown. A review of security footage over the last week revealed that this occurred several days prior, during landscaping endeavors on site grounds. Langford's office sits below ground level, and a flurry of dirt and particulate had blown through the open window above his desk. Langford himself would enter hours later, and nonchalantly brush off what dirt had not already fallen through the vents. Dr. Langford was informed of this, and reminded of the fact that carrot flowers grow naturally on Site-15's grounds.

分解調査の結果、シャーシ内に少量の土壌が堆積しており、そこからニンジンの花が生長していたことが判明しました。過去1週間の監視映像の検証により、これは数日前、サイト敷地内の造園作業中に発生したものであることが明らかになりました。ラングフォード博士のオフィスは地下階にあり、机上の開いた窓から土埃や粒子状物質が舞い込んでいました。ラングフォード博士は数時間後にオフィスに入り、通気孔から落ちなかった土埃を何気なく払い落としていました。ラングフォード博士にはこの事実が伝えられ、ニンジンの花はサイト-15の敷地に自然に生育していることが再確認されました。

Dr. Langford refused to accept this explanation, which in combination with his difficulty adapting to mandatory counselling following the events at Site Romero-5, indicated a need for further psychological resources.

ラングフォード博士はこの説明を受け入れることを拒否しました。これは、サイト・ロメロ-5での事件後の義務的カウンセリングへの適応困難と相まって、さらなる心理的支援の必要性を示していました。

During his first appointment with Dr. Glass, Dr. Langford was administered a Rorschach test and quickly became deeply agitated, necessitating sedation. It was later found that Dr. Langford had developed auditory-visual synesthesia regarding complex fractal imagery. Upon seeing such images, Dr. Langford subjectively experiences the distant sound of screaming.

グラス博士との初回面談において、ラングフォード博士にロールシャッハ・テストが実施されましたが、深刻な動揺を示したため鎮静剤の投与が必要となりました。後の調査により、ラングフォード博士は複雑なフラクタル画像に関して聴覚・視覚共感覚を発症していることが判明しました。そのような画像を視認した際、ラングフォード博士は主観的に遠くからの叫び声を知覚します。

 _

[[footnoteblock]]
