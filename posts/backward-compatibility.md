<!--
.. title: Breaking changes & Backward compatibility v2
.. slug: backward-compatibility
.. date: 2023-04-04 21:30
.. tags: 
.. category: API
.. link: 
.. description: 
.. type: text
-->

<img src="/images/breaking_changes.jpeg" alt="Breaking changes everywhere">

I learned what backward compatibility means regarding software engineering when I started working on microservices. When you are responsible for services widely used by other teams inside and partners outside, you most likely become paranoid about maintaining backward compatibility of your API as much as possible. Especially when it is a  highly volatile environment with rapidly growing functionality and direction changes on the fly.

At some point,  I invented the term "backward awkwardability" - an awkward feeling while telling consumers that there are breaking changes in a new release, so they have to migrate. If your team does it frequently, they will say something like, "C'mon guys, you introduced breaking changes just a few iterations before! What's going on?"

Let's talk about backward compatibility and how to deal with the breaking changes in terms of API.<!-- TEASER_END -->

# Breaking the broken

Maintaining backward compatibility means newer versions will keep the application's existing functionality intact. A recent version can contain bug fixes, improvements, or new features. But all previous components are working as expected, and no efforts are required to bring them back to work after the update.

Breaking backward compatibility means you obligate your consumers to make efforts so they can retain the functionality they are already using. It is not the same as regression. The latter implies degrading the current customer experience due to newer changes. But that usually happens unintentionally because of a lack of quality assurance and fixed from the developer side.

Breaking changes are intentional, and it requires some work to adapt the changes from the consumer side. They already did some job to start using your service. And now, they need to do this exercise again to keep going, and no guarantee that it will not happen again unless there is a written agreement to prevent such cases.

Migration is often a non-planned job in the short or mid-term. Consumers are paying a double price: for new and current functionality. We assume that the value should compensate for the efforts.

Regarding software development, the efforts are additional work hours to change the source code in compliance with the breaking changes. The cost of such changes may be high: a Business Analyst should assess the impact of changes, a Developer to investigate required changes and implement them, and a Quality assurance engineer to verify them.

Let's review a more general example related to User experience. Any drastic changes in how users interact with the system require additional efforts to learn and adapt to how to use the functionality again. It is not critical when it is about moving a button in a direct-2-consumer app (I wanted to use Instagram as an example, but moving a button there might also be impactful). But considering professional and semi-professional software products, such changes will impact productivity resulting in money loss.

A frustrated end-user can stop using an app and switch to a competitor. It is more complicated for professional service: you can switch from Figma if they decide to revolutionize the design process in an expected way. For enterprise-level vendors, such a switch might be a costly endeavor. A concerned service can be a vital part of business processes, and it is impossible to drop it immediately and jump to a competitor. Anyway, the cost of switching to another service is always higher than the cost of implementing the breaking changes.

# Expect the unexpected

Is it possible to avoid breaking changes? Yes, technically. Keeping compatibility at any cost leads to an increase in technical debt. Your team will have to implement sometimes non-trivial and not the best solutions to honor their commitments. They also will be very limited in using new frameworks and libraries and major updates of the ones in current use. So you pay the price for maintaining backward compatibility instead of your customers.

That strategy may work for conservative industries. The alternative is to regulate the introduction of breaking changes.
The regulations depend on the organization's policies and services specifics. In general, it results in API contract terms aligned with consumers.

The following questions are considered when "signing" the contract:

**1) Frequency and schedule**

The organization defines how frequently you are willing to release incompatible versions: per several releases or some calendar period. You aggregate the breaking changes in your product backlog and fire them in a particular release. So consumers can plan their migration activities accordingly.

The main issue is to follow that schedule, as there might be business reasons to introduce breaking changes earlier than initially expected.

**2) Communication**

It matters how you notify customers about it. The worst option is to send them a link to a Jira ticket with a poor description and a mess in the comments. The best option is to write a comprehensive migration guide. Developers might consider writing such a guide a waste of time, but it is an investment to reduce future support activities.

**3) Migration support**

A comprehensive guide will not save you from additional communications: answering questions, helping with the update, and fixing bugs. So be prepared to have a support buffer in your team's capacity. Or even better, super-obvious advice: always have a support buffer.

**4) Support timeline for previous releases**

Customers may postpone the update to an unknown time due to various reasons. And they may keep requesting improvements and bug fixes for an older version they currently use. That ends up supporting several releases: moving forward with new releases and producing backports to the previous ones.

The backports continuously require more efforts from the team, shifting focus from the future to the past. The more gap you have, the more challenging it is to improve an older version. It is not a trivial task from both a development and testing perspective that can trigger unexpected problems.

To fight this, you must include another point in the contract: how long you commit to supporting previous versions.
In my practice, there was a case when we supported five previous major releases. That was a solid argument to speed up the update. As we had a 2-week release cycle, the customers had about two months to plan and conduct the update.

Frequent updates may not be typical for your industry. That period may vary due to different business contexts. Or you have a good old customer with a fat bank account unwilling to migrate soon. And the senior management will eat you alive if you try to push the unwanted update. That is mainly the organization or program-wide question. You can only support previous releases for a while but can't drop too frequently.

# When the link becomes missing

Maintaining backward compatibility for existing functionality and managing breaking changes is a challenge. And who is responsible for managing that? The answer is rather disappointing -  the entire team in various aspects:

* Business Analyst to conduct impact analysis when considering design options. 
* Product owner to communicate with stakeholders. 
* Tech Lead to manage tech debt and overall delivery. 
* Developers follow the agreements and make all that happen. 
* QAs to ensure we don't break something unintentionally.

To finalize that topic, I would like to emphasize the following statements:

* When discussing a feature design or a bug fix for such a critical service, always ask yourself and the team if that can potentially introduce breaking changes. Become paranoid, just like me.
* Ensure all stakeholders, including the team, know the breaking change policy. If you don't have it already, you don't need it. If you need it, start the discussion in your organization.
* Test Automation is the key to preventing unexpected breaking changes with regression testing.
* When designing a data structure in general and API request/response format, remember that there will be no chance to change those when your service goes live. It is not possible to elaborate on all questions in advance. But that approach leaves no room for "will do it later." Try to consider all possible options, even if they might be unrealistic. The price for reckless design is the highest price we pay in the industry.
* Make sure breaking changes are appropriately communicated to your customers.
* And follow your Contract commitments.

*Take care,*

*Ilya*


Change history:

- 2021-04-26: Initial version published
- 2023-04-04: Second revision published