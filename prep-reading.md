# El Reading Notes of the 401 Variety

## Problem Solving
[How To Solve Programming Problems](https://simpleprogrammer.com/solving-problems-breaking-it-down/)

**Common Mistakes**
1. Improper Allocation of Time.
- measure twice, cut once. Don't be so fast to dive right in, do it right the first time, by taking your time.
2. Starting with code ASAP.
- Again, take your time. More important that *solving* the problem is *understanding* the problem. Talk it out, think it over, and take our time. This isn't a race.
3. Over solving the problem.
- The **KISS** method is key here, Keep It Simple Stupid. Whatever that looks like, try not to over-complicate a simple solution.

**Steps For Success**
1. Read the problem completely twice.
2. Solve the problem manually with 3 sets of sample data.
3. Optimize the manual steps.
4. Write the manual steps as comments or pseudo-code.
5. Replace the comments or pseudo-code with real code.
6. Optimize the real code.

The vast majority of your time should be spent on steps 1 - 3.

## Time to Think Like a Programmer
[How To Think Like A Programmer](https://www.freecodecamp.org/news/how-to-think-like-a-programmer-lessons-in-problem-solving-d1d8bf1de7d2/)

First, let's explain what **not** to do:
- Try a solution.
*if that doesn't work*
- Try another solution.
*if that doesn't work*
- Repeat step two until you strike gold!
This is literally the worst possible way to go about this, come on dude, do better.

*“Almost all employers prioritize problem-solving skills first.*
*Problem-solving skills are almost unanimously the most important qualification that employers look*
*for….more than programming languages proficiency, debugging, and system design.*
*Demonstrating computational thinking or the ability to break down large, complex problems is just as valuable (if not more so) than the baseline technical skills required for a job.”* 
— Hacker Rank (2018 Developer Skills Report)

*“The biggest mistake I see new programmers make is focusing on learning syntax instead of learning how to solve problems.”* 
— V. Anton Spraul

**The Moment You've All Been Waiting For - The Steps**
1. **UNDERSTAND**
- Seek to understand *exactly* what is being asked for.
- Questions often appear to be impossible because you don't *understand* them.

This is why you should write down your problem, doodle a diagram, or tell someone else about it.

*“If you can’t explain something in simple terms, you don’t understand it.”* 
— Richard Feynman

2. **PLAN**
- DO NOT, I repeat, *DO NOT* dive right into solving the problem.
- Slow down, think, and plan out the solution.
- Give your brain time to analyze the problem and process the information.
- REVIEW THE COMMENTS!

3. **DIVIDE** This is *the most important* step!
- Rather than try to solve a gigantor problem solo style...break it up into smaller 'sub problems.'
- Beginning with the simplest of the problems, begin chipping away. Go nice and slow (like Usher), one by one.
- Now that all the mini-sub-problems are done, connect the dots.
- All those sub problems are like Lego clipping on to Lego, dot by dot, until the problem is solved!

*“If I could teach every beginning programmer one problem-solving skill, it would be the ‘reduce the problem technique.’*
*For example, suppose you’re a new programmer and you’re asked to write a program that reads ten numbers and figures out which number is the third highest. For a brand-new programmer, that can be a tough assignment, even though it only requires basic programming syntax.*
*If you’re stuck, you should reduce the problem to something simpler. Instead of the third-highest number, what about finding the highest overall? Still too tough? What about finding the largest of just three numbers? Or the larger of two?*
*Reduce the problem to the point where you know how to solve it and write the solution. Then expand the problem slightly and rewrite the solution to match, and keep going until you are back where you started.”* 
— V. Anton Spraul

4. **Crap - Stuck**
- Take a breath, it's gonna be ok. You are not unique.
*Here are some steps to get through a real pain in the you-know-what*
    1. Debug
- Go step by step through your solution trying to find where you went wrong.

*“The art of debugging is figuring out what you really told your program to do rather than what you thought you told it to do.”* 
— Andrew Singer

    2. Reassess
- get away from the computer, no seriously.
- Now that you're back, look at the problem from another perspective. Is there anything that can be abstracted to a more general approach?
- If all else fails...utilize the nuclear option. Delete everything and begin again with fresh eyes. I’m serious. You’ll be dumbfounded at how effective this is.

*“Sometimes we get so lost in the details of a problem that we overlook general principles that would solve the problem at a more general level.*
*The classic example of this, of course, is the summation of a long list of consecutive integers, 1 + 2 + 3 + … + n, which a very young Gauss quickly recognized was simply n(n+1)/2, thus avoiding the effort of having to do the addition.”* 
— C. Jordan Ball

    3. Research
- Google-foo that bad boy. You read that right. No matter what problem you have, someone has probably solved it. Find that person/ solution. In fact, do this even if you solved the problem! (You can learn a lot from other people’s solutions).

**Don’t look for a solution to the big problem. Only look for solutions to sub-problems. Why? Because unless you struggle (even a little bit), you won’t learn anything. If you don’t learn anything, you wasted your time.**

5. **PRACTICE**
- Don’t expect to be great after just one week. If you want to be a good problem-solver, solve a lot of problems!

## The Five Whys
[One, Two, Three, Four, Five Whys](https://www.mindtools.com/pages/article/newTMC_5W.htm)

- The 5 Whys uses "counter-measures," rather than "solutions." A counter-measure is an action or set of actions that seeks to prevent the problem from arising again, while a solution may just seek to deal with the symptom. As such, counter-measures are more robust, and will more likely prevent the problem from recurring.

**1. Assemble a team**
**2. Define the problem**
**3. Ask “why” the problem is occurring**
**4. Ask “why” 4 more times for each answer generated**
**5. Know when to stop**
**6. Address the Root Cause**
**7. Monitor fixes**

## MOVIE TIME!
[Event Loop?! What the heck?!](https://www.youtube.com/watch?v=8aGhZQkoFbQ)
* The event loop's job is to take a gander at the stack as well as the task queue. 
* If the stack is empty the event loop grabs the first thing on the queue and pushes that bad boy onto the stack.
* The callback queue is like a staging area for code that has completed its execution and needs to re-group with its buddies back at the main queue.
* Do not block the callstack or your website will not render, and that's a bad day USA my friend.

[Hey, it's me Mario](https://www.youtube.com/watch?v=9vJRopau0g0)
* Check this stat out -> 2.5x more attempts and higher success rate for study participants who were not penalized for failing to solve a puzzle. Wild right?
* Ah yes, the Super Mario Effect - treating life’s fun little challenges like a game of Super Mario Bros.
* **DO NOT FOCUS ON MISTAKES!** Rather, focus on defeating King Koopa rather than that time you accidentally threw Mario into a lake of lava, hey - it happens to the best of us.
* *“Life gamification”* - framing the programming process as if it were a game, you are FAR more likely to keep trying and gaining enjoyment from learning...if you stop taking yourself so dang seriously - sheeeeeesh.
* When everything is a game, the fear of failure is eliminated and learning happens more naturally, just as Nintendo had intended.
