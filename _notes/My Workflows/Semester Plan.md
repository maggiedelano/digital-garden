---
title: Semester Plan
---

This note is part of the series of notes about [[My Workflows]].

# High Level
At the beginning of every semester (and over the summer), I create a strategic plan. This includes a few different steps:

1. I list out research and personal tasks I hope to accomplish for the given time period.[^1]
2. I convert these high level tasks into milestones with specific dates.[^2] 
3. I add the milestones to a weekly calendar.
4. I work backwards from each milestone and outline what I need to complete each week to reach the milestone on my set due date.
5. As part of my [[Weekly Review]] I review the plan for that week, which is already populated on the strategic plan, to prioritize my time. I add/subtract milestones and update the weekly tasks as needed.

I really like this setup because it's my first experience with backwards planning that has actually been effective. As I've been doing the plans I've gotten much better at predicting how long tasks will take, and working backwards helps me know when I realistically need to start on a task. I also really like having a fully populated strategic plan ready at the beginning of each week. This gives me confidence that I'm making progress toward all the different projects I'm working on without feeling like I'm juggling them all at once. It also helps me to know which weeks will be particularly busy, and whether my plans are realistic or if I'm over-committing myself.


# Current Implementation

My plans are currently implemented in [[Roam Research]]. I create a dedicated page with the three sections shown below. I then populate each section in sequence as described above.

- Goals
	- Research
	- Personal
- Major Due Dates / Milestones
- Week by Week

The one advantage of implementing the plan in Roam is that I can use [block references](https://www.roamtips.com/home/what-is-block-roam-research) to have my milestones appear in both the milestones view and in the week by week view. If a due date changes, the changes appear everywhere. I can also easily see if I've forgotten to schedule any of my milestones.

In the week by week view, I make the individual weeks heading 1 size, and then nest the relevant to dos underneath. I use custom css to add a little calendar icon before daily notes pages in my graph to give things a little color:

```css
/* add a calendar to all dates (pages that end w/ 2021...) */
span[data-link-title$=", 2021"] .rm-page-ref--link:before{
    content: "🗓 ";
}
```


Here are a two screenshots of the setup:

<img src="/garden/assets/milestones.png" height="75%" width="75%"/>

<img src="/garden/assets/weekly.png" height="75%" width="75%"/>

## Potential Improvements
The only downside of this system right now is that I have to manually create the week by week blocks and move the milestones to them. However, since I only need to do this once a semester, I don't think it is worth automating. There is a keyboard shortcut in [Roam Toolkit](https://chrome.google.com/webstore/detail/roam-toolkit/ebckolanhdjilblnkcgcgifaikppnhba?hl=en-US) that allows you to quickly increase the date by a week, so that makes things a lot easier.

# Resources
This plan was based on watching the [Strategic Plan webinar](https://www.facultydiversity.org/webinars/semesterplan18) from the National Center for Faculty Development & Diversity. Highly recommend encouraging your institution to get a subscription for you if possible.

# Notes
[^1]: Although I am at a teaching focused institution and teaching makes up much of my days, I follow the [guidelines](https://www.facultydiversity.org/webinars/semesterplan18) from the National Center for Faculty Development & Diversity that says that research and personal tasks should be the focus of your strategic plan because teaching has more built-in accountability than most research and personal tasks.
[^2]: Some of these dates are more firm than others. For example, if I have a hard paper deadline, that's not likely to change. I try to pick a reasonable deadline for everything else, ideally spreading out over the course of the semester so things don't pile up at the end.