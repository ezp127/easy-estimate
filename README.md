# easy-estimate

### What is this?

Say you have a bunch of tasks on your backlog, and your manager gives you a deadline or asks you to provide an estimation of when you and your team will complete the project.

Easy Estimate—a cliché, yes ^_^—is a simple  estimation[^1] tool that helps you discover if what you are trying to accomplish is even possible.

You can use this tool to make projections of anything you classify as a pile of things that need to be done.

### How to install

1. Click "**Save link as...**" on this file: "[easy-estimate.html](https://github.com/ezp127/easy-estimate/raw/main/easy-estimate.html)".
2. Open it in your favorite browser.

### How to use

#### Backlog items

Count *(I meant it, just count; no fancy Fibonacci story points needed)* how many backlog items[^2] you have in total, including finished and unfinished. This number must be cumulative and replicated in each chart backlog column. 

Say you start the project with 20 stories and plan to accomplish it in 4 sprints[^3]. Your backlog items should look like this:
 
    backlog items: 20, 20, 20, 20
 
Then, in the second sprint, you decide to include one more story, so the backlog input should be `20, 21`. At the end, if you keep these 21 stories, your final result should be: 
 
    Backlog items: 20, 21, 21, 21

Feel free to kill two stories in the third sprint if needed.

    Backlog items: 20, 21, 19, 19

#### Finished items
 
Make a projection. You can do this by accumulating how many items you think you can finish per sprint.
Say you have those 20 backlog stories and plan to complete them in 4 sprints. You could distribute 5 stories per sprint, so your chart can be configured as:

    Finished items: 5, 10, 15, 20

Now say your team finishes the first sprint on time with 5 stories completed as planned, then on the second sprint something happened and they managed to deliver only 3 stories, so we have `5, 8` (remember, it's cumulative). The third sprint ends with 3 more stories, and finally 2 on the fourth sprint. As a result, we have:
   
    Finished items: 5, 8, 11, 13

As we can see, 7 stories remain unfinished, and more sprints are necessary. The conclusion is that the initial estimation made before the project started was just a wild guess, and it failed.

### Okay, where's that estimation you promised?

The estimated projection will be revealed on the chart by the crosses of those two lines: **Backlog projection** and **Finished projection**.
This line cross will indicate, approximately, whether the current pace is sufficient to complete the project on time or call for further intervention.

![image](https://github.com/ezp127/easy-estimate/raw/main/demo.png)

### What's the science behind this tool?

It's just [linear regression](https://en.wikipedia.org/wiki/Linear_regression) represented on a bar chart.

### Trouble shootings

- The input values of **Backlog items** and **Finished items** should be comma-separated. Don't include a comma at the end.
- The **X scale** should be comma-separated. Don't include a comma at the end.
- The **Y scale** should be an integer number.
- You can save your progress and changes just by bookmarking the page in your browser to generate different versions of it. Once you hit the **Update chart** button, all the chart data is updated on the page link.

### Footnotes

[^1]: **#NoEstimates**. I would like to invite you to watch [this nice presentation on YouTube](https://www.youtube.com/watch?v=QVBlnCTu9Ms) given by *Allen Holub* about software development estimations. I guarantee your time won't be wasted.

[^2]: As items, I refer to: epics, stories, tasks—you name it. Only make sure to keep consistency; don't mix different types of items on the same chart.

[^3]: By sprints, I mean it can be anything: scrum sprints, weeks, months, or years. Just rename the chart *X scale* as you wish.


#### Q&A for developers:

**Q**: "*Dude, your code is the ugliest I've ever seen; why don't you use the latest {put favorite front-end framework here} along with an enterprise database; back-end framework; Kubernetes; and spend 36 months developing this app???!!!*".
 
**A**: Didn't you hear the latest trend? Vanilla single-file application is the new hype. Don't miss out!

**Q**: Is this a solid and production-ready application?

**A**: No. I would call this a *draft/prototype/side-project/with-no-aspiration-to-become-the-next-unicorn-startup* that you can just download and try on your own computer.
