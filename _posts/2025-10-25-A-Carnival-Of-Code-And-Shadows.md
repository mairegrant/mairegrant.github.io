---
layout:     post
title:      "The Bug Detection Roller Coaster: A Carnival of Code and Shadows"
published:  true
---

![RollerCoaster1](/assets/rollercoaster1.png)

# The Bug Detection Roller Coaster: A Carnival of Code and Shadows

The carnival gates creak open slowly in the warm twilight fog, the park is abandoned. Offside is a rickety wooden tracked roller coaster with graffiti over the booth. As the gates crawl further apart the sound of electricity and old code humming quietly with secrets can be heard. The sign flickers on — “Bug Detection” — a ride of iron and whispers, the fluorescent orange bulbs glittering like blinking eyes. Dishevelled paper streamers and faded flags hang off decorative Victorian style lampposts.

Step right up — for this is no ordinary ride. No, this is a plunge into the uncanny valleys of software testing. You know you shouldn’t, but your feet take you to the direction of the car whispering towards you in the fog and soon you are strapped and on your ascent. The climb is slow and then faster and then slow again, there is a chill in the air now. Below the tracks bugs of all shapes and sizes scuttle around hurriedly into the shadows before it is too late, but they have been spotted, and they are everywhere. Every click, the roll of the track pulling you into a black velvety darkness.

You are plunged downwards in one quick movement into the valley of familiarity where everything looks… ordinary. Where have the bugs gone? The code hums to you, a soft lull. White noise in the background. Bugs crouch in the corners, grinning like porcelain dolls with cracked faces and sharp teeth. You struggle to see them behind the glamour now even though you’ve seen it a hundred times. This is the trick. This is how they hide.

The track twists into a loop. The car jolts faster now, the sticky, sickly smell of candyfloss and popcorn permeate your senses and suddenly you are upside down. Your thoughts are too, spiralled and anchored to old assumptions, tangled whispers of “it’s fine, it’s always been fine, that’s just how it works, it’s always been that way…” The mirrors here are cruel, they show you what you expect to see and not what is really there. The bugs are laughing now. They scuttle around faster, vibrating with energy, laughing in metallic tones. They laugh; they laugh because they know you have stopped looking.

You close your eyes; the ride will be over soon. The track rises, high above the abandoned theme park. You open your eyes as the track rises into the mist. Up here the air is thin and cold, but you can see everything. You’ve learned the patterns, the secret doors, the sigils, their names. There they are — the ghost bugs. Ancient, clever and stitched into the bones of the system. They don’t want to be found. The car rattles to a halt. The carnival isn’t finished with you. Your knuckles are white on the cold iron bar, and you can feel it, etched into the cool metal. The bugs are still there. They have retreated for now, but they are there, in the bolts, in the shadows, in the hum of the tracks. As you step off the only thing you know for sure is that you will be back and you will ride again.

![RollerCoaster2](/assets/rollercoaster2.png)

I recently visited Japan and we passed by Fuji-Q Highland, guilty of not doing enough research beforehand we skipped it due to time constraints and afterwards was met with FOMO (thanks TikTok) when I learned that Takabisha is the second steepest roller coaster in the world and the park is famous for being some of the highest, fastest and steepest coasters in the world.

Channelling that FOMO + excitement for Halloween I combined my inspiration to talk about something I love almost as much as roller coasters — finding bugs. Recently joining a new team I’ve been met with the common adages and coming in as a set of “fresh-eyes” really struck a chord with me this time.

I know the value of fresh-eyes on an application but how do we maximise the effect of this phenomenon?! Bug detection rate starts high when testers have “fresh eyes” and this gradually declines over time as the tester becomes familiar with the domain, bug detection then stabilizes before typically gradually increasing due to deeper insight.

As domain knowledge and system familiarity increase then bug detection can be seen to start plateauing. This might look something like this where 0 represents the business-as-usual defect logging rate.

![RollerCoaster3](/assets/rollercoaster3.png)

The fresh-eyes phase is high for the first few weeks due to a combination often of novelty, unbiased perspective, determination to learn (feeling inspired) and questioning logic to ascertain understanding. The time frame above is hypothetical as onboarding and complexity will differ from project to project.

How does this work?
Novelty triggers “system 2 thinking” (deliberate and analytical) before mental shortcuts take over and dominate. Having a lack of domain familiarity means that testers question logic and assumptions, hence finding more issues. Over time pattern recognition techniques and habituation reduce anomaly detection unless this is countered by structured techniques.

We can typically think of the “fresh-eyes” effect wearing off as a series of stages.

“Fresh-eyes” phase — high defect rate

2. Decline phase — defect rate lowers as testers become accustomed to quirks

3. Stabilization phase — defect rate drops to a normal level that others may have been targeting before

4. Deep insight — as domain knowledge and logic grows bugs detection starts to trend upwards again albeit at a slower rate.

To think of this in terms of formula for observability and testing we can map to the following two parts. Domain knowledge and bug detection rate.

Domain knowledge:

![formula1](/assets/formula1.png)

Domain knowledge (time)

Starts at 0 when time t=0 (tester knows nothing about domain).

Grows fast at first as learning is fast in beginning due to novelty.

Slows down and approaches 1 (a plateau) as time progresses because there is a limit on how much domain knowledge can grow.

Use exponential as learning curves often follow this pattern with rapid early growth and then diminishing returns.

0.3 here is representative of the growth rate but a bigger number means that domain knowledge grows faster and reaches plateau faster. A smaller number here represents slower learning. 0.3 domain growth gives a curve that knowledge grows quickly in the first few weeks and then slows down which is typical of onboarding patterns.

Bug Detection Rate:
![formula1](/assets/formula1.png)

Bug Detection Rate (time — in weeks here)

0.8 is the starting bug detection strength which is often high in the beginning (this differs for every application)

0.4 is the decay speed, a larger number represents a faster drop in bug detection and a smaller number represents a slower decline.

0.2 is the size of the late-phase bump (how much improvement that additional domain knowledge brings).

0.1 is the width of this bump — a larger number is a narrower bump which is a short improvement while a smaller number giving a wider bump is a longer improvement phase.

t-10 = the centre of the bump around week 10 in this example

In short we are focusing on the variables of

how fast knowledge grows
how fast early bug detection fades
how wide the late improvement phase is
the values substituted are hypothesized parameters to illustrate the concept

To put this metric detection into practice and to validate as a study against real-world data we should collect:

Defects found per tester per time unit (e.g weekly or sprint based)
Severity distribution (critical vs minor to monitor if fresh eyes finds more obvious issues early)
Defect discovery date (to plot detection rate over time)
Defect type (UI, functional, integration etc to monitor if later phases with higher domain knowledge garner more systematic bugs).

As domain knowledge is harder to quantify, we can use proxies such as:

Time in project (weeks since onboarding)
Training completion percentage (if applicable) e.g courses, documentation read
Code coverage or feature coverage (how much of the system the tester has explored)
Peer review scores or knowledge assessments (optional but could be used for calibration)

Compare predicted vs actual bug detection rates. Adjust parameters in line with organisational differences.

![RollerCoaster4](/assets/rollercoaster4.png)

I liked the analogy of the roller coaster above to describe the 4 phases of bug detection from the fresh-eyes phase to deep insight. Another reason I liked the roller coaster analogy is because we can get on a second time but we can never re-emulate that first time, we know what to expect, we aren’t shocked, it loses some of the magic from the second time onwards and are chasing the thrill and adrenaline of that first time. That is what I am trying to emulate in testing — finding a way to get as close to that first ride magic as possible.

How can we try to replicate stage 1 “fresh-eyes” bug detection rate?

Rotate testers across projects to introduce fresh eyes periodically helps cash in on this benefit but there may be some time loss to consider due to increased questions, knowledge transfer and onboarding.
Session-Based Test Management (SBTM): Time-boxed exploratory sessions to promote curiosity. This can be combined with paired exploratory testing and bug hunts / bug bounty initiatives (optionally can be incentivized).
Leverage AI and LLMs to help simulate fresh eyes — ask questions and prompt test scenarios in ways that can help simulate the fresh-eyes scenario.
Apply checklists, automation and structured testing to counter cognitive biases.
Enforce psychological safety so testers feel comfortable raising questions around logic and reporting defects.

Disclaimer: Some image and graphics in this article are generated by AI: Microsoft Co-Pilot for illustrative purposes and not my own artwork.

Find the article on LinkedIn here: https://www.linkedin.com/pulse/bug-detection-roller-coaster-carnival-code-shadows-maire-grant-bbbve
and on Medium here: https://medium.com/@mairegrant/the-bug-detection-roller-coaster-a-carnival-of-code-and-shadows-74a0e47251eb
