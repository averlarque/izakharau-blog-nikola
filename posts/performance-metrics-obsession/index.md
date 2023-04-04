<!--
.. title: How I overcame my obsession with performance metrics and became a real PO
.. slug: performance-metrics-obsession
.. date: 2022-07-31 11:48:26 UTC+02:00
.. tags: 
.. category: Product Ownership
.. link: 
.. description: 
.. type: text
-->

<img src="/images/Meditation-Man-Working.jpg" width="90%" alt="Overcoming the obsession" style="vertical-align:middle;margin:1% 1%"><br>

I fell into a common trap of every manager: obsession with performance metrics. Since I have been promoted to the PO role my responsibilities include tracking stats related to the backlog and team performance. That includes the team’s capacity, estimates, velocity, and other specific metrics. In an ideal world, the estimation of planned features matches capacity, the team performs a predicted velocity and (more importantly) delivers features in time. But we all know that doesn’t work this way.

This is the story of how I became obsessed with numbers instead of being obsessed with a product. And how I overcame that and shifted my focus to real value.

<!-- TEASER_END -->

## Why did I fall into the “number obsession” trap?

Here are the main reasons, from my perspective:

**Ambitions**

As a newbie Product Owner, I wanted to do my job perfectly: produce an ideal roadmap with epics and user stories that contain clear requirements so that the team could provide precise estimations (in story points). Then that would be translated into a plan fitting the team’s capacity. The team would commit to the plan and complete it with flying colors within a predicted timeframe. Customers are happy, stakeholders are happy, my manager is happy, and the team is also happy. I would receive a gold medal for “the best PO of the year” with a promotion to the Chief Product Officer position. Or Vice President of something, why not?

But the reality is harsh. The requirements are not always defined well, technical complexity is underestimated, the team lacks experience in some domains, dependencies on other teams, and urgent customer support requests. I named only a few obstacles - pretty sure you know the others.

So the original plan is not valid anymore, epics and features shift to “somewhen when it is ready - maybe this year, maybe not”. You found yourself in the hell of constant re-planning (you can read about it in [one of my previos essays](https://izakharau.me/posts/product-manager-year-one/)). You re-plan, the plan fails to meet reality, you replan again and now it looks good. Oh, f*ck, two developers left the team… Here we go again.

When you spend most of your time on re-planning, you can’t be focused on the product.

**Pressure**

Of course, there are reports that track those performance metrics across all the teams. Nothing bad here, this is a must-have if you want to stay on track.

“Why did your team close so few story points in a previous sprint?” I have been asked more and more frequently.

I had a default answer. “We dragged some user stories to the next sprint due to <blah-blah>.” 

That follows with something like, “Take a look at this graph. You can see that you are behind the program increment plan. You should have completed this <number> of story points. But you only completed <much less> so please do something. Let me know if you need my help”.

That “do something” implied the re-planning. “Sure, I will take a look and handle this”.

Now I understand: no one tried to assault me with those questions. Just to highlight an issue and make sure that it is on my radar. But that, multiplied by my ambitions and immaturity as a PO, built up enormous pressure inside me.

I fiercely wanted those damn graphs to look good. I tried to use different approaches in feature decomposition and planning, introduced changes to the refinement process, and scheduled additional meetings to discuss any technical issues before the development. But still, non-completed tasks dragged from sprint to sprint and overlapped with new tasks. None of the original plans seemed feasible or even somehow controllable.

With all that, my old good friend, the imposter syndrome came into play. “What if I am not a real PO? What if __**they realize**__ that I am not a real PO? I should have better stayed as a Business Analyst and never move to a product organization.”

## The Overcoming
Friday, the last day of a Sprint. About 10 PM. I am on the call with a Team Lead (TL) discussing the sprint closure. We really struggled a few previous iterations having a very low team velocity vs our quarter roadmap plans. Several big technical features were continuously dragged from sprint to sprint with multiple issues appearing along the way. 

But this sprint is different. We have managed to close those big features, handle a few customer requests, and fix a bunch of bugs. I did some calculations and that appeared to be our best sprint for the last 7 (!) months. The team is encouraged as it seems we have overcome that dark period.

But this is not what we are talking about with TL. We are discussing 2 medium-sized features that have been developed but not yet tested. They were delivered to a testing environment late today, so our QA already ended her working day. If we could close those features right now, the sprint result will be outstanding. The team really worked hard and deserved that.

“What will we do with the features?” TL asked. I am a Product Owner and I have the power to decide whether a feature is completed or needs additional work to be done.

“Listen, those features are quite small improvements of non-critical functionality. They passed dev testing phase and I personally checked them. All works as expected. Right?” I don’t want to lose the outstanding number I already calculated in my mind. And I am determined to make that happen.

“What do you suggest? Close the tickets without real testing?”

“Yes, you are right. As I said, that is not a critical functionality. I don’t see any risks there. Let’s set them as non-QA, close, and go rest. We did a really great job so we all deserved that”, I can sound very convincing.

“OK, I agree”.

After some manipulations, the features were considered as done, the tickets were resolved and the Sprint was closed. Time to enjoy the weekend.

Saturday morning I received a message from our QA Lead (QL). “Hi, I saw you had closed those 2 tickets as non-QA”.

I am ready to defend, “Yes. Developers finished them very late so you were already off. They are quite small so I decided to complete them as non-QA”.

“OK. I just wondering, do we need to cover them with automated tests?”

F*ck. We’d better cover them with autotests. But that means the QA team needs to write testing scenarios, validate them, and then proceed with automation. Basically, to do the work I previously defined as “not needed” by converting the features to non-QA.

I take a pause. There is a growing feeling that I have done something very stupid. I manipulated with features and moved testing activities in “a shadow mode” to the next Sprint and proudly announced that they are completed. But they are not. I start feeling sick.

“Yes, we need to automate both features”, it took me about 30 minutes to answer her.

“OK, no problem. Next week I will pass it to the QA team and we will proceed with the automation. Have a nice weekend!”

That weekend was not nice for me at all. I passed through the Five stages – denial, anger, bargaining, depression, and acceptance. I fought with my ego which was obsessed with the numbers and wanted to achieve high results, even fictional, at any cost.

Next Monday we had a team retrospective call. I apologized to the entire team. I confessed that I manipulated tickets for the only reason to satisfy my ego with good stats. I spoiled a really great team achievement and now QAs had to cover my ass with that testing.

“What I did is stupid. I am really sorry. I will never do that again”.

And I am keeping my promise. Now, by the end of each Sprint, I consider only what is really done. I am no longer pushing tickets for good stats. I don’t really know how many story points my team closed last sprint or earlier. I am smiling when some managers report something like “We completed 1000 story points during a last sprint/quarter/year”. I am no longer playing that game.

I am focused on the value we, as the Team, can produce for our customers. We can do a complex functionality during a few iterations and that will not look good on reports. But when we deliver that might have a big positive impact on those who use our services. Value can be transitioned to customer satisfaction and that can be transitioned to profits. Story points do not transition to value.

*Take care,*

*Ilya*

<small><a href="https://www.vecteezy.com/free-vector/meditation">Meditation Vectors by Vecteezy</a></small>