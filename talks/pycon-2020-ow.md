- [Title](#title)
- [Conference](#conference)
- [Status](#status)
- [Artifacts](#artifacts)
- [Abstract](#abstract)
- [Detailed description](#detailed-description)
- [Notes](#notes)

# Title

<!--- Proposal title -->

Decoding bias and narrative in competitive video games broadcasts with video analysis

[⬆️ Back to top](#title)

# Conference

<!--- Conference name and year + links -->

[PyCon 2020](https://us.pycon.org/2020/)

CFP Link: https://us.pycon.org/2020/speaking/

[⬆️ Back to top](#title)

# Status

<!--- 🎉 Accepted, 🚮 Rejected, 🚪 Withdrawn -->

🎉 Accepted

PyCon pivoted to a virtual conference, so it was uploaded as a pre-recorded YT talk.

[⬆️ Back to top](#title)

# Artifacts

<!--- Links to recording, speaker page, slides etc. But also reason for rejection, if any. -->

[Talk description on PyCon's website](https://us.pycon.org/2020/schedule/presentation/107/)

[YouTube video](https://www.youtube.com/watch?v=0HzbyQPKW9E)

[Slides](https://speakerdeck.com/kimadeline/pycon-us-2020-decoding-bias-and-narrative-in-competitive-video-games-broadcasts-with-video-analysis)

[GitHub repo](https://github.com/kimadeline/overwatch-ocr)

[⬆️ Back to top](#title)

# Abstract

**Length limit:** N/A

With video game competitions (also known as eSports) being broadcast on online streams and regular TV stations, in-game video producers have to balance between making the game accessible to casual viewers, and packing enough action on screen to keep regular players interested.

What they choose to show on screen also define the narratives surrounding the competing teams, building hype around them and setting implicit expectations (for example what character class is shown the most).

In this talk we will walk through video analysis of professional Overwatch games to extract data, explore and validate a few hypotheses on what eSports broadcasters think viewers want to see.

[⬆️ Back to top](#title)

# Detailed description

## Why this talk

<!-- Optional, depends on the proposal -->

N/A

[⬆️ Back to top](#title)

## Audience

<!-- Optional, depends on the proposal -->

This talk will show that you don't need advanced knowledge of Python or machine learning to cobble a few tools together to perform simple video analysis. As such, the audience is only expected to have basic Python knowledge.

This talk would be best suited for people with an interest in eSports, video analysis, detecting bias, or simply a story on using Python to answer questions.

At the end of it, the audience should have learned about a variety of tools for video processing, optical character recognition and data plotting. Hypothesis-driven development will also be covered, and how people can apply it to verify or invalidate assumptions. Last but not least, it will hopefully spark some critical thinking about the content we ingest, helping us reflect on what content producers want us to see, and which opinions they want us to have.

[⬆️ Back to top](#title)

## Talk outline

<!-- Include time breakdown if any -->

### Intro 👋 (2 min)

About me
Outline

### Why this talk 🎮 (7 min)

Motivations (1 min)

- I am an Overwatch player and a beginner Pythonista

Basics of eSports and Overwatch (4 min)

- Why eSports?: TV broadcasting, endorsement deals, partnerships with traditional sports
- What is Overwatch?
- Anatomy a professional game of Overwatch

Detecting bias: Who gets the most screen time? (2 min)

- Home or away team?
- Winning/favourite team or losing/underdog one?
- Which character class: tank, damage or support?

### Tools of the trade 🛠 (10 min)

How are we going to fact-check these hypotheses? (1 min)

- By analyzing an area of the screen to check if we're in first-person point of view
- Focus on Overwatch World Cup games: USA vs South Korea and USA vs China

The process (7 min)

- Overview
- Video splicing step using `ffmpeg`
- Optical character recognition with Azure Cognitive Services
- Picking `TinyDB` as a database and sticking with it
- Plotting the data with `plotly`

What I could have done better (2 min)

- Video splicing
- Azure API call optimization
- Database choice
- Prettier plots

### Findings 📈 (5 min)

Hypotheses validated or invalidated (3 min)

- Home or away team
- Winning/favourite or losing/underdog team
- Which character class

Data I didn't consider (3 min)

- Other elements on the screen
- What about camera angles that are not first-person POV
- Audio track
- Sample size

### Wrap-up and call to action 🎬 (3 min)

- Video analysis doesn't have to be scary, you can use it for almost anything, and then submit a talk proposal about the process
- If you're an Overwatch player: you could even expand the analysis to other elements of a recording of your game to extract more data (everybody loves data) and review your play
- Hypothesis-driven development is useful for making data-informed decision (everybody still loves data)

[⬆️ Back to top](#title)

# Notes

<!---
Optionally, anything that doesn't fit in other sections:
Any additional equipment you might need, whether or not you’ve given this talk before, etc.
-->

**Talk type:** Regular talk

**Talk duration:** 30 minutes

This is my first time submitting a talk proposal to PyCon US, and, if accepted, would be my first time attending it as well. I have given presentations to small groups, but this would also be my first experience speaking in front of a large audience.

As a an avid Overwatch player and a newly minted Python developer (~6 months of Python experience), I wanted to share this side project combining my passion of gaming with my journey in learning Python, hence why this talk should be accessible to all audience levels.

I don't plan to do live coding nor will I need to play sound, so I don't have any specific needs.

🐙🐈 The code is located [on GitHub](https://github.com/kimadeline/overwatch-ocr).

[⬆️ Back to top](#title)
