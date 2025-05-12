---
layout:     post
title:      Attributes for Grouping Defects
published:  true
---

In this article I may refer to defects as bugs, problems and issues interchangeably.

### Defect logging — how do we do it?

Every company and application takes it’s own slightly different approach based largely on similar principles. The more data we log against a defect, the deeper insights we can gain about the system under test.

I’ve compiled a list of attributes on which defects can be **grouped** _although this is by no means exhaustive_! Feel free to let me know if there is anything I have left out or anything else you would add . Is it feasible to add all applicable defect attributes to a defect? In the interest of time, _probably not._ Some attributes will be more valuable than others in a particular application in painting a picture of the defect landscape.

I wanted to figure out how long it takes on average to log a defect, I am still unclear on that (additional research pending! If anyone knows some stats around this — help a gal out)!

I’d love to experiment with this in the future — measuring the time it takes to log defects and finding ways to streamline the process. Many companies use **defect logging templates** in house to increase speed, standardize formats, and make defect searching easier.

### Exploratory Testing + Logging: The Overlap

Recording time spent logging a defect could be skewed by an overlap in exploratory testing time. I often explore and log defects at the same time, filling in the details as I go — screenshots, payloads, URLs and anything else applicable. Are these as such, two separate activities? One larger activity? as bug logging for the most part accompanies issue reproduction at the same time?

This post primarily focuses on defect logging — just one pillar of defect management. I have catalogued attributes to group defects, description, steps to reproduce and title have not been included. My goal is to provide a list of ways that defects can be grouped which can lead to identifying patterns.

**Questions I have:**

*   What attributes can be grouped together?
    
*   What groups overlap, and what can pairing these together tell us about the system?
    
*   Can we identify patterns in defects by grouping attributes?
    

**Is there an optimal number of fields to include on a bug report?**

Giving as much information as we can means nothing important may be left out — (unless there is something we have missed) but if not all of that information is used, this is time wasted on filling out those fields which at scale could lead to a massive saving in time and thus money.

If we use a **standardized format** and log as much information as possible, we could leverage **machine learning** to predict patterns and uncover connections between defects that we might otherwise miss. We could see a lot more **Bug Prediction as a Service (BPaaS)** and advanced metrics for defect management in the future — especially given the ROI they offer.

Considering that defects can be used as **system behaviour documentation** and provide a snapshot in time of when something occurred, this means information not used on the first pass and analysis of the defect may be useful on a second pass e.g if revisiting post closure to give context for potentially related issues.

### So, What Can We Group Defects By?

Here’s a list of defect categories that might help:

![AttributesForGroupingDefects](/assets/group_defects.png)

**Functional Defects** These defects occur when the system doesn’t meet predefined requirements. You can group these defects by specific requirements or broadly as “functional” defects.”

**Non-Functional Defects** These relate to non-functional requirements, like security or performance. You can categorize them by individual requirements or group them broadly as “non-functional” defects.

**User Group** Different user groups may experience the software differently. Group defects by which group or role is affected — customers, internal users, testers, developers, etc.

**Department** Categorize defects by the department where they originated. This can overlap with the root cause but focuses on the origin point.

**Defect Life Cycle Stage** Where is the defect in its life cycle? Open? Closed? Rejected?

**Area of the System** Where did the issue occur? Specific pages, modules, or user flows?

**Severity** How much does this issue affect functionality? Major, minor, trivial — defects can be classified based on their severity.

**Time of Discovery** When was the defect logged? By date, time, or business quarter?

**Requirement** As mentioned in functional defects, we can group by a specific requirement or requirement type. Specific requirements could be things like a compliance code that a feature has to comply with, if this requirement is not met — release cannot happen, we can then sort and filter bugs based on this requirement to ensure no bugs in the system remain against this requirement.

**Reproducibility** Is the issue reproducible? How often does it occur? Is it intermittent, or is it a one-off?

**Root Cause** What’s the root cause of the defect? Is it logic error, human error, or something introduced in testing?

**Risk** How risky is this defect to the business and the system?

**Release/Version** Group defects based on which release or version they impact.

**Codebase Area** Where in the code did the defect originate?

**Development Phase** Was the defect found in planning, implementation, or deployment etc?

**Impact Scope** Who and what will be affected? Will it impact a single user or the entire system?

**Frequency/Occurrence** How many times does the defect occur? Is it intermittent, or does it happen consistently, what is the rate at which it occurs?

**Impact on Business** How much will the defect impact the business? Is it a major reputational risk, or will it cause financial losses?

**Environment** In what environment was the defect found? Sometimes, defects arise due to environmental conditions.

**Priority** How quickly does this defect need fixing? Priority can be influenced by its risk and business impact.

Feel free to chip in if you think there is anything I have missed or if you’d add any additional attributes to the list. Let’s keep this conversation going and make defect management more efficient!

[Find me on Medium](https://medium.com/@mairegrant)