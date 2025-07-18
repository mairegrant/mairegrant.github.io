---
layout:     post
title:      "Slow Testing"
published:  true
---

# What is fast tech - what can we learn from fast fashion in tech? 

By now we are all aware of the repercussions of fast fashion and over consumerism but what learnings can we apply from this to software development and is it too going in the same direction? 

## Overproduction and Overconsumption 
We have seen the rise of micro-trends in fashion, with more means than ever before of influencing and advertising to people. These micro-trends mean new products are being pushed out as fast as possible and that people are consuming beyond their means. 

Tech companies often release new models of devices incrementally even if little to nothing has changed knowing that people will buy these new products even if their existing devices still work. 

Mass hype around product launces such as regular Apple events create a fan followed culture that supports an unsustainable consumption, making having the latest smartphone or device a trend or status symbol as much as it is for purpose. 

Upon the purchasing a new smartphone, most of its carbon impact is locked in before the device is turned on – it costs around 60 kgCO2e to manufacture, package and ship the product, equivalent to approximately 350 km driven in an average petrol car. [1]

A consistently changing landscape of frameworks, languages and methodologies come with a cost associated and rework leads to increased time and electronic waste. (e.g., going from jQuery to Angula to React ... and so on). Engineers are prompted to keep up to date and to chase new tools in some cases over mastering the fundamental underlying principles and over maintaining legacy systems (where feasible). 

Many companies often add additional features that are not necessary, at times to to show that changes are occurring but without consideration for the impact or actual user need in turn increasing complexity and decreasing maintainability.

## Disposability 
In fast-fashion clothes are not built to last, unsustainable techniques are used and the byproduc is that they are thrown away after a few years (or less), so too, software products are developed and discarded at an ever increasing speed leaving artefacts behind that consume resource, bloat our systems and encourage a mindset of speed over sustainability. This results in duplication and a promotion of throwaway culture.

A lack of percieved consequence means that care is not taken. Speed, novelty and short term wins are valued over longevity, sustainability and ly crafted designs. Throwaway systems become the norm, more MVPs than necessary are produced that cannot be maintained. 

Software begins to focus on speed over quality craftsmanship. 

## Burnout  
It is no secret that fast fashion can create harsh and undesirable working conditions putting employees and skilled individuals under pressure to deliver faster. The same principle applies to software teams in high pressure environments being pressured to deliver faster and keep up with growing demands and unrealistic expectations. 

Automation in the form of machinery for manufacture and AI tools and automation in software devalue skilled individuals. As a tester I love to "move fast and break things" in the right context and with purpose but this can bleed into an emphasis on speed over stability that we are becoming familiar with. 

## Environmental and Ethical Impact 
Fast fashion has a massive impact on the environment. So too, environments that are always up (even when they don't need to be) have a negative environmental impact. Software relies on massive energy consumption overheads which under the hood can lead to questionable practices (think data and crowd labour).

## Slow Fashion
The opposite of fast fashion is slow fashion where high quality, thoughful materials, ethics, sustainability, integrity and stability and long-term impact are prioritised en-masse production. 

|Fast Fashion |Slow Fashion  | Slow Tech Equivalent | 
|--|--|--|
|Disposablity  |Made to last, reusable, repairable  | Scalable and sustainable codebases that can be scaled up or down | 
|Low Quality Materials | Higher quality materials, intentionally selected for durability and sustainability | Well thought out code and design patterns, efficient algorithms
|Trend-driven | Timeless, designed with longer term in mind  | Maintainable code and architecture principes |
|Exploitative practices | Fair wages, ethical manufacturing practices| Transparent development practices |
|High environmental impact | Sustainable manufacturing techniques, reduce environmental impact| Imposed standards (data, laws), ethical, no biased systems
|Frequent releases | Reduce the number of products produced, intentional releases| Intentional releases, maximise delivery, coordinate features |

## Examples of "Slow" Thinking in a Tech World 
- Don't reinvent the wheel, use open source when you can
- Sustainable design practices, less is more mentality (where applicable), systems that don't promote overconsumption of media and information, digital clutter. 
- Longevity focused softwares - Maintain and improve the existing systems over rewriting if it is possible 
- Green computing practices - Reduce ewaste, energy use and in turn reduce carbon emissions. 

## Action - How can I apply the principles of "slow-tech" in my everyday role? 
As a tester how can I implement these practices in my day-to-day to try and make a difference? 

### Quality Over Speed
- Don't just do enough to get it out the door, test with purpose and intention. Treat testing as a craft and keep slow fashion principles in mind, e.g for performance, scalability. 
- Promote regular exploratory and regression testing, search for negative scenarios and edge cases. 
- Challenge unrealistic timelines for testing that impact ability to test thoroughly and with full coverage. 
- Flag potential tech debt early on or anything that may be detrimental to the system making it unreliable. 

### Reduce and Reuse
- Reuse libraries, paradigms, test data and artefacts among team members and teams to reduce maintainability and time to create. 
 - Can we share documentation and principles that help us to align?

### Champion Craftsmanship and Inclusivity 

 - Quality over quantity. Treat testing as the craft and skill that it
   is. Take care in crafting thoughtful test scripts and test automation
   that requires less maintenance and can be scaled.
 - Shift left, look at pull requests, unit tests, UI/UX designs from a testing perspective, are we building testable code and systems or are we using testing as a tickbox.
 - Consider accessibility, usability and edge cases early in order to
   reduce rework for unconsidered non-functional requirements.  
 - Write code with future requirements in mind so that less rework is
   needed.

The "Slow Fashion" Tester Mindset

Quality > Speed 

Longevity > Trends (maintainable tests, reusable tools)

Ethics > Lack of Transparency (Question shady design practices and data use) 

Sustainability > Burnout (Balance, positivity and healty workloads for long-term efficiency) 

Craftmanship > Shortcuts (Take pride in delivering valuable skilled work) 

### References and Further Reading
[1] https://www.carbontrust.com/news-and-insights/insights/smart-phones-smart-choices-harnessing-purchasing-power-to-reduce-the-carbon-impact-of-our-phones

***Avoiding the Rewrite Trap - Camille Fournier -*** 
https://skamille.medium.com/avoiding-the-rewrite-trap-b1283b8dd39e

***The True Cost of Rewrites - Doug Bradbury***
https://8thlight.com/insights/the-true-cost-of-rewrites

***A Slow Fashion Lifestyle***
https://stplwear.com/blogs/journal/6-principles-of-a-slow-fashion-lifestyle?srsltid=AfmBOore597GuEcKiBnvvgKKhMCxoC9Tze-qvNmGhx8GogCwnCotYtL1


***The Principles of Sustainable Software Engineering***
https://learn.microsoft.com/en-us/training/modules/sustainable-software-engineering-overview/