---
title: Research and round 1 testing
description: Our research questions, designs and testing for the first round of research in HMP Lindholme. 
date: 2021-09-16
---

## Research questions 

We sought to answer the following questions:

1. How confident are users navigating to an allowlisted site and then returning to the Hub?
2. How do users feel about interacting with an allowlisted site? 
3. When a user is on an allowed site, what happens when they then click a link which takes them to another external site (one that is not on our allowed list)?
4. Are the Hub and allowlisted sites understood by our users? Where does one end and the other begin?

To answer these questions, our user researcher came up with 3 scenarios for testing:

**Scenario 1:** Find the Level 3 music course
**Scenario 2:** Find and fill out a questionnaire on learning and employment on an allowlisted site (in this case, Survey Monkey)
**Scenario 3:** Navigate back to the Hub homepage from the allowlisted site 

## Designing for testing ##
### Homepage simplification ###
We simplified the current design of our homepage to make the journeys easier for participants. We changed some links in our Popular topics navigation menu to reflect what our users had identified with most in a previous card sort session.

We also changed **Popular topics** to **Quick links**. Currently, the links in our **Popular topics** navigation menu are hardcoded into the front-end by our developers. They do not automatically update based on popularity, so they are not always an accurate reflection of what is actually the most popular content. 

*Before and after: simplifying the homepage for testing.*

We designed fake category landing pages for **Learning and skills**, **Courses**, and **Music** to aid our tasks.

The main concept we wanted to explore was how to tell users they’d be leaving the Hub to access an external website. 

We wanted to reassure users that they were:
- leaving the Content Hub
- entering an authorised safe site
- not in trouble for accessing this site

## Constraints

### No control over errors ###
Although we created initial designs, we quickly discovered that we were not able to control the error message users were shown if they tried to access any links on the allowlisted site that were linking to other external (non-allowlisted) sites. 

This was controlled by the browser, and dictated by network security restrictions, so was not something we could change.

### New branding, new navigation ### 
We were also not able to control the branding, content, logos or navigation on the allowlisted website. 
New content tile design
We wanted to be able to demarcate between content that lives on the Hub and allowlisted content so there were no surprises if a user was suddenly taken to an external site.
We decided to try a new content “tile” (or card component) for allowlisted sites, building on our existing tiles. 

*Development of ideas for the new design of the content tile.*

### Creating a new tag ### 
How could we visually show which content wasn’t ours? We had a lightbulb moment to reappropriate the existing “SERIES” tag we already have on the Hub but with some tweaks: 

1. We changed the background of the tag from purple to green.
2. We introduced a new tick icon to reinforce that “it’s safe”.
3. We changed the content to “**SAFE SITE**”. 


*Before and after: adapting the design of our existing tag component.*

### Call to action buttons ### 

In other parts of the Content Hub (such as Your profile) we’ve used the NHS card with an image component. We would love uniformity but we were limited by the design of our other legacy content tiles elsewhere on the Hub. These have call to action (CTA) buttons at the bottom of each tile which signal to the user the type of content they’re about to see, with button text that says either “Watch”, “Read” or “Listen”. 

These can, however, be confusing. In some instances, we’ve found CTA button text mistakenly says “Read” when the next page is a page full of videos. 

We decided to try a more universal instructional text of Open as this was not specific to any content type. 

### Testing data input ### 
Much of our content is static. So we wanted to test an interactive website to see how our users managed to input data. We set up a simple, fake questionnaire about learning and education in prison on Survey Monkey. 
Using brand logos

The image we chose to use on the card was the Survey Monkey logo. The idea behind using the external site logo in the image was to create continuity for users between our site and the new allowlisted site. 

We wanted our users to know (especially if they weren’t familiar with the new site) that they had clicked on the right thing.

### Adding a new subtitle to our card component ### 
On the new tile, we used the name of the page as the main title, followed by a lighter, smaller subheading. Subheadings on the tile are a new idea.

This new subheading tells users that the content will open on a new website. We included the main part of the URL (in this case “SurveyMonkey.com”), to telegraph to users that they’re leaving the Hub. 

### Creating a new external link icon ### 
We came up with lots of ways to convey to users (both in text and with icons) that they were going to an external site that would also open in a new tab. We also found an old blog about the decision to remove the external link icon from GOV.UK. 


### Icons from GOV.UK ### 

GOV.UK argue that you don’t always need to tell people links are external, unless for example, the user is in the middle of a task. That is probably true for people in the community who can, for the most part, access the internet without limits. However, we were not sure if this was true of people in prison.

Allowlisting is a new concept on the Hub. We thought our users (especially those already using the Content Hub) would expect some restrictions on what they can and cannot access. We thought it might be useful to signal to users that certain content may be on an external site, so there were no surprises when they see an unfamiliar site for the first time. 

We also know that due to the lower literacy levels of people in prison, some of our users struggle with lots of words. So, we decided to trial a new ‘opens an external site’ icon to reinforce this.

*The tile design that we tested during the first round of research.*
 
### New interstitial page ### 
When clicking on an allowlisted site for the first time, we wanted to be able to “interrupt” users to reassure them that a new site was going to load but that it was safe to visit. 

We considered a modal or “pop up”, but we know these components tend to be unloved at best and really annoying at worst.


### Idea to show “interrupter” warning content on a pop-up. ### 

Although the pop-up idea would allow us to retain our own navigation and headers, we worried that if a user continued onto the allowlisted site they would not understand where the original Content Hub tab had gone. 

So we decided to try a bespoke interstitial page. When a user clicked the content tile, a new tab would open with this new holding page in it. After clicking **Continue**, the allowlisted site would load in that same new tab. 

We decided against a forced redirect. After a certain amount of time showing the interrupter content, we could automatically load the new external website. This would save users from having to take an additional step of clicking Continue. But, we worried that a time limit would be arbitrary and potentially even punishing to our users who might need longer to read and digest the information on this page.

**Our final design included:**

- the Content Hub logo for reassurance
- an H1 telling users: “You’re leaving the Hub” 
- content to tell the user which external site they were now going to, with the main part of the URL shown
- content to reassure users “This is a **safe** website you are allowed to visit.”
- a continue button, to actively get user consent
- a checkbox to capture preferences about seeing this interstitial page again


## The interstitial page that we tested for round 1 ## 

### Importance of showing users URLs  
We later discovered that not all of our users can see a browser bar for security reasons. Only some residents in certain prisons can. This made us question whether our users should have access to it in the future. In the interim, we don’t think there’s any value in us showing users any URLs if they cannot see a browser bar on their laptops.

### To boldly go...  
GDS recommends that bold is used sparingly. However, we felt the message of safety was important, as we know from previous user research that some of our users are concerned about getting into trouble inadvertently whilst using the Hub. So we decided to make the words “safe website” bold for emphasis and to give added reassurance.
Don’t show me this again!

Serendipitously, when linking to Survey Monkey (an external link) in our Figma prototype, we stumbled across a great example of an interstitial page. This gave us the idea for the “Don’t show this message again” content.


*The example of an interstitial page from figma.com*


We couldn’t decide whether to show this message for each new allowlisted site (meaning users might see it several times, when the number of allowlisted sites grows) or if we wanted them to be able to opt out of seeing it ever again.  

As these designs were more to test the concept of allowlisting, and less about achieving the finished design from day 1, we decided to keep it simple initially and gather as much feedback as possible.


---
You can learn more about the purpose of a design history on the [DfE Digital blog](https://dfedigital.blog.gov.uk/2020/09/01/design-history/).
