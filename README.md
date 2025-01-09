# easy-estimate

## What is this?

Say you have a bunch of tasks in your backlog, and your boss gives you a deadline or asks you to provide an estimation of when you and your team will complete the project.

Easy Estimate — a cliché, yes — is a simple  projection[^1] tool that helps you ~estimate~ discover if what you are trying to accomplish is even possible.

## How to install

1. Click "**Save link as...**" on this file: "[easy-estimate.html](https://github.com/ezp127/easy-estimate/raw/main/easy-estimate.html)".
2. Open it in your favorite browser.

## How to use

### Backlog items

Count *(I meant it, just count; no fancy Fibonacci story points needed)* how many backlog items[^2] you have in total, including finished and unfinished. This number **must be cumulative** and **replicated** in each chart backlog column. 

Say you start the project with 20 stories and plan to accomplish it in 4 sprints[^3]. Your backlog items should look like this:
 
    Backlog: 20, 20, 20, 20
 
Then, in the second sprint, you decide to include one more story, so the backlog input should be `20, 21`. At the end, if you keep these 21 stories, your final result should be: 
 
    Backlog: 20, 21, 21, 21

Feel free to kill two stories in the third sprint if needed.

    Backlog: 20, 21, 19, 19

### Finished items
 
Make a projection. You can do this by accumulating how many items you think you can finish per sprint.

Say you have those 20 backlog stories and plan to complete them in 4 sprints. You could distribute 5 stories per sprint, so your chart can be configured as:

    Finished: 5, 5, 5, 5

Now let's imagine your team finishes the first sprint on time with 5 stories completed as planned; then on the second sprint something happened and they managed to deliver only 3 stories; the third sprint ends with 3 more stories; and finally 2 on the fourth sprint. As a result, we have:
   
    Finished: 5, 3, 3, 2

As we can see, 7 stories remain unfinished, and more sprints are necessary. The conclusion is that the initial estimation made before the project started was just a wild guess, and it failed.

## Okay, where's that estimation you promised?

The estimated projection will be revealed on the chart by the crosses of those two lines: **Backlog projection** and **Finished projection**.
This line cross will indicate, approximately, whether the current pace is sufficient to complete the project on time or call for further intervention.

![image](https://github.com/ezp127/easy-estimate/raw/main/demo.png)

As the example above shows, if you keep finishing stories (green bars) at the current pace, at least one more sprint will be needed to complete the project.

## What's the science behind this tool?

It's just [linear regression](https://en.wikipedia.org/wiki/Linear_regression) represented on a bar chart.

## Trouble shootings

- The input values of **Backlog**, **Finished**, and **Planned** should be a list of comma-separated integer numbers. Don't include a comma at the end.
- The **Labels** (X scale) field should be a comma-separated list of labels. Don't include a comma at the end.
- The **Scale** (Y scale) field should be an integer number.
- You can save your progress and changes just by bookmarking the page in your browser to generate different versions of it. Once you hit the **Update chart** button, all the chart data is updated on the page link.

## Footnotes

[^1]: **#NoEstimates**. I would like to invite you to watch [this nice presentation on YouTube](https://www.youtube.com/watch?v=QVBlnCTu9Ms) given by *Allen Holub* about software development estimations. I guarantee your time won't be wasted.

[^2]: As items, I refer to: epics, stories, tasks—you name it. Only make sure to keep consistency; don't mix different types of items on the same chart.

[^3]: By sprints, I mean it can be anything: scrum sprints, weeks, months, or years. Just rename the chart *X scale* as you wish.
