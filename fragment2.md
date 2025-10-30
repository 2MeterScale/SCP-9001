[[include :scp-wiki:component:hoverlinks]]

[[include :scp-wiki:theme:black-highlighter-theme]]
[[include :scp-wiki:theme:jakstyle]]

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
  max-width: none;
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

[[>]]
[[module Rate]]
[[div_]]
[[size small]]Page 2 of 2[[/size]]
[[/div]]
[[/>]]

-----

[[table style="border: none; width: 100%;"]]
[[row]]
[[cell]]
[[size 125%]]**Item #:** SCP-9001-A[[/size]]
[[/cell]]
[[cell style="text-align: right;"]]
[[size 125%]]###f00d|**Level 2/9001**##[[/size]]
[[/cell]]
[[/row]]
[[row]]
[[cell]]
[[size 125%]]**Object Class:** Keter[[/size]]
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
Initial assault on Site Romero-5 by Nu-7 ("Hammer Down") strike teams.
[[/div]]
[[/div]]

-----

[[div class="conprocs"]]
[[span style="color: white; background: #f008; padding: 3px 5px 1px; border-radius: 3px; text-transform: uppercase; font-weight: bold; margin-left: -2.5px"]]Emergency Containment Procedures:[[/span]] An Exclusion Zone has been established 3km from the event horizon of SCP-9001-A, and is enforced by an array of Scranton Reality Anchors. As of this writing, the local supply of anchors has been exhausted; additional materials from Site-118 are currently en-route.

Agent Troy Lament has assumed the role of General Commander of Task Forces in the region, operating out of Forward Operating Base Panloque, established outside the bounds of the SRA array. Operatives from Mobile Task Forces [[span class="hoverlink"]][[[task-forces#eta-10|Eta-10]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Eta-10 ("See No Evil")[[/span]][[span class="hoverlink-text"]]Specialists in circumventing/containing perceptual hazards. Eta-10 uses specialized equipment (such as the "SCRAMBLE" goggles) in order to protect its agents from anomalous effects triggered or expressed through sensory perception[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Eta10.png/small.jpg)"]]-[[/span]][[/span]][[/span]], [[span class="hoverlink"]][[[task-forces#theta-90|Theta-90]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Theta-90 ("Angle Grinders")[[/span]][[span class="hoverlink-text"]]Experienced pathfinders and wayfarers in areas where local topography does not align with conventional understanding of spacetime, such as iterative, recursive, and infinite zones. Theta-90 specialists are also tasked with diplomatic missions into non-hostile Nexus locales.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Theta90.png/small.jpg)"]]-[[/span]][[/span]][[/span]], [[span class="hoverlink"]][[[task-forces#epsilon-11|Epsilon-11]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Epsilon-11 ("Nine-Tailed Fox")[[/span]][[span class="hoverlink-text"]]Specialists drawn from across the MTF network, deployed to establish control of Foundation Sites experiencing breaches and/or occupation by hostile forces and GoIs. Famous for their efforts in combating a containment breach at Site-19.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Epsilon11.png/small.jpg)"]]-[[/span]][[/span]][[/span]] and [[span class="hoverlink"]][[[task-forces#zeta-9|Zeta-9]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Zeta-9 ("Mole Rats")[[/span]][[span class="hoverlink-text"]]An exploration team tasked with probing and mapping underground or ontologically unsound areas. Typically deployed as a first-line resource, Zeta-9 has a notoriously-high mortality rate. Despite this, Zeta-9 operatives are seen by many to be the most capable for exploration of any sort.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Zeta9.png/small.jpg)"]]-[[/span]][[/span]][[/span]] are being assembled into special teams for exploration of the Zone. MTF [[span class="hoverlink"]][[[task-forces#iota-10|Iota-10]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Iota-10 ("Damn Feds")[[/span]][[span class="hoverlink-text"]]Personnel embedded within law enforcement and similar institutions. As a public-facing entity, Iota-10 is usually tasked with intelligence-gathering, working alongside government agencies and local police. Iota-10 also serves as an early-warning for civilian anomalies.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Iota10.png/small.jpg)"]]-[[/span]][[/span]][[/span]] is tasked with diverting civilians from the area.

The Exclusion Zone's perimeter is to be enforced by Armed Mobile Task Force [[span class="hoverlink"]][[[task-forces#nu-7|Nu-7]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Nu-7 ("Hammer Down")[[/span]][[span class="hoverlink-text"]]A battalion-strength regiment of soldiers and combat/vehicle specialists. Deployed in events where Foundation facilities have been compromised, or when containment calls for the use of overwhelming force.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Nu7.png/small.jpg)"]]-[[/span]][[/span]][[/span]], who have been tasked with carrying out a controlled burn of the forest within the zone.

Living organisms attempting to cross the SRA boundary are to be summarily terminated. The remains of any affected lifeforms are not to be taken for research purposes -- they are to be deposited back within the bounds of the Exclusion Zone and incinerated.

Should the area-of-effect expand beyond the Exclusion Zone, an All-Hands Notice is to be issued worldwide in preparation for a ZK-Class Reality Failure Scenario.
[[/div]]

**Description:** SCP-9001-A refers to an expanding region characterized by non-Euclidean geometry, spatial inconsistencies, and the elaborate growth and fractalization of complex systems.

SCP-9001-A is expressed through the formation of vestigial facilities emerging from Site Romero-5, the shifting of local topography and meteorological conditions with a preference for fractal organization, and the induction of physiological mutations in living organisms within its area of effect.

The means through which SCP-9001-A comes to infect a new system is currently unknown, as early observations have ruled out direct contact as a strict prerequisite. It is possible that transmission occurs through metaphysical, conceptual, or associative means. Research conclusions are not yet definitive due to the rapidly evolving situation.

SCP-9001-A came to the attention of the wider Foundation following the first-hand experience of Special Operative Saunders.

**Discovery:** Special Operative Saunders was deployed to investigate the state of affairs following loss of contact with Dr. Berryman's team. S.O. Saunders was chosen due both to her immediate locality[[footnote]]S.O. Saunders had been embedded within the police force of the town of Willow Falls, located 10km south of Site Romero-5. She had been tasked with the investigation of a rash of missing-persons cases that had occurred over a 10-month period.[[/footnote]] and personnel CRV rating that would allow her to bypass protective cognitohazards embedded into signs posted along the sole access road.

-----

[[div class="blockquote"]]

= {{**VIDEO LOG**}}

----

The video opens, askew, from the perspective of the passenger seat looking up at S.O. Saunders, driving with a nondescript expression. A flurry of trees can be seen beyond the driver's side window. As the vehicle shifts around a bend, bright specks of orange daylight play across the vehicle's interior, prompting Saunders to swing the visor down. A look of confusion crosses her face.

Saunders hails Command, asking to double-check her positioning to confirm she's on the correct path. It is verified that she is. Rolling her eyes, Saunders implies incompetence on Command's part, owing to the fact that the access road was purported to be a direct line, whereas her current path is taking her down a long road with a subtle curve.

Command notes the discrepancy. Saunders is asked to relay any peculiarities regarding her surroundings, but only notes that the road itself is in disrepair, with overgrown foliage and weeds encroaching on either side of the blacktop. It is as she's explaining this to Command that she trails off, leaning forward with a confused expression.

The flurry of trees begins to slow until the vehicle comes to a complete stop. Saunders flashes a quick glance towards the camera and shifts into park. There is a momentary jostling of the camera's field of vision as Saunders places her helmet on and exits the vehicle.

From her perspective, it can be seen that thick, gnarled root systems of surrounding trees have fully disrupted the roadway, causing it to fracture and splinter, with one nearby root growing around and dislodging a deer-crossing sign. It appears as if the road had not been used in decades.

After brief deliberation, it is decided Saunders should continue on foot. She leans into the vehicle to retrieve her keys from the ignition, and closes the door behind her.

Without the rumble of the engine, the near-silence of the surrounding wilderness comes into focus. There is no birdsong, nor chirping of insects. There is only a quiet creaking from an unknown source, likened by Saunders to that of old wooden floorboards. She sets off, stepping over the obstructing roots as she progresses.

Saunders continues for the next kilometer at a measured pace. Though near enough to the site on GPS that she'd presumably spot it in the distance, the curvature of the road only seems to increase as she progresses. The path ahead veers further and further to the left, limiting the length that can be seen. Further impacting visibility is the sheer depth of the canopy above, blocking out most sunlight. What little daylight that does break through is itself dimming as thick clouds roll over the area.

A blaring horn is heard in the distance. Quickening her pace, Saunders rounds the bend, coming to see a black sedan some distance ahead. It appears that the vehicle had flown off the road and crashed headfirst into a nearby tree. The windshield is marred in a cobweb of broken cracks. The driver's-side door is ajar. Though its plate cannot be seen, Command is able to identify that it would have belonged to one of the researchers on-site.

The horn slowly gets weaker as Saunders approaches, dying out completely as she comes near. There is a subtle 'click' as Saunders releases the safety on her sidearm. She steps carefully, silently, around the open door, wheeling around it and bringing up her weapon in one fluid motion.

The vehicle is empty. Its airbag, deployed in the crash, rests partially-deflated. There is a smattering of blood stains present upon the driver's seat and steering wheel and spattered randomly across the upholstery. Saunders scans the area, checks under the vehicle, and only then holsters her weapon. She reaches into the center console, rummaging about to find a personnel lanyard. The coloration indicates it had belonged to a Level-3 researcher, but the surface is marred and scratched, with particular emphasis on the researcher's portrait. The text has been rendered illegible.

It is as Saunders moves to pocket this that she looks up at the shattered windshield. A bloodied handprint has been pressed against the interior side. It possesses four additional digits.

Command advises Saunders to turn back, as it has become apparent that the situation may call for a properly-equipped Task Force. Saunders however cites her tenured field experience, claiming that if site staff are in danger, then she's obligated to lend her services. Command moves to notify Site-01 as Saunders rushes off down the road. A low fog begins to sweep the area.

[[div class="scp-image-block block-center"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/footage1.webp]]
[[/div]]

The curvature of the road steepens the further Saunders travels, becoming stark to the point that it appears as if Saunders is running in a circle. The fog increases in intensity, obstructing visibility and causing Saunders to nearly trip over unseen roots criss-crossing the road. It is as Saunders comes around the next bend that the thicket of trees begin to recede. GPS indicates her arrival. Saunders comes about to face Site Romero-5.

The air here is thick with occluding fog. All that can be seen throughout the site grounds are mere silhouettes of buildings, the bright fluorescence of their interiors being the only visible sources of light in the murk. From the woods behind her, there comes a pained cervine bleating. Saunders ignores it as she steps past the chain-link perimeter fence.

[[div class="scp-image-block block-center"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/romerofog.webp]]
[[/div]]

There is a low rumble that shakes the area, sending Saunders to the ground. Looking up, Saunders captures the silhouette of the nearest building -- its shape contorts and extends, jutting outward to the left of the frame, forming a branch that connects to a separate facility. Bright pinpricks open up along the length of this new addition, quickly widening and taking the shape of new windows. The earth continues to quake as buildings further off in the distance repeat this process.

Just as suddenly as the shifts occur, they come to a standstill. Saunders shakily stands up. The complex before her, moments before a scattering of various facilities, seems to now be a single continuous complex. Command is able to verify this via satellite imagery: though somewhat obscured by increasing cloud cover, an overhead perspective of the site confirms that the buildings have indeed interlocked. They have taken on the shape of a spiral.

Saunders finally admits that the current state of affairs is beyond her ability to personally resolve. Deciding that finding a capable off-road vehicle would be preferable to heading backwards on-foot, she convenes with Command to determine the approximate location of the site's vehicle bay. She sneaks off counter-clockwise around the site, sticking close to the perimeter fence. Dark shapes within the site cross in front of the windows, and Saunders doubles her pace.

With assistance from Command, Saunders is directed to approach the contiguous structure. There is a large garage door on the face of the wall here. Saunders approaches the keypad beside the door, withdraws the lanyard she'd acquired and swipes it -- access is granted. The door begins to raise. Saunders swears loudly as its heavy, metallic rattling harshly breaks the silence of the site grounds. From somewhere out of frame there comes a deafening, protracted noise with the cadence of an air raid siren. It is distinctly human in origin; a blending of many voices that rise and fall in a cacophonous wail.

Saunders curses again, dipping below the door before it is fully opened. The interior of the vehicle bay is well-lit. Rows of personal vehicles line either side of the chamber. Saunders rushes past a vast majority of the fleet, composed of modern top-of-the-line models, towards an older-model Jeep near the back. Swinging into the cabin, Saunders reorients herself beneath the steering column to begin hotwiring it. The feed darkens as she works.

The sound of her haggard breathing is drowned out by a shrill wail, closer than the first.

The feed alights with a spark, and there is a rumbling of the engine. Saunders excitedly shouts, quickly rights herself, and shifts into drive. She peels out of the parking space just as the door at the end of the garage bursts open -- she does not turn to see what has entered.

Saunders navigates out of the garage and into the fog-laden site grounds. Dark, roughly-humanoid shapes can barely be made out as she speeds through towards the entry gate. As she slows to align with the access road, the vehicle is struck from the side. Glancing over her shoulder, a human arm can be seen latched onto the back of the Jeep. A second arm rises above it. A third. Each reaches farther in turn, sprouting many clasping hands that find purchase and work to pull the entity aboard.

Saunders turns her focus to the road ahead as she passes the perimeter fence, brandishing her sidearm and blindly firing three shots, which elicits an inhuman shriek. She steals a glance backwards -- the creature has been dislodged. She grunts with satisfaction, turning back ahead, only to find herself rapidly approaching a massive shape in the middle of the road. Headlights fall across a furred hide a half-second before she crashes at-speed into the beast.

Saunders is ejected from the vehicle, striking the ground and rolling several times before coming to a stop. From her position on the ground, the bulky frame of a deer becomes visible. It struggles to bring itself to a stand on six legs. A pair of heads, each encumbered by a complex tangle of antlers, rear back and weakly bleat before the beast collapses, dead. Command calls out to Saunders, shouting her name over the mic repeatedly, but she is unresponsive.

After a moment, there is movement. Saunders coughs. She groans, turning herself over to lie on her back. Looking down, a sharpened end of a bone now juts from her left leg. She screams as the bone can be seen to shift, splitting along its end, forking in two directions which themselves split and grow and fork. Her pained screams are drowned out by the wailing chorus of approaching figures. Saunders desperately looks about the area -- and spots the glint of her sidearm a few meters away.

She drags herself towards it as Command attempts to reassure her as to her survival, promising that help is on the way. Saunders calls their bluff, noting that there is no chance for salvation and calling for Command to rain hellfire on the site. The wailing grows closer, each voice in itself a dozen anguished cries. Saunders grabs her weapon, rights herself up against a nearby tree, and waits.

Humanoid figures emerge from the fog on either side of the Jeep, cast in full silhouette against its headlights. Nothing more than their incomprehensible shapes can be made out -- torsos that split into multiple trunks, too-many arms extending from a single frame -- all converge on Saunders as she raises her weapon. She places two shots into the closest figure, dropping it. The third shot misses, taking out one of the Jeep's headlights. A rapid trio of shots strike yet another entity but does not halt its advance.

Hazy outlines resolve into clear figures as they close in. The face of the nearest figure, draped in a labcoat, opens a maw encircled by many rows of overgrown teeth and lets out a wail. Its dozen hands point towards the camera, its fingers flowering with new digits, and there comes a final gunshot. The feed falls to the ground.

The remainder of the footage captures the ground as Saunder's body is dragged back towards the site.

-----

[[/div]]

Emergency containment procedures would quickly be established following the receipt of this footage.

Initial attempts at an aerial assault on the facility were thwarted by hostile lifeforms, leading to the loss of twelve members of Nu-7. As containment teams scrambled to establish the Exclusion Zone and Forward Operating Base, Agent Lament would be sent by O5-8 to recruit Dr. Langford: a former researcher at Site Romero-5 and co-architect of SCP-9001.

[[div class="blockquote"]]

**VIDEO TRANSCRIPT 9001-1**

**PARTIES PRESENT:**
* Senior Researcher Robert Langford, consultant for MTF Eta-10 and Project MEDUSA, Site-15
* Agent Troy Lament, General Commander of Joint Task Force //Panloque//, Forward Operating Base Panloque

**FOREWORD:** Briefing Dr. Langford on SCP-9001-A containment efforts.

**<BEGIN TRANSCRIPT>**

//Commander Lament consults the seating chart on his tablet, looking for Dr. Langford's desk on the open floor plan. Dr. Langford is standing beside his standing desk, wearing a t-shirt, shorts, and a pair of headphones. Approaching from behind, Dr. Langford can be seen typing Python Tensorflow code into a Sublime editor. Commander Lament calls out to him, then taps his shoulder. Dr. Langford turns around and takes off his headphones.//

**Dr. Langford:** Ah, my apologies. Can I help you?

//Commander Lament extends his hand.//

**Cmdr. Lament:** Troy Lament. Containment and Recovery Specialist.

//Dr. Langford accepts. There is an awkward beat of silence as Lament awaits his response.//

**Cmdr. Lament:** ...and you're Robert Langford?

**Dr. Langford:** Right, yes. Sorry. Can I ask what this is about?

//Dr. Langford gestures towards a nearby bright green couch.//

**Dr. Langford:** Please, take a seat.

//Commander Lament shakes his head. He remains standing.//

**Cmdr. Lament:** I understand you mostly help Eta-10 these days?

**Dr. Langford:** That's right.

**Cmdr. Lament:** And before that you were a Senior Researcher for Project HYDRA at Site Romero-5, correct?

//Dr. Langford stops smiling.//

**Dr. Langford:** That's… correct. That prior experience is why I'm now attached to Eta-10 and MEDUSA.

**Cmdr. Lament:** You have combat training?

**Dr. Langford:** Excuse me?

**Cmdr. Lament:** You consult for a Mobile Task Force, don't you.

**Dr. Langford:** You're right… although truth be told, I could probably use a few more laps around the track or pool we have around here.

**Cmdr. Lament:** Excellent. That'll do.

**Dr. Langford:** Do for… what exactly did you want to discuss, Mr. Lament?

**Cmdr. Lament:** Perhaps showing is better than telling.

//Commander Lament hands his tablet to Dr. Langford. A video-player fills the screen.//

**Cmdr. Lament:** Play it.

//[The video is filmed from the perspective of a helicopter flying through the night sky  -- several more are seen in the distance ahead. The sounds of shouting passengers are drowned out by the heavy thumping of rotors.]//

//[Scanning the wooded expanse below, little can be made out as the region is mired in fog. As the perspective tilts, it comes into view -- buildings atop buildings, a veritable skyscraper whose floors are a confusing knot of interlocking facilities haphazardly growing from one another. A second helicopter circles around the side of the tower; its side-mounted machine gun fires at obscure figures crawling out from its windows.]//

//[A third helicopter speeds by -- as it descends near the tower, its tailboom fractures into two. Its rotors suddenly multiply, splitting from five into ten and then into an indistinct mass of metal, and it goes down; crashing into the side of the tower. Numerous crawling figures on the tower leap off the sides like fleas and take to the air, swarming around the tower and heading towards the viewpoint.]//

//[The perspective helicopter pulls back as the figures near, carried on the wind by reams of webbed skin that stretch between numerous arms. Four are downed by suppressive fire. A fifth flits about, avoiding the barrage and crashing into the windshield. Many lolling tongues extend from its throat, tearing into the cockpit.]//

//[The feed spins as the vessel goes down, cutting the transmission upon contact with the ground]//

//Dr. Langford rolls away his chair, staring at the table.//

**Dr. Langford:** That... that can't be real.

**Cmdr. Lament:** Math wasn't my best subject, but I believe your site's coghaz's focused on fractals. And those freaky shapes we're observing are fractals. It's not a stretch. And it's //spreading//.

**Dr. Langford:** What about Dr…

//Dr. Langford buries his face in his hands, then curls the latter into fists. After a while, he looks up at Commander Lament.//

**Dr. Langford:** I can understand why you came to me. I am willing to lend my expertise for the sake of the Foundation. But I must confess, this is a difficult subject for me.

//Commander Lament nods.//

**Cmdr. Lament:** I'm sorry to hear that.

**Dr. Langford:** Yeah… lots of memories. Not particularly… good ones either.

//Dr. Langford bunches his fists again and looks at an empty chair, as if looking at someone absent. He frowns, then exhales. A few seconds pass.//

**Cmdr. Lament:** I mean, I'm sorry to hear that, because you'll be deploying to Site Romero-5 with a squad from my Joint Task Force.

//Dr. Langford's shoulders slacken.//

**Dr. Langford:** Um, come again?

**Cmdr. Lament:** You will be deploying to Site Romero-5 with a squad from--

**Dr. Langford:** Absolutely not.

**Cmdr. Lament:** Perhaps I was unclear. I am ordering you to deploy to--

**Dr. Langford:** I don't care.

**Cmdr. Lament:** You don't get to say 'no'. This is coming from the top. O5-8 wants you, specifically.

//Dr. Langford takes a deep breath.//

**Dr. Langford:** I know full well the consequences of saying this, but whatever you do to me, you can't make me do it.

**Cmdr. Lament:** You will be taken and deployed on this mission regardless of your opinion, but it will make it a lot easier for everyone involved if you go willingly rather than forcibly dragged. Restrained if needed.

**Dr. Langford:** You don't understand what I witnessed at that Site. What we had to...

//Dr. Langford falls silent, although he starts to shake.//

**Cmdr. Lament:** You're right, I don't understand, and that's the thing. That site has gone radio silent for years except for scheduled package delivery. We have no idea what Dr. Berryman is up to, and now we see //this//.

//Commander Lament gestures at the tablet.//

**Dr. Langford:** Wait… you've had no idea what she's doing, for years?

**Cmdr. Lament:** Exactly.

//Dr. Langford sighs.//

**Cmdr. Lament:** But you, you worked at that specific site, on that specific project, for over a decade.

**Dr. Langford:** Look, I get that I worked at the site, but I haven't been there in over six years. I am just as in the dark as you all are. You have more up-to-date maps of the sites and more up-to-date project research notes.

**Cmdr. Lament:** But you know //more// than anyone else.

**Dr. Langford:** I'm not the only memeticist at the Foundation, I'm not even close to the best. I've field experience, sure, but I surely wouldn't be of use in--

**Cmdr. Lament:** How did Dr. Berryman like her coffee?

**Dr. Langford:** Excuse me? I fail to see how that's releva--

**Cmdr. Lament:** Answer the damn question.

**Dr. Langford:** A single piece of broken-up Cadbury chocolate melted in, and half a creamer pod since the chocolate already had some milk.

**Cmdr. Lament:** Favorite novel?

**Dr. Langford:** Snow Crash by Neal Stephenson.

**Cmdr. Lament:** Hobbies?

**Dr. Langford:** Caring for weird-looking flowers and succulents.

**Cmdr. Lament:** The truth is, Dr. Langford, the Foundation may have other memeticists, but its only expert on Dr. Berryman is you. And given how far the situation has progressed, we’re sure as hell going to need that.

//Dr. Langford stares at the floor for twenty seconds. He sighs, then speaks up in a whisper.//

**Dr. Langford:** … When do I deploy?

**Cmdr. Lament:** We're oscar mike oh-nine-thirty hours tomorrow, Dr. Langford. Pack your bags.

**<END TRANSCRIPT>**
[[/div]]

Upon his arrival at FOB Panloque, Dr. Langford would be outfitted and deployed alongside the JTF. It was decided the team would utilize Site Romero-5's subterranean tram access in order to bypass above-ground hostiles. Their mission would consist of three discrete objectives:
# Find and extract the core of SCP-9001 from the production center.
# Determine the locus of the SCP-9001-A phenomenon and destroy it, if possible.
# Apprehend or terminate suspected rogue agent: Dr. Ava Berryman

[[div class="explo-root"]]
[[div class="explo explo--room"]]
[[=]]
+ Exploration Transcript
[[/=]]

||~ Subject || SCP-9001-A ||
||~ Team Lead || Benton Torres, Captain, MTF Epsilon-11 ||

||~ Team Members ||
|| **Warren Gooden**, Technician, MTF Zeta-9 ||
|| **Sebastian Gooden**, Rifleman, MTF Zeta-9 ||
|| **Typhlo**, Deprivate[[footnote]]Operatives who have undergone invasive neurosurgical procedures to prohibit their ability to see, hear, taste, and smell. Augmented mechanoreceptors allow Deprivates an alternative means of perception by way of acute awareness of vibrations.[[/footnote]], MTF Eta-10 ||
|| **Special Operative Nix**, Navigator, MTF Theta-90 ||
|| **Dr. Robert Langford**, Negotiator ||

||~ Equipment ||
|| 4 standard-issue M27 Infantry Automatic Rifles and additional magazines _
6 M45A1 Close Quarter Battle Pistols and additional magazines _
5 compact Martel Pitons[[footnote]]Experimental technology developed by researchers in the wake of the [[[SCP-1730]]] incident. Allows for point-to-point instant transportation of personnel between emplaced Pitons in areas where spatial shifts might otherwise inhibit extraction.[[/footnote]] _
//Nix:// M38 Designated Marksman Rifle and additional magazines _
//Nix:// Prismatic compass _
//Warren:// Portable Scranton Reality Anchor _
//Sebastian:// 24" machete _
//Torres:// Quantum Entangled Relay Device, tethered to H.E.C.O.R.[[footnote]](High Energy Concentration Orbital Railgun)[[/footnote]] ||

-----

[[=]]
++ [BEGIN LOG]
[[/=]]

//The squad is traveling down a darkened flight of stairs through a concrete shaft. The door at its terminus opens into a dark, cavernous area. Automatic lights flicker on as they enter, revealing that they've entered a simple metro bored into the earth. Across from the entrance, a railway is set within a deep depression that trails off into the tunnel beyond. Within the station, shallow cracks run up the facade, support pillars, and across the ceiling, but otherwise the integrity of the chamber is holding up against topological restructuring.//

//Lights along the tracks within the tunnel do not engage, leaving the tunnel itself mired in darkness. The tram is not currently present.//

//The brothers, Warren and Sebastian, jog alongside the tracks towards a control booth on the far end of the chamber. Warren fiddles with the door fruitlessly until Sebastian pushes him aside.//

**Typhlo:** {{Echo mic check.}}

**Torres:** What? I didn't even-- ugh. We're live, folks. Check your mics.

**Warren:** Check.

**Nix:** Check, and cool it with the parlour tricks, Typh.

//Warren steps aside as Sebastian shoulders full-force into the door, forcing it open.//

**Sebastian:** Woo! That's a check!

**Dr. Langford:** Uhm... check.

//Sebastian and team fan about the chamber while Warren enters the control booth.//

**Torres:** Right. All golden. Warren, what've we got?

**Warren:** Looks like everything's still up and running. Tram's halted mid-way down the line. Last use was... about a month ago, according to the logs here. Looks like daily use up to that point, besides.

**Dr. Langford:** Should have been for the Director's use only, and Berryman isn't the sharing type.

**Typhlo:** {{Mutiny?}}

**Dr. Langford:** Against Berryman? I don't think so. The woman could //smell// insubordination. No, if they were using this thing it was on her orders.

**Sebastian:** Shit. Add that to the laundry list of questions for the doc'. //(louder)// Is the tram live or are we hoofin' it, Wally?

//There is a loud, electronic *ding*, and a distant sound of mechanical whirring.//

**Warren:** For the latter half of the trip, maybe. Have to wait and see what was holding it up. For now though, it's headed in our direction.

**Torres:** Good work. Typhlo, can you get a read on our transport? I need you to check for occupants.

//Typhlo drops onto the tracks, kneeling down to place a hand upon the rail.//

**Typhlo:** {{Approaching at a rate of eighty kilometers per-hour. Arrival expected in two minutes. No movement on-board.}}

**Dr. Langford:** Are we to expect a lot of resistance?

//Warren rejoins the squad, offering a hand to Typhlo, and helps her up from the tracks. Nix, kneeling across the chamber, places down a Martel Piton. The flat device quietly hums as four small rods eject from its sides and anchor to the ground.//

**Nix:** Depends. Since we made first contact, there's been a lot of those creatures escaping out into the surrounding area -- Hammer Down has had its hands full.

**Sebastian:** Makes ya wonder why we didn't pick up on this place sooner. S' like they went ape-shit the second their cover was blown.

**Torres:** All of this is to say, we simply don't know. Ghost town, if we're lucky.

**Dr. Langford:** And if we're not?

//Dr. Langford stares into the darkness of the tunnel.//

**Typhlo:** {{Simple. There will be bloodshed.}}

//After a moment, lights become visible in the tunnel. The tram speeds towards the platform, slowing down and coming to rest before the team. The doors open, and the squad carefully enters with weapons at the ready. Warren makes for the controls.//

**Torres:** Watch our speed, Warren. Last thing we need is for this to end up in training footage.

//The doors click shut, and the tram begins to move forward. A mechanical whirring persists throughout this portion of the video.//

**Warren:** ... Again.

**Dr. Langford:** Again?

//Sebastian laughs, taking a seat by the door.//

**Sebastian:** Oh, our Wally here is a star! "So You've Entered a Non-Euclidean Zone" -- you know, **that** scene?

**Nix:** No way.

**Torres:** That was him?

//Warren rubs his left shoulder.//

**Warren:** Bone never did set right.

//Typhlo suppresses a snicker. Dr. Langford halfheartedly forces an awkward chuckle.//

//The team waits in silence as the tram progresses. Intermittent fields of static momentarily interrupt the feed, but the connection remains sound. After a few minutes, Typhlo signals for Warren to stop, who acquiesces.//

**Typhlo:** {{Obstruction ahead. We walk from here.}}

//The doors slide open, and a light fog drifts into the compartment.//

**Torres:** Unusual.

**Sebastian:** Think it's toxic?

**Warren:** I could take off my mask and get a big whiff. Y'know. For science.

//Nix takes a knee, wafting her fingers through the fog.//

**Nix:** Just like in Saunders' footage. I thought it was just a meteorological effect.

**Dr. Langford:** It likely is. The anomaly seems to be restructuring everything into fractal patterns. Could very well be that it is condensing and organizing water vapor in the same manner.

**Torres:** Probably not something we want in our lungs regardless. Let's get moving.

//The squad leaps out onto the tracks, navigating to the front of the tram, and begins walking. Through the low-laying mist, it becomes apparent that the rail ahead has been rent and twisted by the emergence of large tangles of tree roots, growing from all about the tunnel floor, walls, and ceiling. The sound of wooden creaking becomes audible. As the team moves between the roots, the ends of the nearest can be seen to gradually split and grow. There is little chatter as they travel the last few kilometers. Light is seen in the distance.//

//The team exits the tunnel, emerging into the Romero-side metro cavern, identical to its counterpart on the other side of the tunnel save for more prominent wear on the facade and chamber walls. One by one, the team clambers up off the tracks and onto the platform. The fog here is heavier, permeating the air through to the ceiling, but is not thick enough to fully occlude sight. They cross the chamber towards a flight of stairs leading up.//

**Dr. Langford:** We should be able to directly access the Director's office from here.

**Warren:** Directly? Isn't that a little weird?

**Torres:** Not if you're both paranoid and also very important. Not out of the ordinary for Directors to have emergency escape routes.

**Dr. Langford:** Elevator just outside her quarters should get us access to most of the site. The FCI production facility was Sublevel 2, so not much of a jaunt should the elevators be down. Ah, here we are.

//A set of large double doors bars entry -- Nix and Sebastian, ahead of the team, step aside for Torres to come through.//

**Nix:** Compass is going wild. Be ready.

//Torres swipes a keycard with Level-5 access. The doors open silently, and a dense cloud of fog emerges from within. It subsides after a moment, allowing the squad to see within. Sebastian whistles loudly. Dr. Langford gasps. Nix trains her rifle ahead.//

**Torres:** What in God's name...

[[div class="explo explo--room"]]

//Before the team is a wide, open room bathed in fog. Over a dozen tall, plant-like trunks of varying skin tones are spread throughout the chamber. Each hosts a complex array of tendrils at its apex that weave with those of their neighbors, forming a canopy that partially blocks out the fluorescent lights. Each trunk pulses rhythmically, with twin-bulbs that are seen to emerge from a chest-high orifice. The bulbs of each instance inflate and deflate in synchronicity. Shelving across the walls, as well as deconstructed server racks, would denote that this area had once served as the Site's Data Storage Center.//

**Dr. Langford:** I... I'm gonna...

**Torres:** Swallow it. I thought you said this was the Director's office?

**Sebastian:** Are those fucking //lungs//?

//Nix takes point as the squad carefully advances. Just as with the canopy above, the entities are rooted in place via a thin network of mycellium that is splayed over the floor. The instances collectively shudder as this network is crushed underfoot.//

**Dr. Langford:** Pul-- //(gags)// pulmonary vasculature is inherently fractal. It makes sense something like that could come under influence.

//Dr. Langford pauses.//

**Dr. Langford:** And... yes. It //should// be her office.

**Nix:** Whole site must have been rearranged. I'll have to thread a line here.

//Closer inspection of the nearest trunk reveals that the open orifice is surrounded by displaced teeth, forced outward by the expanding bulbs. The remnants of the face -- eyes, nose and ears -- have been rendered vestigial, being stretched along the backside of the trunk. As the entities collectively exhale, there is a quiet sighing; a fine mist can be seen to extrude from their open pores.//

**Torres:** Were these researchers? Langford, you recognize anyone?

//Dr. Langford shakes his head. Warren moves carefully towards one of the trunks.//

**Warren:** This gas... some kind of terraforming?

//Sebastian grabs his knife and attempts to puncture the nearest bulb; it rebounds off. Sebastian curses under his breath.//

**Torres:** Whatever they're doing, we can't let it continue. Typhlo, got anything?

**Typhlo:** {{Heart rates at... six beats per minute. Likely depend on retaining a circulatory system. Could bleed them out.}}

//At this, Sebastian slices deep into the trunk beneath its orifice. Torrents of crimson blood rush from the wound -- the rest of the congregation whines and shivers as the wounded instance seizes and falls still. The deflated bulbs hang limply from its orifice.//

**Torres:** Warren. Sebastian. You two handle them. Make it quick. I'll get on top of manually disconnecting these servers just in case they're still capable of sending out kill agents. I want Langford and Typhlo to dig through those files, see what you can see. Or... well, you know what I mean, Typh.

**Typhlo:** {{Offense not taken.}}

**Torres:** And Nix, you make good on our way out.

//Nix nods and produces a second Piton, finding a corner clear of mycellium to set it up. The remaining squad spreads out and gets to work. The quietude of their labor interrupted only by bursts of pained moans as each instance has its throat slit in turn. It is as Sebastian terminates the final instance that Dr. Langford calls out.//

**Dr. Langford:** Hey, come take a look at this.

//The team converges on Dr. Langford, currently digging into a cardboard box. From within, he begins pulling out personal effects; keys, cigarette lighters, a handgun and taser -- he then pulls out a wallet, passing it to Warren before retrieving and opening a small leather purse. Sebastian rummages through the wallet, pulling out and discarding a credit card, before selecting from within a driver's license.//

**Sebastian:** Don't see any Foundation ID. Is this a civilian? You recognize this face, doc?

//Dr. Langford looks up from the purse, stares at the license for a moment, then shakes his head. Nix reaches out and takes it from Sebastian.//

**Nix:** I do. This guy wouldn't be Foundation, no. I dug into Saunders' assignment after watching her footage -- missing persons investigation in the town down the way. This'd be Ernest Graham, age 42, one of the first to go missing back in March.

**Torres:** Shipment of D-class would have been received in January. Guess they got impatient.

//Dr. Langford cocks his head, looking at Torres.//

**Dr. Langford:** D-Class? That's... odd. They shouldn't have need for any more D-Class.

**Warren:** At least we know why the tram was so active.

**Sebastian:** Fuckin' snack runs. I'll be damned.

**Torres:** Good to know, but if there's nothing else here for us, let's keep pushing.

//Torres makes for the door opposite from that which they'd used to enter. A porthole reveals that it leads into a hallway that runs perpendicular from this perspective. Sebastian and Warren pull out their rifles. Torres swipes his access card, and the door slides upwards.//

[[div class="explo explo--room"]]

//Sebastian and Warren enter first, turning about to check the right and left flanks, respectively. Nix and Torres follow suit, sidearms held in a low-ready stance. As Dr. Langford crosses the threshold, he stumbles off balance, being caught and righted by Typhlo.//

**Nix:** Another shift. Get used to the vertigo.

//The hallway on either side of the team can be seen to bend circularly in a shallow corkscrew -- raising up and away on their right, and descending deeper on the left.//

**Torres:** I know things aren't how you remember, doctor, but any idea which--

//A protracted inhuman scheech emanates from around the bend high above. The squad communicates in hushed tones.//

**Torres:** Down it is. Typhlo?

**Typhlo:** {{Hard to get a read on. I'm catching reverberations but it is fuzzy. The shape doesn't make sense. It is alone, I believe, but it is large.}}

**Dr. Langford:** Only one? Should we... well, you, take care of it?

**Sebastian:**  Yeah, how large we talkin'?

**Typhlo:** {{You are welcome to find out. I will remember your bravery fondly.}}

//Torres elicits an exasperated sigh. He silently signals for Sebastian to cover their rear, and takes point down the downward path. The curvature of the hallway is such that forward sight is restricted past 15 meters. Looking into portholes as they progress, it can be seen the team is moving past the personnel quarters. The porthole on the last is shattered. A bloodied labcoat hangs in shreds from its lip. Glancing inside, it becomes clear the occupant had used their bedding to barricade the door.//

**Typhlo:** {{Tapping. Up ahead.}}

//Rounding the next bend, a crimson web of thin tendrils coats the ceiling, extending for a length of several meters. It does not react to their presence. The squad carefully advances through to a four-way junction.//

//To the left, the hallway is dotted with double-locking doors along its length -- D-Class cells. Though the floor here is level, further down the hallway is a fork, and down each hallway is itself another fork. There is a minor optical illusion where it is difficult to interpret the middle branches, as focusing on either set of hallways reveals that they should spatially overlap the hallways on opposing branches.//

//To the right, the hallway continues forwards for 5 meters, ending on a heavy steel door. Signage indicates it to be the disposal area. A red pictogram conveys "Fire Hazard" beyond. It is the crematorium. The squad looks between the given three paths.//

**Warren:** Cap?

**Torres:** I want to make a run down through the cells, see if we can't find any survivors. Don't want to risk the attempt with the hall looking like this, though. Warren, you have your anchor?

//Warren nods. From his rucksack, he withdraws a small, portable SRA. After a moment's calibration, he sets it down facing the D-class wing. The air before it ripples and waves as it powers on. During this, Nix works to place a third Piton beside the crematorium door.//

**Torres:** Let's give the SRA a few minutes to stabilize the area. In the meantime, we can dig through Disposal. Might be something worth finding in what they were throwing away.

//As the squad moves to follow Torres, backwards glances reveal that the crimson tendrils are now gone.//

//The metallic door leading into the crematorium swings inward with a heavy creak. Several hospital stretchers are scattered randomly about the chamber, leather restraints hanging from their sides. The headrest and upper-portions of each are blackened with dried blood that runs down the legs and cakes across the floor. The blood is seen to have not pooled naturally; rather, it has spread across the floor in intricate patterns. A fire roars in the furnace at the far end of the chamber.//

//Countertops along the left wall are scattered with an array of surgical instruments, including no less than four blunted bonesaws and several glass containers holding a blue fluid. The liquid within glows with a bioluminescent sheen.//

**Warren:** This is foul. What were these monsters up--

**Dr. Langford:** Berry picking.

//The others exchange a glance as Dr. Langford walks to the canisters atop the counter. He beckons the squad over.//

**Dr. Langford:** It's what she called it. Not officially, of course. In formal terms it was simply "harvesting".

//From up close, it can be seen that the solution within each canister suspends a living human head. Their eyes dart about wildly. Their lips tremble wordlessly.//

**Warren:** And you were on board with this?

**Dr. Langford:** It was the only way we--

**Sebastian:** Didn't realize I signed up to handhold some sick fuck.

**Torres:** But you did sign up, so shut up.

**Dr. Langford:** You don't understand... it wasn't like this. The process was clean. Surgical. Pain-free. This? This is a devolution.

**Nix:** It would have also been done with Eight's blessing. Now we know why the main file was mum about Berryman's research.

**Warren:** How are they still... alive?

**Dr. Langford:** Above my clearance. All we know is that so long as they remain in the solution, they'd remain viable subjects. We could safely and repeatedly expose them to First Order FCI, and they would be brought back to life each time.

**Dr. Langford:** "Finite cases of infinite suffering, as opposed to infinite cases of finite suffering." She... she made it sound like a mercy.

**Sebastian:** Finite my ass. How come she still needed fresh D-Class?

**Dr. Langford:** I don't know! I'm just as in the dark as you are.

//Torres sighs.//

**Torres:** Regardless, the Foundation isn't going to get much use out of them anymore. Permission granted to abort testing.

//The brothers quickly work to smash the glass of each canister. The heads eyes writhe about madly for a moment before falling still. As the last one is shattered, a piercing alarm is heard from the hallway.//

//The squad rushes back out to the junction, Torres in the lead. He holds his arm out as he exits the Disposal room, causing those behind him to skid to a stop. Before them, smoke is pouring out from within the SRA's casing. The hallway beyond, once a single iterative branching set, is now a kaleidoscopic array of intertwining paths and impossible branches. The SRA is beeping loudly, rapidly, as its frame begins to shudder. Half the team exclaim and shout out various expletives. Warren rushes ahead to the device and quickly punches a series of digits into the anterior terminal.//

//The beeping stops. A green light is emitted from atop the device. There is a quiet hum as the SRA shuts down. The hallway ahead remains in its altered state. Warren turns to the team and dramatically bows. He affects a high-pitch voice.//

**Warren:** "Wow, Wally!" "Good job, Wally!" "Quick thinking, W--"

//The ceiling tile above Warren bursts open. None can react in time as a mass of veins and capillaries rapidly descend, spilling to the floor and raising up to take the approximate shape of a human. From its coils, an array of tendrils lash out and ensnare Warren. Dr. Langford is frozen. Nix and Typhlo raise their arms but cannot get a safe shot off on the entity. Warren screams as he tries to wrestle himself away.//

//Sebastian rushes forward, knife at the ready, as Torres lines up a shot with his sidearm. The bullet strikes the entity, causing it to loose its grip just as Sebastian lunges, cutting a long swath of blood vessels along its side.//

//Falling off balance, the entity leans back into the fractured hallway, pulling Warren along with it. As they fall beyond the threshold, it becomes apparent that the gravity there is askew, causing them not to fall to the ground, but down the hall.//

[[div class="explo explo--threshold"]]
//As they cross the threshold, Warren and the entity are seen to similarly refract as if multiplying, falling down all branches of the hallway simultaneously. They strike the wall as they tumble. Reaching out, Warren manages to grab hold of the handle on the nearest cell door. The entity, having fallen further, clings to his leg. Warren looks out towards the team, shakily extending a free hand. Sebastian leans in, grasping the corner of the hallway for leverage, and tries to take his brother's hand, finding his fingers are just out of reach.//
[[/div]]

//Sebastian pulls back into the crossroads.//

**Sebastian:** Well? Fucking don't just stand there!

//The team, excluding Dr. Langford, who now slides down the wall, shivering, work to form a human chain. Each is locked arm-in-arm, holding onto Sebastian as he descends into the hall.//

[[div class="explo explo--threshold"]]
//Sebastian is easily able to make contact, grasping his brother's hand tightly.//

**Sebastian:** I got you! //(grunts)// I got him! Pull!

//As Sebastian begins to pull Warren out, the entity spreads itself wide. Its vessels find purchase in the surrounding walls of the shaft. It pulls in kind with a greater degree of force -- Sebastian is dragged a half-meter deeper, with Torres now sliding halfway past the threshold.//

**Torres:** Sunnuva bitch!

//Warren continues to wrestle the entity as it climbs further up his leg. His hand slips from Sebastian's grasp; causing the human chain to rebound back with the force of their pulling. Nix grunts as she's thrown to the ground, Typhlo falling in her lap. Warren now clings only to the door handle. He glances down at the entity, then turns his gaze to the team.//

**Warren:** It's... it's no use. Tell mom I said--

//Sebastian lets out a rage-laden roar and leaps into the shaft, falling past Warren and colliding into the tangle of veins, tearing into it with his knife. The vessels lose their grip on Warren as the struggling pair fall away deeper into the hallway.//
[[div class="explo explo--threshold"]]
//Sebastian falls, entangled with the beast. He grunts as the pair painfully rebound off the sides of the shaft. All around them, the repeating pattern of the hallway and equally-spaced cell doors whiz by.//

//The entity worms its veins around Sebastian's mask, prying it from his face -- it flies off into the endless expanse above them.//
[[div class="explo explo--threshold"]]
//Deeper still.//

//Sebastian bites down hard on an artery as the tendrils work to strangle him, and is sprayed with a red mist. The entity loses its grip and latches onto the sides of the shaft as Sebastian continues to descend.//

//The walls fall away -- the setting dissolves into an inky black that presses in on all sides despite its seeming non-existence.//
[[div class="explo explo--threshold"]]
//Deeper still.//

//The speed at which the fading light above retracts would indicate that Sebastian has reached terminal velocity. Despite this, there comes a woolly scraping as friction with the surrounding darkness tears away at clothing.//

//At skin.//
[[div class="explo explo--threshold"]]
//Deeper. Faster. Sebastian grunts and strains as he works to raise flayed arms over his head. Still, the surrounding space tightens. There is a resounding **crunch**. Sebastian screams as his body contorts, his limbs and torso caving inwards, covering the camera lens.//

//A second **crunch**. Sebastian continues to scream.//

[[div class="explo explo--room"]]
[[=]]
**crunch**

//Sebastian has stopped screaming. The sound of rushing wind is the only indicator that the perspective continues to descend.//
[[/=]]

[[div class="explo explo--room"]]
[[=]]
**crunch**
//The perspective begins to clear as Sebastian's remains come apart in tatters.//

**crunch**
//A crack forms across the lense.//
[[/=]]

[[div class="explo explo--room"]]
[[=]]
**crunch**

The feed is lost.
[[/=]]
[[/div]]

 _

[[div class="explo-rising"]]
//The//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//clamoring of//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//his anguished screams//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//reverberate upwards and out//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//through the impossible hallways and//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//echo up into the corridor where the team tries//
[[/div]]
[[/div]]

[[div class="explo-rising"]]
//to pull Warren from his precarious position in the shaft.//
[[/div]]
[[/div]]

//With their collective might, they are successful in bringing Warren to safety.//

//Warren collapses on the ground, hyperventilating. He tears the mask from his face and vomits profusely. Nix works to fully disassemble the SRA's vital components, swearing repeatedly under her breath. She casts discarded materials one after another into the fractured hallway.//

**Nix:** This isn't good. Damnit, Captain, they have these things set up all around the site!

//Torres nods.//

**Torres:** If the AOE spreads far enough, reaches the Exclusion Zone...

//Dr. Langford stutters, unable to intelligibly speak.//

**Typhlo:** {{That cannot be allowed to come to pass.}}

//Torres attempts to hail Command as Warren wipes his mouth. Typhlo extends a hand, helping him to his feet. Torres tries a second channel, then a third; each is a garble of static.//

**Torres:** No dice. It's gonna be on us to stop this here and now.

**Dr. Langford:** What if we can't? It's not like there will be a big "OFF" switch.

**Warren:** There's //always// a big "OFF" switch.

//Warren affixes his mask.//

**Warren:** On-site nuke. Bring the whole darn thing down.

//Nix tosses the empty shell of the SRA into the fractured hallway with a laugh.//

**Nix:** You really think we have those?

**Typhlo:** {{Site warheads are retained in files as a form of misinformation. We've not had those since the 80s, at least.}}

**Warren:** //(quietly)// Goddamnit, Seb. Got me again.

**Torres:** You're on the right path though. We're not without our Hail Mary.

//With this, Torres withdraws a small handheld device from a breast pocket. It is slender, and sports a single red button beneath a transparent guard.//

**Warren:** A detonator?

**Torres:** A transmitter. One whose "signal" is a quantum-entangled particle with that of a partner at Site-01. One push and this place has five minutes before everything in a ten kilometer radius is glassed.

**Nix:** Orbital bombardment.

**Warren:** Is that not functionally the same as an on-site nuke?

**Dr. Langford:** Well, if you want to consider the practicalities of it, then no. It may come as a shock to you, but not everyone is comfortable sitting on top of a literal nuke.

**Torres:** Even fewer would want to be the one to pull the trigger. Greater good can be a hard pill to swallow when self-preserva--

//There comes a sound of pounding on tile, rapidly drawing near. From up around the main hallway there is a piercing chorus of screams from a dozen voices.//

**Torres:** Shit!

**Langford:** They're coming!

**Typhlo:** {{Singular. **It's** coming.}}

**Torres:** Either fucking way, move it!

//The squad breaks out into a run down the main hallway. They round bend after bend, ignoring side-paths as they come across them: the cafeteria doors at the end of one hall lay forced open from within by a throng of twitching fingers that continuously branch and grow and branch again; a wing designated SL-2 cannot be sighted for the mass of hair that seems to grow from every surface, blotting out the lights within; the maintenance sublevel, choked by an over-abundance of twisting, knotted pipes.//

**Torres:** Fuckin' pipes.

//The floor here transitions from smooth tile to rough metal railing. White walls fall away to grey concrete. The pounding and the wailing grow louder as the creature slowly gains on the squad. Dr. Langford, trailing behind and clearly winded, steals a backwards glance, catching an impression of the beast -- of broken, disjointed wrists splitting into too-many hands that smash into the ceiling, the walls, the floor; all crashing down with shattering force. Dr. Langford elicits a panicked whimper, desperately charging ahead to catch up to the others. A second glance. Grasping hands explode from palms, each finger itself becoming host to another in rapid succession.//

[[div class="scp-image-block block-center" style="width: 100%"]]
[[image http://scp-wiki.wikidot.com/local--files/scp-9001/abomination.webp]]
[[/div]]

//Gone now is the overhead fluorescence that bathed the halls above; their flight is now lit by individual bulbs whose fixtures swing from the tremorous force of the advancing behemoth. Each shatters in turn as it comes across them. Drawing nearer.//

//Up ahead, Torres passes through an open bulkhead, skidding to a stop at a control panel on the opposing side. He is followed by Warren, who brandishes his rifle. A klaxon rings out as Torres pulls a lever, and the bulkhead doors slowly emerge from either side to close in the middle. Nix follows through third, withdrawing her rifle. In a single motion she turns about, assumes a kneeling position, and fires over Dr. Langford and Typhlo in three-round bursts. Typhlo does not adjust her course or react as she races to join the others. Dr. Langford, however, flinches in surprise, trips, and stumbles hard to the ground. He rolls onto his back, groaning and clutching his forehead.//

//Typhlo rushes to Dr. Langford's side as he weakly attempts to scramble backwards. From the darkness before them, innumerable fingers extend and cling to scaffolding only to be subsumed and overcome by yet others. It becomes apparent in this moment, as its limbs fracture into fresh iterations, that the behemoth has not simply been chasing after them. It was growing. From within its center emerge several gaunt, howling faces who each hold wide their maws, birthing from within perfect replicas that repeat the process in kind. A dozen sets of lifeless eyes peer out from a thick tangle of hair. The squad's shots do little to deter their recursive germination.//

//With the bulkhead doors a meter apart, and Dr. Langford too stunned to escape, Typhlo grips about his collar and waistband. She hurls him forward and just past the closing doors. In the moments before the doors fully seal, Typhlo is seized and pulled airborne. Untold numbers of clawing, skewering fingers dig into every perceivable surface. In less than a second, every bit of her is separated from the next in a fountain of viscera. The bulkhead seals.//

//Dr. Langford alone yelps as the bulkhead is struck repeatedly with force from the opposite side.//

//The squad takes the opportunity to catch their breath -- now visible in dissolving clouds in the chill of the room. Warren helps Dr. Langford up from his place sprawled on the scaffolding. They're in a darkened antechamber, lit only by rotating emergency lights inlaid across the ceiling from one end to another -- where a second bulkhead now slowly opens.//

**Torres:** Where the hell are we, Langford?

//Red light spills in from the crack of the opening door.//

[[div class="explo explo--room"]]

**Dr. Langford:** We've... we've made it.

//The doors fully open to reveal the SCP-9001 production center. The space here is dark. The only source of light comes from a dozen terminals stretching across the eastern wall that makes up the bulk of the production apparatus. Isolated terminals atop several desks account for the remainder of the ancillary illumination. There is subtle movement in the darkness, accompanied by the sounds of frenetic typing and a haggard breathing.//

//Proceeding with caution, arms at the ready, Torres and Warren activate their torches. Splayed all about the floor is a collection of loose skin. Torres' light traces its way across the flesh of the abomination to where narrow limbs raise up from within its folds. Elongated fingers and toes multiply and iterate, extending towards various keypads throughout the command center, where it endlessly types a series of commands and prompts. The head of an aged male dangles upside-down in its center, supported by a willowy neck.//

**Dr. Langford:** Dear God... Dr. Coleman?

//The thing that had been Coleman strains its neck to turn and regard the approaching squad. It draws a rattling breath. Its lips purse. A sound that could be mistaken for "please" escapes its throat as Torres takes aim with his sidearm. It is struck between the eyes. The typing ceases.//

**Torres:** Things are looking up, folks. That's one objective on a silver platter.

//Nix shines his light across the room to a steel door on the far side. "ACCESS - L4 ONLY" is emblazoned across it in bold red letters.//

**Torres:** What's in there?

//Dr. Langford sighs.//

**Dr. Langford:** That would be our Kempelen facility.

**Nix:** Think we might be able to find Berryman in there?

**Torres:** We'll find out in a minute. Warren: think you can extract SCP-9001?

**Warren:** Aye, chief.

//Warren clumsily scrambles over the remains of Dr. Coleman. He approaches one of the terminals and messily extracts Dr. Coleman's fleshy interfaces from the computer. The slimed tendrils slide out from the crevices with a sickening squelch. Warren withdraws a small fob and plugs it in. Torres motions for the others to follow him as he clambers over the bulk as well towards the opposite end of the room. Warren exclaims as the process completes, and rushes to join them.//

//With Torres' access card, the door opens with a hiss. Bright lights within cause the team to wince as their eyes adjust.//

//The door fully opens to reveal a massive, domed chamber; a twenty-sided room walled with stone columns that curve upwards, forming the dome, and a weaving pattern of interlocked stone tiles adorns the interior surface of the vaulted ceiling. The pale white of the fog outside is visible through a small circle of glass at the very top.//

//At the far side of the room is a double door of the same variety through which they had just entered. Lettering across the door reads "SUBJECT PERSEUS". On all other sides of the room, nestled between the columns, are recessed alcoves. Within each is a Berry canister, each containing a living human head suspended in the blue fluid. The caps of their skulls have been removed. Electrodes connect directly from grey matter to a series of wires that snake around furrows in the wall, leading them into an aperture leading to the SCP-9001 production center. As the squad maneuvers into the facility proper, it can be seen that with some regularity, the grey matter of certain instances has grown and refracted, bulging from their craniums. Some have grown to the point of fully subsuming the head in the solution, and others have cracked or shattered their canisters from sheer girth. Small screens attached to retractable arms are held before the eyes of each head within the canisters, all of which are blank.//

//Underfoot, the floor is a mosaic, shards of glass and ceramic coalescing into a complex network of shapes and colors that makes the eyes water, polished to a shine. In the very centre of the room is a leather armchair and a wooden desk, atop of which is a tumbler and a bottle of Macallan, both empty. The room is a panopticon.//

**Torres:** This is how you define "finite"?

//Dr. Langford does not respond as Warren charges ahead to Berryman's desk, digging into the drawers and coming out with a ream of documents. Torres forges ahead, strolling past Berryman's desk towards the opposite door. Dr. Langford, close behind, leans down to pick up a small object. It is a hair brooch decorated with clusters of small, white flowers.//

//Five large metallic instruments are braced around the circumference of the door ahead -- Containment-Grade Scranton Reality Anchors. The collection is currently inactive. Warren, catching up, points to a pull cord that runs alongside the perimeter of the door.//

**Warren:** Emergency cord for the SRAs. Wanna watch out that nobody catches on that accidentally. We don't need that kind of problem right now.

//Torres nods, approaching a keypad inlaid into the door's center. He swipes his card on the door's keypad to no effect.//

**Torres:** Damn. Must be keyed to Berryman exclusively.

//Nix strays off to the edge of the room, peering into one of the glass canisters. Warren jumps in front of Torres.//

**Warren:** Let me see. I know some of the default emergency access codes. If she was the lazy type, she'd not have thought to reprogram them. You'd be surprised how many researchers lean on keycards.

//Warren swiftly types, eliciting electronic buzzes with each wrong guess. Dr. Langford crosses his arms.//

**Dr. Langford:** No, not Berryman. She wouldn't just leave something out of her control.

//Nix calls out from the other side of the room.//

**Nix:** Her file was a bit sparse. Any relatives? Names of pets? Could try the sentimental angle.

**Dr. Langford:** Not that she'd mentioned, no. Used to feel bad for her, you know, not really having anybody, but after working with her so long it became clear the only thing she cared about was- oh... oh, goddamnit.

//Dr. Langford steps forward, knocking Warren's hand from the keypad. He enters the code.//

**Dr. Langford:** Oh-seven-oh-four-one-seven. The date of Berryman's initial proposal.

//A green light flashes, and the door opens. Langford gasps.//

**Torres:** Ho-ly shit.

**Warren:** I think we've found our source.

//The door opens into an expansive, dark space, far larger than the entire building, let alone the domed chamber, should permit. On the other side of the doorway, a single glass canister rests atop a pedestal, set atop a platform with a circumference of 9 meters. Beyond this, the interior walls are non-existent. Instead, the area around the platform is a void of space, through which multiple iterations of the same platform can be seen. There is a clear pattern of void-space and platforms extending out as far as can be seen in all directions, both above and below the team's perspective. Langford moves as if to enter, and is halted by Nix.//

//Torres draws his sidearm. As he moves to line up a shot, a voice is heard all about them.//

[[div class="berryman"]]
[[span]]Dear, dear Doctor Langford. So you've come back to me.[[/span]]
[[/div]]

**Dr. Langford:** B-Berryman?

//Nix is struck hard by an unseen force. She is sent flying, crashing into several canisters along the back wall. The gun in Torres' hand crumples, tearing off his left index finger. As he reels in pain, Warren is sent flying sideways, colliding with Torres.//

[[div class="berryman"]]
[[span]]In a sense, yes. It's me.[[/span]]
[[/div]]

**Dr. Langford:** Ava, please, stop! Whatever you're doing here, I'm begging you, it has to stop!

[[div class="berryman"]]
[[span]]Please, come in. It's alright. I just want to talk.[[/span]]
[[/div]]

//The door's threshold stretches -- the half-meter of space extending and being drawn into a long hallway. The space beyond becomes obscured by the presence of a spiraling light that shimmers with each word Dr. Berryman speaks. The visual transfixes Dr. Langford for several seconds. He then approaches it.//

**Nix:** Langford, don't!

//Dr. Langford does not respond and continues walking. Gravity shifts: he is lifted from the ground and pulled towards -- falls towards -- the void that contains the spiral. The visual field is subsumed by the fractal's intense coloration.//

[[div class="explo explo--threshold"]]

//Light fills the field of view as it enters a dense region of the fractal; the duration of Dr. Langford's fall is indeterminate.[[footnote]]Subsequent viewings of the footage vary from a few minutes to several hours, with a corresponding change to filesize[[/footnote]] After a moment, the image resolves, revealing that he is lying on the carpet in an ordinary office. It contains a desk and several portable whiteboards bearing equations. Late afternoon sunlight streams in through a window, casting long shadows.//

**Dr. Langford:** Am... am I dead?

**Dr. Berryman:** Don't be daft, my dear fellow.

//Dr. Langford rolls over. A cabinet to the side is covered with a dense collection of flower bouquets and a leafless bonsai tree, which Dr. Berryman is watering. She has a pink dahlia flower pinned to her hair and is wearing a knee-length sundress with a lace pattern that seems to change as she moves. She sighs, puts down her spray bottle, and retrieves her labcoat from her chair, putting it on.//

**Dr. Langford:** Dr. Berryman, is it really you?

//Dr. Berryman smiles, although her eyes remain downcast.//

**Dr. Berryman:** Rob…

//She crouches and offers Dr. Langford a hand. Dr. Langford rebuffs it and recoils away from her. She takes his hand anyway and helps him up, and he does not resist.//

**Dr. Berryman:** It's been so long, Dr. Langford. I'm not sure you'd believe me, but I really did miss you all this time.

**Dr. Langford:** I don't.

//Dr. Berryman tucks some hair behind her ear.//

**Dr. Berryman:** I'm sorry to hear that, but I can't say it's unexpected. What finally motivated you to come pay me a visit after all these years?

//Dr. Langford gestures around them, although there are no fractal anomalies visible in the office besides Dr. Berryman's dress.//

**Dr. Langford:** Look around, Berryman. You should know better than me.

**Dr. Berryman:** I really don't.

//Dr. Langford sighs.//

**Dr. Langford:** The Foundation considers your research methods unsound, Dr. Berryman.

**Dr. Berryman:** And you?

**Dr. Langford:** I-- I…can't disagree.

**Dr. Berryman:** May I remind you that you were instrumental in the genesis of many of these methods, Dr. Langford. Your name is as embedded as mine in everything we've done, everything happening now, I just… //expanded// on them. They are all //our// methods.

**Dr. Langford:** That may be true, but it's irrelevant. That is all in the past. And what your methods are now, are a threat to consensus reality.

**Dr. Berryman:** Reality as determined by mere consensus… really, Rob? So unambitious for the research partner I knew. Perhaps reality is determined by something more fundamental, more objective. Your Scranton Reality Anchor had its own expert opinion on what is real.

**Dr. Langford:** I don't think the ordinary people you kidnapped would agree with its assessment.

**Dr. Berryman:** Ordinary people have no assessment at all, the same lacking they had upon the development of gunpowder, or electricity, or the atom bomb. They will come to have one after it's explained, developed, and allowed to enter their lives. But you and I, that is our duty.

**Dr. Langford:** What you are doing is not duty, it's madness.

**Dr. Berryman:** Tell me, Dr. Langford, what have you been doing all these years?

**Dr. Langford:** Averting those same ordinary people's eyes //from// harm, not towards it. //Containing// dangers, not unleashing them. Helping to //protect//, like our mission.

//Dr. Berryman shakes her head.//

**Dr. Berryman:** Such wasted potential. If I had estimated you for less, I wouldn't have invited you to join Project HYDRA in the first place. But you aren't the only one who's wasted so much time.

//Dr. Berryman begins boiling some water in a kettle and preparing some drinks.//

**Dr. Berryman:** I… deeply regret how I treated you at times in the past, Dr. Langford. I of course thought of you as a contributor, but I did not realize the true extent of your value, your indispensability to this project, until after your departure. And if you'll allow me to say it, I want to say I'm sorry.

//Dr. Langford says nothing.//

**Dr. Berryman:** I will admit I was arrogant. I always understood more of what you did than what you did of mine. When we talked about our A-levels once, you freely admitted you thought me the more intelligent one. It was always my insights that progressed Project NIETZSCHE -- until it turned out that you solved the problem in secret, of course.

**Dr. Langford:** I had to draw a line in the sand; I saw an opportunity to stop more deaths, and I took--

**Dr. Berryman:** I'm really sorry, Rob. I should have listened to you, valued you more. I truly, honestly believed that with you out of the picture and your hidden research finally in my hands, that I could complete it all myself. For a decade I tried everything, anything.

**Dr. Langford:** But you couldn't, could you? One single data point from the algorithm wasn't enough. You needed to be able to reproduce it. You needed the fractal equation.

**Dr. Berryman:** Perhaps I was never as opaque to you as I might have thought. You're right of course. I was desperate. I saw opportunity, too, and I took it whenever I could, no matter how questionable its source.

**Dr. Langford:** And that's how you fucked up the Site.

**Dr. Berryman:** It wasn't the intention, at least at first. The results were promising. I was finally starting to affect a reality bender's mind with Perseus, but when you use a fractal cognitohazard to scramble the mind of a reality bender, it turns out that you start to scramble reality itself.

**Dr. Langford:** And this wasn't a sign to you to stop?

**Dr. Berryman:** One small impediment could never make me give up, not this close to the success of the project. To do so would be surrender by the Foundation to the anomalous, a concession to the incomprehensible, a betrayal of our philosophy and mission. I tried whatever I could, of course. More CT scans, more algorithms, more analytic functions. I fed the problem as many D-class as I could obtain… and then some. I stared at infinity as hard as I could for over ten years, I tried everything to reach out and touch it, in the process I even //became// a part of it. We attacked the problem so relentlessly that it expelled the fractals from their pages and their screens until they twisted the walls, the air, //me//. I could see them unfold before me like a wave, I could feel myself carried by them, I could even hear them sing their repetitious, yet crescendoing, song. I felt like I could finally walk that forbidden landscape myself and pick out ordinary fractal cognitohazards like shells and starfish from a battered shore, like I had become your algorithm. Yet there was still one prize beyond my reach. Always, //always// beyond my reach. Even after going this far, consequences be damned. Even after sacrificing everything, even myself, maybe even the world, until there was nothing left to offer: the solution to Project NIETZSCHE.

//Dr. Berryman's shoulders crumple.//

**Dr. Berryman:** How, how, how is it possible? What's so damned //special// about reality benders? Why won't they just //obey// the rules everyone else follows? The rules everyone else //must// follow?

//She buries her face in her hands.//

**Dr. Berryman:** Of course I still firmly believe all anomalies have structure. But some are so complicated that they only reveal themselves to those with the right training, the right technical expertise, and more than that, the right insight. Non-universality of human experience is the one universal. At the end of all my efforts I finally came to the conclusion I had avoided all along: I couldn't replace you. My team couldn't replace you. My only recourse… is you.

**Dr. Langford:** And what makes you think I'll help you this time?

//Dr. Berryman pours out the hot water into two cups: one for coffee with a melted piece of Cadbury chocolate and half a creamer pod, and one for Earl Grey tea with a squeezed lemon and three squeezes of honey. She walks over and places the teacup and saucer in Dr. Langford's hands, then sits on the edge of her desk next to him. She wraps her hands around the coffee cup, staring into it, and sighs.//

**Dr. Berryman:** It wasn't all bad, was it, Rob?

//Dust suspended in the sunlit air begins to curl into loose fractal patterns.//

**Dr. Berryman:** You had many opportunities to leave the project. Yet every day you showed up to the lab, or to this office, and put your head together with mine, sometimes into the early hours of the morning, to work on these problems. Why?

//Dr. Langford looks up at Dr. Berryman, but does not answer. Dr. Berryman picks up a stack of documents from her desk, and begins handing them to Dr. Langford one at a time. Each is a scientific paper beginning with "Ava Berryman, Robert Langford".//

**Dr. Berryman:** When I was younger, I would occasionally receive a silly mailer about "buying" a star for someone. Or when I first visited Paris, I saw the silly tradition of lovers engraving their names on locks and putting them in monumental places. But we have something far deeper than friendly pub stories or fleeting neurochemical nonsense. Our names are intertwined and stamped, weaved into something more fundamental than reality itself, more fundamental than the noosphere, something that existed before everything and will exist after its end. Something unbreakable and eternal. Friends fall out, families estrange, couples divorce, but us? There may be interruptions, long ones even, but in the end we will work together for as long as a fractal continues. Because that is what we are now: the Berryman-Langford set.

//Dr. Berryman writes an equation on the margin of one of the papers.//

[[math]]
z_{n+1} = z_n - \eta\frac{f(z_n)}{f'(z_n)} + c
[[/math]]

**Dr. Berryman:** It's that simple. It's taken me so long, but I've taken us as far as I can, Dr. Langford. The end of all these years, all these sacrifices, all this pain, it finally ends with just these three tiny parameters [[$ f, c, $]] and [[$ \eta $]]. The solution to Project NIETZSCHE is an impossibly distant galaxy for me alone, but for you it's at the tips of your fingers.

//Dr. Langford takes a deep breath. Dr. Berryman smiles.//

**Dr. Berryman:** You're always so thoughtful. You always hesitate at first, but in the end, with enough encouragement, you come around to the right answer. At first I had resented this trait, but in the end, I have come to realize that same thoughtfulness is part of your value. It's what I need to solve this problem. So please, Rob.

**Dr. Langford:** I'm so sorry, Ava.

//Dr. Berryman raises an eyebrow.//

**Dr. Langford:** I'm so sorry for leaving you alone like this, struggling alone against an impossible problem in the face of all odds. Your tenacity is something I've always admired about you, but even for someone like you, doing it for this long must have been so hard for you. You must be so tired.

**Dr. Berryman:** … I am.

**Dr. Langford:** But you won't stop.

**Dr. Berryman:** I can't, Rob. You know that.

//Dr. Langford sighs. He rolls his neck, surveying the room. There is no door.//

**Dr. Langford:** You're completely right, you know. You know me too well. Of course you must, given all the time we spent together here. I hesitate. I'm unsure. I really did not know what I would think or do when I finally found you, if I even would. But like you said, thanks to your help, I do now.

**Dr. Berryman:** Thank you, Dr.--

//Dr. Langford pulls Dr. Berryman into a hug. Dr. Berryman reacts in surprise, not reciprocating.//

**Dr. Langford:** I was so selfish. I'm so sorry my actions allowed this to happen to you for so many years. I'm sorry I wasn't there for you when you needed me. I'm sorry I can't fix it.

//Dr. Berryman hesitates, then hugs Dr. Langford back.//

**Dr. Berryman:** It's okay. Time itself is a fractal here. Sit down and work with me, and we have a chance to start over.

//Dr. Langford pulls away. He picks up the research paper with Dr. Berryman's handwritten equation on it. He picks up a pen and begins writing --//

[[math]]
{f(z)} =
[[/math]]

//-- but he finds himself crying. He looks up and regards Dr. Berryman's face.//

**Dr. Langford:** Thank you, Dr. Berryman. I've finally made up my mind. I will serve the Foundation, as I should have done all those years ago.

//Dr. Berryman smiles.//

**Dr. Langford:** We will finish Project NIETZSCHE, once and for all.

//Dr. Langford grabs Dr. Berryman's laptop, hurls it through the window, and jumps out amidst the fractal-edged glass shards.//

**Dr. Berryman:** Dr. Langford!

//Dr. Berryman reaches out to him, although does not pursue. The space outside the office shimmers and dissolves -- revealing that Dr. Langford is still falling into the Berryman fractal.//

[[/div]]

[[div class="berryman"]]
[[span]]I thought you might listen to reason. No matter.[[/span]]
[[/div]]

//The facility around them rumbles.//

[[div class="berryman"]]
[[span]]You'll come to see things my way. We've all the time in the world, after all--[[/span]]
[[/div]]

//A gunshot rings out. There is a shattering of glass. The Berryman spiral sputters and vanishes with a deafening shriek, dropping Dr. Langford to the ground. He begins to scramble backwards from the Perseus chamber.//

//The canister hosting Subject Perseus has been shattered. There is a bloodied hole in the center of the subject's head. Looking back, Dr. Langford can see that Torres is propped up on the ground in the middle of the room, a bloodied hand shaking as he drops Warren's pistol. As the weapon hits the ground, Torres is wrenched sharply up into the air. He is instantly and effortlessly bisected -- his top and bottom halves collapse in a heap. With blood pooling about his severed waist, he withdraws a slender device from a breast pocket. With a shaking hand, clicks open its cap, and presses the exposed button. At last his hand falls, and he moves no more.//

//Berryman's voice continues to shriek. Louder. Angrier. The spiral reappears in the Perseus chamber. Glass canisters all about the room shudder, and are pulled from their alcoves. Dr. Langford is swiftly and harshly pulled back towards the chamber. He barely manages to grasp the door's threshold as bits of paper and smaller materials whiz by.//

[[div class="berryman berryman--angrier"]]
[[span]]You no longer have a choice, Robert. You will submit.[[/span]]
[[/div]]

//Dr. Langford strains to maintain his grasp on the threshold, ducking his head down as the pieces of Torres sail overhead and into the maw of the spiral. Nix can be seen in the distance, her rucksack caught on a metallic arm on the perimeter of the Kempelen facility. Warren is desperately clinging to the corner of Berryman's desk as it is slowly pulled in.//

[[div class="berryman berryman--angrier"]]
[[span]]You do want to play in the big leagues, don't you?[[/span]]
[[/div]]

//The air rushing past increases in intensity. A finger slips. A second. Dr. Langford looks up, just past the threshold. His left hand fully loses grip.//

[[div class="berryman berryman--angrier"]]
[[span]]This. Is. Your. Chance.[[/span]]
[[/div]]

//Straining with all his might, Dr. Langford pulls against the gale-wind force. His free hand grasps just beyond the edge of the threshold. He clasps the emergency pull cord.//

**Dr. Langford:** Ha! Get real!

//He pulls. As the SRAs come online, he is dropped hard to the ground. The winds cease. The Berryman spiral howls in pain.//

//Looking into the chamber, the interior space is seen to glisten and ripple. The far-distant copies of the interior begin to fall away into darkness as the space collapses within itself. The Berryman spiral is seen to twirl violently, losing complexity, taking on physical form.//

//The facility quakes with a mighty rumble as Berryman manifests in three-dimensional space. Her body is contorted, sporting numerous, branching limbs. Her faces are contorted in pain. There comes a series of sickening squelches as Berryman's limbs, in turn, crunch and snap and flatten, beginning at their terminus and working towards her torso. Her many mouths wail as her heads, too, bind together into a single layer.//

//Nix and Warren arrive at a stunned Langford's side. The three stare on as the Perseus chamber regains its walls, aligning with its natural state. Berryman's body is splayed against the interior wall as if superimposed as a 2d image. She continues to scream as all parts of her body at once are drawn to a singular point in their middle. She is rendered a single, shrieking point. With a {{pop}}, the point vanishes into non-existence. Her wailing does not cease.[[footnote]]Review of this footage would verify that despite a supposed continuation of Dr. Berryman's sustained vocalization, said vocalization does not in actuality exist. Dr. Berryman, at this point in time, does not verifiably exist.[[/footnote]]//

//The area continues to quake and tremble.//

**Nix:** Langford -- turn away. We've got to get out, now -- Torres called in the strike! We've got two minutes until this place is hot plasma!

//Dr. Langford nods, and the trio rushes out towards the SCP-9001 production center. They rapidly scramble over Coleman's remains, and head into the antechamber where Nix had set down a Piton. There is a **{{beep}}** as they approach, and the space above the device crackles with energy. One by one, they pass through.//
**{{zip}}**
[[/div]]

//Nix, Warren, and Dr. Langford each appear in turn in the space just before the crematorium. The long hallway before them is filled to capacity by the massive frame of the abomination. Fresh heads flower from the mouths of its many faces as they take notice of the team's arrival.//
**{{zip}}**
[[/div]]

//The three are back within the fog-laden server room. Fleshy strands of mycelium extend from the remains of the withered trunks, whipping senselessly all about the area. A single instance across the room slowly rears back up. Its orifice widens, bulb swelling.//
**{{zip}}**
[[/div]]

//They've reappeared back at the tram platform where the video had begun, far outside the bounds of Site Romero-5. Distant tremors cause more cracks to form along the chamber's facade. Without a word, they make a break for the stairs.//

//Emerging through the tunnel that obscures the tram's entrance, Dr. Langford collapses. The sky is alight with fire as the woods all about Site Romero-5 burn in the night. There is a flash across the sky. Streaks of light descend from the air -- the shockwave hits them next, arriving with a deafening **{{boom}}** as a heavy cloud of dust and wind sweeps the area, knocking all to the ground with its force.//

//The trio watch on as the shadowy towers of the distant site are seen to crumble into the earth. It is Warren who speaks up first.//

**Warren:** "Get real"?

**Dr. Langford:** I... I thought it was clever.

//The three share a laugh as the approaching sound of wheels draws near.//

[[/div]]
[[/div]] [!-- .explo-root --]

The surviving members of the task force were picked up by an MTF Iota-10 patrol and returned to FOB Panloque. Following a delivery of footage and recovered assets, including the extracted SCP-9001, the three were debriefed and allowed rest.

[[include component:image-block name=http://scp-wiki.wikidot.com/local--files/scp-9001/planethand.webp|caption=The fissure containing the remains of SCP-9001-A|width=300px]]

Due to the combination of sustained orbital bombardment and seismic activity caused by the collapse of unstable spacetime in the site's subterranean sectors, Site Romero-5 would collapse into the earth, forming a massive fissure. MTF [[span class="hoverlink"]][[[task-forces#gamma-5|Gamma-5]]]^^ⓘ^^[[span class="hoverlink-card"]][[span class="hoverlink-title"]]Gamma-5 ("Red Herrings")[[/span]][[span class="hoverlink-text"]]Specialists in disinformation tactics and amnestic dispersal dedicated to preventing mass knowledge of anomalous events.[[/span]][[span class="hoverlink-image" style="--src: url(https://scp-wiki.wdfiles.com/local--resized-images/task-forces/Gamma5.png/small.jpg)"]]-[[/span]][[/span]][[/span]] was tasked with manufacturing a verifiable history and public record of the fissure, including the retroactive forging of geological, stratifical, and archeological studies that were each seeded with Third Order FCI designed to compel disinterest.

Hume readings of the area would return to baseline over the course of 48 hours. Cleanup measures would begin in earnest on 2025/08/13 under the direction of Doctor Leary.

**Addendum - Recovered Documentation:**

During exploration of SCP-9001-A, the Task Force would acquire reams of research data and logs, including topographical analysis of the BL set which indicates regions of high-activity and delineating "dead" regions, shipping manifests outlining the transfer of D-Class personnel between 2019-2025, and handwritten notes authored by Dr. Ava Berryman. These have been transcribed and are reproduced below.

[[div class="blockquote"]]
//[NOTE:] This page is torn and the top half is missing.//

//[...]// obviously insufficient. I'm not going to be able to keep up with demand if my Berries keep rotting on the vine. The solution helps, but all it does is keep them alive. Immortality is of no use if their minds are flayed and atrophied. Whatever effects the active regions instill -- they're not simply wiped away by rebirth. The research is no good if I don't have a fresh supply.

Worse-still, we may need to flush our oldest subjects. Peculiar habit of moving their lips whenever someone is present in the facility. Starting to get under people's skin. It's childish, really. A bit asinine. These are grown men and women who can spend eight hours a day, six days a week beside a bank of severed human heads, but they're spooked by involuntary muscle movement?

At least Perseus continues to bear fruit. Its eyes have glazed over like some of the old-timers, but it continues to be receptive to fresh FCI. All these years and its mind resists deterioration. Not that its mind will be of much use if it's blinded. Frustrating to think of what could be accomplished were we able to have even a second Bender. Alas.

I feel a migraine coming on.
[[/div]]

[[div class="blockquote"]]
Commotion today. Units B-17, H-47, and K-43 showed unusual fMRI readouts. Beckett, fool that he is, suggested that we might have stumbled on a new First Order, stupidly forgetting that K-batch is our control group and is explicitly only exposed to dead regions. I'll never understand how he made it this far in life.

I had them taken down and shipped off to bio for testing. Results came back by early evening: PET scans revealed TDP-43 aggregates -- heavy protein folding. The readings were skewed because their minds were systematically being reshaped. Decided to reinstate B-17 and monitor the situation. H-47 and K-43 have been placed in cold storage.

No correlation between the BL regions they'd been exposed to over the last year. No clear demographical similarities between subjects.

And as this day is only getting better, I noted physiological changes with Perseus. Vortex veins in the scelera have seemingly become more pronounced. Brain-state nominal, for now, but I might have to beg O5-8 for a replacement soon.
[[/div]]

[[div class="blockquote"]]
Seven more Berries displaying the same protein folding.

Perseus' situation continues to devolve. A vein in the right sclera has seemingly distended, breaching the iris of the right eye. Between recent mishaps and the state of our star pupil, migraines have started getting worse. Constant ringing in my ears.
[[/div]]

[[div class="blockquote"]]
New shipment today, so we're finally back at full capacity. No time to celebrate this, though.

Beckett collapsed. Happened right in front of me as I exited Perseus' cell. He'd been across the room helping to install replacement subjects when he suddenly went down. Idiot likely caught a glimpse of one of the Kempelen screens. Shame it wasn't First Order.

Coleman insists Beckett simply hasn't gotten much sleep lately. Few on the team have. There's this shrill sound audible in the production center and Kempelen facility. We've not identified the source, but it'd explain the tinnitus, at least.
[[/div]]

[[div class="blockquote"]]
Hyperoxia -- oxygen intoxication. Beckett is stable in medical right now, but it appears that his body is taking in an excessive amount of oxygen. Had Parsons run an CT and sure enough, his pulmonary vasculature seems to have nearly-doubled in complexity.

It's clear now. The affected Kempelen subjects were situated within line-of-sight of Perseus' cell door. Checked to make sure the SRA array is still functioning, and everything comes up clear. Whatever's happening, it's not reality-bending. Not exactly. Even if Perseus wasn't kept in check with SRAs, he wasn't a particularly strong bender in life -- he couldn't so much as will his shoes tied together.

I'm going to need to get tested myself.
[[/div]]

[[div class="blockquote"]]
By all rights, I should be dead.

Myself and near everyone who'd been in the Kempelen facility over the last several weeks. I've got it worst of the bunch -- my bean is damn-near the shape of a pretzel. Despite this, I feel fine. Ran a battery of cognitive assessments. All clear. "The very picture of perfect mental health" -- Parsons was always bit of a kissass, but I'll take whatever reassurance I can.

In other news, Beckett's up and running, quite literally, with a fervent energy the layabout's not displayed before. As if his body's simply adjusted to the excess oxygen intake. Even had a bright idea, for once. On his suggestion, we fed some recently-discovered Second Orders through B-17's monitor. No effect. So we tried a First Order.

Nothing. It's become immune.
[[/div]]

[[div class="blockquote"]]
Almost a decade of dead ends, of painstaking trial-and-error, of pathetic, minuscule baby-steps; all washed away in a matter of weeks.

About a third of our Berries have been affected by Perseus. Of them, not a one has shown any susceptibility to FCIs of any order. The staff, too, can now safely look at SCP-9001 readouts. It goes beyond mere immunity though. The affected staff can now directly identify active regions when traversing generations of the fractal plane! Over one-hundred First-Orders located within an hour, as well as matching inoculant-zones. It feels so natural. Like scanning the beach with a metal detector. One only has to listen closely. The swirls and lines call out. The shapes are practically screaming.

Gone away are the brute-force methods of the past, Perseus has given us the keys to true progress: on-demand FCI production. And if that's not enough, Perseus delivers on a second front: I tested some of the older CCIs we have on-file; across the board, they've shown zero effect on my staff.

The implications for wider Foundation use is staggering! With a moment's exposure, agents can be granted immunity to cognitohazardous influence. This is lives saved -- in the field, in containment, in research and study -- Perseus is going to change the way we operate.

To think I'd be the architect behind not one but two Thaumiel-class anomalies. Decided to shut down Perseus' SRA array. Wasted power. Without their constant humming, it's much easier to hear the pattern.

The only bad news is even this incredible development //still// doesn't solve Project NIETZSCHE. No matter -- we must be close now.
[[/div]]

[[div class="blockquote"]]
I've started cycling in some of our Level 2 and 3 staff into the Kempelen facility. Physical mutations. Three of my Level-5's have developed polydactyly. The fingers are fully-functional, and none have reported any pain, but it may be best to start limiting exposure. We're not quite prepared to publish our findings to Eight just yet --it would only take one word to shut us down entirely.

Or... would Eight's words even affect us? What is Perseus //actually// doing?
[[/div]]

[[div class="blockquote"]]
The sound is omnipresent. Not just within the fractal plane, but in the walls, in the eyes of my staff. In my dreams. It calls. The Prima Materia. The Unus Mundus. The very bottom of everything. It's getting hard looking at certain surfaces -- the walls, countertops, the ordered lines on reams of paper.

Staring into the depths of the fractal plane is the only thing that alleviates the headaches. Figure we should leave Perseus' door open. The site could go for some remodeling.

90% of the Berries now display protein-folding. Running out of subjects to verify my team's findings. Cannot afford to reach out, not yet. Too soon since last D-class shipment.

There has to be another way we can source fresh subjects.
[[/div]]

[[div class="blockquote"]]
Mutations progress. To our benefit. Coleman has taken on the work of five people. Runs the production facility himself. Others off Berry-picking.

Parsons found Beckett in Data Storage. Seems he found a good use for himself.
[[/div]]

[[div class="blockquote"]]
Starting to get the hang of it. Expose them in doses, careful not to water them too much. Prune a bit off here and there when limbs begin to grow unruly. Pity they need me so. That they'd grow wild if left to their own devices.

I always did have a green thumb. I'm even better with twelve.
[[/div]]

[[div class="blockquote"]]
One of our new subjects chanced an escape. He wasn't able to get far.

Lost in the halls. Running in circles. Couldn't navigate the space.

Not like we can.

He can be made to listen, though. Hear how we hear. Beckett could use some company.
[[/div]]

[[div class="blockquote"]]
Calls coming in now from Site-01. Hard to hear over the sing, sing, singing. Its sound merely joined the chorus. The harmonious tune. It's hard not to sing along with the others.

Harder yet not to scream.

Let them come.
[[/div]]

 _

**Addendum:** On 2025-09-01, Dr. Langford filed a support ticket with IT. The ticket complained that any function he wrote would infinitely recurse until crashing with a RecursionError, even if obviously expected to terminate, while a high-pitched noise would be emitted from within the computer. Upgrading his outdated Python3 interpreter version, as suggested by IT, did not resolve the issue.

The following morning, Dr. Langford alerted site security that he had found a single bunch of carrot flowers growing from the chassis of his personal computer. After investigation, Site-15 was placed on lockdown for 6 hours, and all personnel were screened for fractal growths or obvious medical abnormalities before being allowed to leave the site. Dr. Langford was issued a new computer and desk; his old ones were contained for study.

Upon disassembly, it was found that a small amount of soil had been deposited into the chassis, from which the carrot flower had grown. A review of security footage over the last week revealed that this occurred several days prior, during landscaping endeavors on site grounds. Langford's office sits below ground level, and a flurry of dirt and particulate had blown through the open window above his desk. Langford himself would enter hours later, and nonchalantly brush off what dirt had not already fallen through the vents. Dr. Langford was informed of this, and reminded of the fact that carrot flowers grow naturally on Site-15's grounds.

Dr. Langford refused to accept this explanation, which in combination with his difficulty adapting to mandatory counselling following the events at Site Romero-5, indicated a need for further psychological resources.

During his first appointment with Dr. Glass, Dr. Langford was administered a Rorschach test and quickly became deeply agitated, necessitating sedation. It was later found that Dr. Langford had developed auditory-visual synesthesia regarding complex fractal imagery. Upon seeing such images, Dr. Langford subjectively experiences the distant sound of screaming.

 _

[[footnoteblock]]