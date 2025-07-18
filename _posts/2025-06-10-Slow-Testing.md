---
layout:     post
title:      "Slow Testing"
published:  true
---

# What is fast tech - an analysis of fast fashion vs software development

By now everyone is aware of the repercussions of fast fashion and over consumerism but what learning can we apply from this to software development and is it too going in the same direction? 

## Overproduction and Overconsumption 
We have seen the rise of micro-trends in fashion, with more means than ever before of influencing and advertising to people. These micro-trends mean new products are being pushed out as fast as possible and people are consuming beyond their means. 

Tech companies release new models, a new smartphone, wearables and devices incrementally even if little to nothing has changed knowing that people will buy the new products even if their existing devices still work. 

Hype around product launces such as Apple events create a fan followed culture that supports this unsustainable consumption, having the latest smartphone or device has became about being a trend or status symbol as much as it is for purpose. 

Upon the purchasing a new smartphone, most of its carbon impact is locked in before the device is turned on – it costs around 60 kgCO2e to manufacture, package and ship the product, equivalent to approximately 350 km driven in an average petrol car. [1]

Constantly changing landscape of frameworks, languages and paradigms come with a cost and rework leads to increased time and ewaste. (e.g., from jQuery > Angula > React ... etc). Engineers are prompted to keep up to date and to chase new tools in some cases over mastering fundamental principles and maintaining legacy systems (where feasible). 

Companies often add additional features that are not necessary, sometimes to show that changes are occurring but without considering the impact or need. This adds complexity and makes systems less maintainable as a whole. 

## Disposability 
In fast-fashion clothes are often not built to last and are thrown away after a few years, so too, software products are developed and discarded at a fast pace leaving artefacts behind that consume resources, cause bloat and encouraging speed over sustainability. The result is wasted effort, duplication and throwaway culture. 

"If it breaks we can just rebuild it" - a lack of consequence means that care is not taken. Speed, novelty and short term wins are prioritized over longevity and thoughtful design leading to throwaway systems, more MVPs than necessary that cannot be maintained. 

High-churn software and features can focus on speed over quality craftsmanship. 

## Burnout Culture 
It is no secret that fast fashion can create harsh and undesirable working conditions putting employees and skilled individuals under pressure to deliver faster. The same principle applies to developers and testers being put under pressure to ship faster and keep up with growing demands and unrealistic expectations. 

Automation in the form of machinery for manufacture and AI tools and automation in software devalue skilled individuals. 
As a tester I love to "move fast and break things" in the right context and with purpose but this can bleed into an emphasis on speed over stability. 

## Environmental and Ethical Impact 
Fast fashion has a massive impact on the environment. So too, environments that are always up (even when they don't need to be) have an environmental impact. Software relies on massive energy consumption which under the hood can have questionable data practices and exploitative use of crowd labour (e.g AI labelling and training). 

## Slow Fashion
The opposite of fast fashion is slow fashion where quality, materials, ethics, sustainability, integrity and longevity are prioritised over mass production. 

|Fast Fashion |Slow Fashion  | Slow Tech Equivalent | 
|--|--|--|
|Disposable  |Made to last, reusable, repairable  | Scalable and sustainable codebases that can be scaled up or down | 
|Low Quality Materials | Higher quality materials, intentionally selected, durable, sustainable | Well thought out code and design patterns, efficient algorithms
|Driven by trends | Timeless, designed with longevity in mind  | Maintainable code and architecture |
|Exploitative practices | Fair wages, ethical practices| Transparent development practices and ownership
|High environmental impact | Sustainable manufacture, reduced environmental impact| Open standards, ethical and fair data use, no biased systems
|Frequent releases | Reduced number of products, intentional releases| Lean, efficient resource usage, intentional releases |

## Examples of "Slow" Thinking in a Tech World 
- Open source stewardship, not just needless creation (don't reinvent the wheel) 
- Sustainable UX and design practices, app design that doesn't encourage addiction or endless scrolling - less is more mentality (where applicable). 
- Software that focuses on longevity - Maintain and improve existing systems over rewriting them where possible 
- Green computing - Reduce cloud and ewaste, energy use and reduce carbon emissions. 

## Action - How can I apply the principles of "slow-tech" in my everyday role? 
As a tester how can I implement these practices in my day-to-day to try and make a difference? 

### Quality Over Speed

 - Don't adopt a fast-fashion mindset, don't test just enough to get it 
   out the door, test with purpose and intention. Treat testing as a   
   craft, being thoughtful and keeping long term reliability,   
   performance and scalability in mind.
 - Advocate for comprehensive regression testing, look for edge cases and negative scenarios outside of the happy path. 
 - Push back on unrealistic testing timelines that sacrifice thorough test coverage. 
 - Let others know when you spot tech-debt that may be detrimental to longevity and long term stability.

### Reduce and Reuse

 - Reduce the need for constant rewrites, look out for smart reuse, are
   there libraries, data and artefacts that can be shared among teams
   and team members?
 - Can we share documentation and principles that help us to align?

### Foster a Culture of Craftsmanship and Inclusivity 

 - Quality over quantity. Treat testing as the craft and skill that it
   is. Take care in crafting thoughtful test scripts and test automation
   that requires less maintenance and can be scaled.
 - Shift left, look at pull requests from a testing perspective, are we
   building testable code or are we using testing as a tickbox.
 - Consider accessibility, usability and edge cases early in order to
   reduce rework for unconsidered non-functional requirements.  
 - Write code with future requirements in mind so that less rework is
   needed.

The "Slow Fashion" Tester Mindset

Quality > Speed 

Longevity > Trendiness (maintainable tests, reusable tools)

Ethics > Lack of Transparency (Question shady design practices and data use) 

Sustainability > Burnout (Health workloads and long-term focus) 

Craftmanship > Shortcuts (Take pride in delivering valuable work) 

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