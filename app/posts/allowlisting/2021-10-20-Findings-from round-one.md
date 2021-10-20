---
title: Findings from round 1 testing
description: Our findings from the first round of research in HMP Lindholme, and ideas for round 2. 
date: 2021-10-20
---

Our User Researcher spoke to 8 participants from HMP Lindholme over two days. They had a range of access needs and digital skills.

*A table highlighting the access needs and digital skills of the participants.*

The findings gave us a lot to think about!

## Main takeaways 
### The type of allowlisted site heavily influenced user reactions

All of our users expressed concerns over data protection. Many were disconcerted about Survey Monkey and the prospect of entering their personal information on an external site. This could be due to a general distrust our users consistently show about how their information may be used while they’re in custody.

Even though Survey Monkey was just a concept, it is clear that we must choose a different allowlisted site for future testing. One contender is Virtual Campus, an education platform for people in prison.

### Is it really safe?

In the context of our scenarios, the “safe site” tag was generally interpreted as being connected to the data protection and security of the site. However, we did ask users about their sentiments on these words through the lens of a questionnaire, so we think this has skewed results. The strangeness of Survey Monkey seems to have heavily influenced user behaviour and attitudes towards their interpretation of what we mean by “safe”. 

There was a distinctly negative reaction to asking users to fill out a questionnaire due to a lack of trust in the way their data would be used within the prison. 

We’re going to try “allowed site” next.

### How valuable is a call to action button?

Most of our users clicked on the whole tile, but two specifically chose to click on the Open call to action button. 

For standardisation with our other card components elsewhere, we may test removing this call to action button text and icon altogether.

*Iterated tile idea for round 2.*

### Interstitial page

The interstitial page tested really well. None of our users displayed any confusion about leaving the Hub. 

One particularly tech-savvy user was vocal about not needing to see the interstitial page again for each new allowlisted site. Most other users vocalised their preference to just see it once.

### Users expect to be told some links may be blocked upfront

The strongest reactions from users were caused by displaying a blocked error message without setting expectations that this would happen beforehand. This happened in scenario 2, when we asked users to click an external link to bbc.co.uk whilst on Survey Monkey.

This led to feelings of frustration, even when it was clear it had been blocked due to the limitations of the prison environment. 

One participant said: *“It’s like **dangling a carrot..** it's blocked... So that's like them saying to me, I can go home tomorrow, but I'm not allowed.“*

Another said: *“**Why bother putting it on page in the first place If you are going to block me?** Why bother putting the link on and saying, have a look here. And then it just **psses me off** then when I can’t go.”*

To combat this, we’ve added new content to forewarn users that not all links on the allowed site will work.

*Iterated interstitial page idea for round 2.*

### Challenging the breadcrumb component

We added the [breadcrumbs component from the Design System](https://design-system.service.gov.uk/components/breadcrumbs/) into our designs to test if it would help users to understand and navigate between the different category levels on the Hub. 

To find the learning questionnaire:
- 2 users used the full breadcrumbs component to navigate
- 4 partially used it at various stages
- 1 user with visual impairment struggled to see the breadcrumbs component altogether 
- 1 user used the back button on the browser to navigate, ignoring the breadcrumbs component 

Overall, the breadcrumbs component was used, but inconsistently.

The participant who ignored the breadcrumbs component completely later said that it was not clear that it could be clicked on. They said: *“Normally that line **would be a different colour**”* in reference to the underline. Further on in the test they then came across a different link that was blue and said: *“You see how that’s in blue? **Now you know you can click on that**.”* He referred back to his comment about the breadcrumbs and said: *“If the other ones were like that **you’d know you can click on it**. Normally when it’s black writing it’s stuck, you can’t do anything with it.”*

We took this finding and shared it with the wider gov design community on GitHub. We started a discussion to ask for any research or design documentation around the decision to style the breadcrumbs component using the near-black **govuk-text-colour** as opposed to the blue link typography style, also known as **govuk-link-colour** in the design system.

In the meantime, we plan to change the style of the component for the next round of testing. We will test the blue link style to see if this makes the breadcrumbs component appear more clickable compared to our previous design, and we will share any findings back into the Design System.

*Before and after: updated design for the breadcrumbs component to test in round 2.*
