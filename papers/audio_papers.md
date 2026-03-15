---
layout: default
title: Effect Sizes Workshop
---

<div class="output" markdown="1">
# Audio guide to the worksheet

This worksheet was uploaded to notebooklm to get an audio guide to the work.  It has been checked by the author to ensure accuracy.

<audio controls>
  <source src="/hsc-7056x/assets/audio/papers.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

</div>

### Transcript

**Speaker 1:** You know, usually when we talk about a medical diagnosis, there's this uh this underlying expectation of precision, right? Like it almost feels like engineering or something.

**Speaker 2:** Exactly. Like you fall off a bike, you break your arm, the X-ray shows that jagged white line, and the doctor just points at the screen and says, "Well, there it is." That's the problem.

**Speaker 1:** Yeah. It's very binary. It's either broken or it's not broken. It's clean. And honestly, that's really comforting.

**Speaker 2:** We naturally like things to be visible. But then, you know, you step into the world of medical research, You start looking at clinical trials or you're trying to figure out if a new treatment actually works and suddenly that X-ray machine is just totally broken.

**Speaker 1:** Completely broken. We're looking at a diagnostic landscape that's just filled with data tables and Greek letters and numbers that are well murky is really putting it lightly.

**Speaker 2:** I mean it is the absolute definition of **diagnostic muddy waters**. The gap between like an exciting medical headline and the actual data in the paper is often massive, right? And it's guarded by this huge wall of statistical jargon, which is exactly why we are here today for this deep dive. Our mission is to hand you, the listener, the ultimate statistical decoder ring.

**Speaker 1:** Yeah, we're going to clear up those muddy waters. We've got a fantastic guide today. It's a mathematics and statistic skills worksheet on reading inferial statistics, complete with the solutions key.

**Speaker 2:** We want to take you from someone whose eyes just kind of glaze over at the side of a data table to someone who can spot exactly what makes a study meaningful.

**Speaker 1:** We're going to decode **P values** and **confidence intervals** using real examples right out of the worksheet.

**Speaker 2:** And we have a really fun hook for you, too. By the end of this deep dive, you'll not only know how to evaluate a new medical treatment, but you'll also finally know the statistical truth, but a massive pop culture myth.

**Speaker 1:** Oh, yes. The allimportant question of whether wearing a red shirt on Star Trek actually mathematically dooms you.

**Speaker 2:** It's vital stuff. But, uh, before we get to the furthest reaches of the galaxy, we really have to start with the **architecture of a study**. Right? Because before you can even begin to read the results, you have to understand how the researchers actually set up the game board.

**Speaker 1:** Okay? So, let's unpack that. Setting up the game board, the worksheet introduces two very different medical trials to show this.

**Speaker 2:** The first one is a trial for a new treatment for uh loose feet.

**Speaker 1:** Yeah, loose feet. They use this thing called the **foot loose index** or FLI, which is basically just a scoring system for foot performance. Higher values mean your foot is doing better.

**Speaker 2:** Makes sense. So, how do they test it?

**Speaker 1:** Well, in this trial, a group of people is recruited. Their foot score is recorded before the treatment starts and then it's recorded again for those exact same people after 3 months.

**Speaker 2:** Okay, keep that specific design in mind. They are tracking the same 35 individuals over time. Now, contrast that with the second trial, right? The second trial is testing treatments for excessive snoring. They use a good sleep index. Again, higher is better, but the setup is totally different. They're testing two distinct drugs against a placebo. So they take their participant pool and just chop them into three completely separate groups.

**Speaker 1:** Ah okay.

**Speaker 2:** Yeah. Group one gets the placebo, group two gets drug A, and group three gets drug B.

**Speaker 1:** And right there, just in those two setups, you have the fundamental divide in study architecture, the **within groups versus between groups** thing.

**Speaker 2:** Exactly. The loose feet study measures the exact same 35 people twice. Once before, once after. So in stats, that's a **within groups analysis** because you're acting as your own control group, right? The researchers are looking for changes within your specific biology over time. But the snoring study fractures the pool into three distinct lanes.

**Speaker 1:** You're comparing the sleep quality of the placebo group against entirely different people in the drug groups.

**Speaker 2:** Yes. And that is a **between groups analysis**. When you sit down to read a study, that's the very first thing you need to identify.

**Speaker 1:** That makes total sense. If I'm comparing myself to myself, that's one thing. If I'm comparing myself some stranger. There are like a million other variables at play, which actually brings me to a detail about that snoring study. The worksheet explicitly mentions that the trial was **double blinded**.

**Speaker 2:** Always a good sign.

**Speaker 1:** Sure. But I want to push back on this a little bit. Like I get blinding the patient so they don't know if they got the sugar pill. But if we're just recording sleep data, maybe monitoring their breathing with a machine, why does it matter if the researcher knows?

**Speaker 2:** You're saying, isn't data just data?

**Speaker 1:** Yeah. Like a snore is a snore. or the machine picks it up. Either way,

**Speaker 2:** it's a totally logical question, but uh it assumes humans operate like robots. **Double blinding** means neither the participant nor the analyzing researcher knows who got what, and that is crucial to prevent bias.

**Speaker 1:** Even with a machine monitoring things, how does a researcher skew a breathing monitor?

**Speaker 2:** It's about subconscious behavioral cues. Imagine a researcher who has spent 5 years of their life developing drug A. They desperately want it to work. You know, obviously If they know a patient is taking drug A, their tone of voice might be just slightly more encouraging during a check-in. Their body language might be more relaxed and that actually affects the patient's sleep.

**Speaker 1:** Absolutely. That subtle encouragement can lower a patient's stress levels, which in turn literally improves their sleep. Or, you know, when interpreting borderline data from the monitor, the researcher might subconsciously round up for the drug and round down for the placebo.

**Speaker 2:** Oh, wow. I never thought about that. You really have to protect the experiment. from human nature.

**Speaker 1:** You do. Double blinding locks that subconscious bias out of the room.

**Speaker 2:** Okay, that makes sense. And speaking of protecting the experiment, there's another detail I noticed in the loose feed trial. The sample size, the **N**.

**Speaker 1:** Ah, yes, the almighty N.

**Speaker 2:** It said the sample size before the treatment was 35 and the sample size after 3 months was also 35, meaning zero participants dropped out, which is a key indicator of a clean trial because think about what happens if a trial starts with 100 people, but after 3 months only 40 are left.

**Speaker 1:** Right. Your first thought is where did the other 60 people go?

**Speaker 2:** Exactly. Was the treatment too painful? Did it have terrible side effects? If only the people with the highest pain tolerance still win, your final data is completely skewed.

**Speaker 1:** You're just measuring a super stubborn subgroup.

**Speaker 2:** Precisely. So an N of 35 starting and ending at 35 is a great health check.

**Speaker 1:** Okay, so the game board is set. We know the architecture. Now, how do we actually read the results? like how do we know if a twopoint improvement is a real win or just random luck.

**Speaker 2:** That is where we get to the concept of a **confidence interval**. This is the range of possibilities, right? Because we never get one single perfect magical number for all of humanity. Let's use an analogy for this to make it concrete.

**Speaker 1:** Go for it.

**Speaker 2:** I want you to think of a **95% confidence interval** like throwing a fishing net to catch a very specific invisible fish.

**Speaker 1:** Okay, I like where this is going.

**Speaker 2:** That invisible fish is the true average improvement for the whole population. We can't see everyone, so we throw our net, which is our sample of 35 people.

**Speaker 1:** Right. And 95% of the time you throw this kind of net, the true answer is trapped somewhere inside it.

**Speaker 2:** Exactly. So, let's look at where the net landed for the LES V trial. The mean difference, the average improvement is 1.91.

**Speaker 1:** Okay. Positive 1.91.

**Speaker 2:** But the worksheet gives us the 95% confidence interval. The net stretches from a lower end of 734 up to a high end of 3.09.

**Speaker 1:** And the critical thing there is the position. of the net. The lower edge and the upper edge are both positive numbers. Right? The entire net landed above zero.

**Speaker 2:** Since they're both positive, we can be highly confident that the true effect is a positive increase in foot performance. Even if the true average is at the absolute lowest edge, 0.734, it's still doing something beneficial. But okay, let's contrast that clean catch with the snoring study. This is where it gets messy.

**Speaker 1:** Let's hear the numbers.

**Speaker 2:** The worksheet gives the 95% confidence intervals for the adjusted means. For the placebo, the net is 43.7 to 50. 1.7.

**Speaker 1:** Okay. So, it reaches up to 51.7.

**Speaker 2:** Yeah. But for drug A, the net is 47.0 to 55.2 and drug B is 47.0 to 55.7.

**Speaker 1:** So, wait, the placebo net reaches up to 51.7 and the drug nets drop all the way down to 47 point.

**Speaker 2:** Exactly. The intervals for the drugs and the placebo are totally overlapping. So, what does this actually mean? Does it mean the drug might be doing absolutely nothing?

**Speaker 1:** Yes, that is exactly what it means. Because the placebo interval overlaps With the drug intervals, the true result for taking the drug might be the exact same as taking a sugar pill.

**Speaker 2:** Wow. So, they're swimming in the exact same water.

**Speaker 1:** They are. This is your first major red flag when reading a paper. If those nets are tangled up, the drug might not be doing anything special at all.

**Speaker 2:** Okay. So, confidence intervals give us the range, the net. But there's another number we need to talk about, the **p value**.

**Speaker 1:** Ah, the p value. The ultimate judge.

**Speaker 2:** If the confidence interval is a net, I like to think of the p value as is a **surprise meter**.

**Speaker 1:** A surprise meter. Okay, break that down for me.

**Speaker 2:** Well, researchers start with the assumption that a drug does absolutely nothing. The **null hypothesis**. The p value basically measures how surprising our trial results are, assuming that the drug is useless.

**Speaker 1:** Right. So if the p value is really low, the results are super surprising.

**Speaker 2:** Exactly. And the traditional cutoff for statistical significance is 0.05. If your p value is less than 05, it means the results are so incredibly surprising that our consumption must be wrong.

**Speaker 1:** The drug must be doing something. The surprise meter is going off,

**Speaker 2:** right? So, let's apply the data. In the loose feed trial, the t test gives a p value of 0.002.002. What's fascinating here is that 02 is far below. 05.

**Speaker 1:** It's basically zero.

**Speaker 2:** Exactly. We reject the idea that the treatment does nothing. There is clear statistical evidence the FLI treatment works.

**Speaker 1:** Okay. But now, let's look at the snoring trial. The worksheet notes they used an **analysis of CO variance** adjusting for age and sex by the way

**Speaker 2:** which makes sense to rule out demographic differences

**Speaker 1:** right and it gives an fstistic of 1.020 and a p value of.366

**Speaker 2:** okay let's analyze this 366 is much much higher than 05

**Speaker 1:** the surprise meter isn't going off at all it's totally silent

**Speaker 2:** dead silent there's not enough evidence to say the snoring drugs work the data just doesn't support it

**Speaker 1:** it's so empowering to just look at a table check the nets in the surprise meter and instantly know the real story

**Speaker 2:** it really is To prove that you, our listener, have truly mastered these tools, we're going to apply them to that fun realworld observational study from the worksheet, the **Star Trek test**.

**Speaker 1:** Yes. This is where math meets pop culture.

**Speaker 2:** Set the scene for us.

**Speaker 1:** Okay. So, a medical researcher watches the original Star Trek series to test a very famous myth. Does wearing a red shirt cause premature death?

**Speaker 2:** A very serious scientific inquiry,

**Speaker 1:** obviously. So, here are the stats from the worksheet. 24 out of 2 39 red shirts died. That's 10.0%.

**Speaker 2:** Okay.

**Speaker 1:** And 16 out of 191 non- red shirts died. That's 8.4%.

**Speaker 2:** All right. I see where this is going.

**Speaker 1:** Here's where it gets really interesting, right? 10% is obviously higher than 8.4%. So, the myth is true, right? Red shirts are cursed.

**Speaker 2:** See, this is where I have to step in as the voice of reason utilizing a **cheese square test of association**.

**Speaker 1:** Oh boy, here comes the math.

**Speaker 2:** If we connect this to the bigger picture, just because one percentage is slightly higher in a specific sample doesn't mean it's statistic. ically significant.

**Speaker 1:** Okay. So, what did the surprise meter say?

**Speaker 2:** The result of the chi square test is a value of 0.349 with a p value of.555.

**Speaker 1:** Wait, 0.555.

**Speaker 2:** Yes. And remember the cutoff 05. A p value of 0.555 is way way above the cutoff.

**Speaker 1:** So, the surprise meter is flatlined

**Speaker 2:** completely. Therefore, statistically speaking, there is zero evidence that wearing a red shirt is associated with premature termination. It's just random variation.

**Speaker 1:** Wow. The versus a total myth. Just random space noise. That's amazing.

**Speaker 2:** It really shows why you can't just look at two percentages and jump to a conclusion.

**Speaker 1:** Absolutely. So, let's quickly recap the big aha moments for you today. You now know to check the architecture is a study within groups or between groups,

**Speaker 2:** right? And you know to check the nets, look for overlapping confidence intervals,

**Speaker 1:** and finally, always check that p value. Make sure it's below 05 before you believe the hype of a new treatment or, you know, a sci-fi curse.

**Speaker 2:** Honestly, huge praise to you the listener for diving into the math with us. The next time you see a flashy headline about a miracle drug, you won't be intimidated by the data tables, you know exactly where to look to judge if the results are actually meaningful.

**Speaker 1:** You are officially armed and dangerous with statistical literacy.

**Speaker 2:** But you know, I do want to leave you with a final puzzle to ponder.

**Speaker 1:** Ooh, okay. Lay it on us.

**Speaker 2:** This raises an important question. Imagine a study has a massive sample size, right? Tens of thousands of people. And because of that, that it gets a highly significant p value of 0.01.

**Speaker 1:** Okay, so the math says it absolutely works. The surprise meter is ringing

**Speaker 2:** exactly. But then you look at the confidence interval and it shows the actual improvement is only like 1% better than doing absolutely nothing.

**Speaker 1:** Oh wow.

**Speaker 2:** The math unequivocally says it works. But is that tiny difference actually meaningful for your life? When does **statistical significance** stop being the same thing as **clinical significance**?

**Speaker 1:** That is a brilliant question. Just because the math finds a tiny fish doesn't mean it's big enough to feed anyone. We will leave you to mold that one over. Thank you so much for joining us on this deep dive. We'll catch you next time.
