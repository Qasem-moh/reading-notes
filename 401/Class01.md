# How to Solve Programming Problems
_When most programmers are given a programming problem in an interview, they make several key mistakes.  The most severe of those is the improper allocation of time._

_If you have heard the saying “measure twice and cut once,” then you are probably familiar with the idea of spending upfront time to make sure something is done right, rather than diving right in._

_The most common mistake I see when conducting interviews or watching someone try to solve a programming problem is they try to start writing code as soon as possible._

_Another big mistake is trying to over solve the solution on the first iteration.  Keep it simple, don’t try to get fancy._

***
## A simple set of steps

I am going to give you a simple set of steps to follow which you can use for any algorithm type programming problem.

1- Read the problem completely twice.

2- Solve the problem manually with 3 sets of sample data.

3- Optimize the manual steps.

4- Write the manual steps as comments or pseudo-code.

5- Replace the comments or pseudo-code with real code.

6- Optimize the real code.

*As much as 70% of our time should be spent in steps 1-3.*

![6 Ways to Get Better at Problem Solving
](https://www.7pace.com/wp-content/uploads/2021/03/02-Image-2-2048x1260.jpg)

***
## Solve the problem manually

Programming is automation plain and simple.  You may have the ability to skip the manual steps and jump directly to code, but there is a manual process which is the foundation of any code you write.

It is very important to solve the problem manually first, so that you know what you are going to automate, otherwise you are just slinging code around.  Which while can be fun, will make you look like an idiot in a programming interview and will probably cause you to sweat profusely.

I recommend that you solve the problem with at least three different inputs to make sure you really understand your solution and that it will work for more than one case.

I often use a Mathematical Induction approach if possible.  Using this approach I might try and solve for 1 first, then for 2, then for n.

Also don’t forget to look for corner cases and edge cases and do any examples for those kind of cases you can think of.

It’s very important that when you solve a problem manually, you recognize what your brain is actually doing to solve the problem.  You may need to write out all the things you are normally storing in your head.  You want to be aware of each step, it is easy to gloss over them.

Let’s look at a very basic example, reversing a string.

If I give you a string “Zebra”, and ask you to reverse it, most people will do the following manual steps.

* Write “Zebra” down.

* Start a new word, and put “a” as the first letter.  (Why –> because it is the last letter, we want to start here)

* Put “r” down as the 2nd letter.  (Why –> because it is the next letter backwards from the last letter we copied)

* Put “b” down as the 3rd letter.  (Why –> same as above)

* Etc

Notice how I write down each little step and why.

## Optimize the manual solution

People often don’t realize how valuable this step is.  It is much easier to rearrange and reconstruct and idea or algorithm in your head than it is in code.

It’s well worth the effort to try and optimize the actual solution or simplify it when it is still in the most easily malleable state.

What you want to do here is figure out if there is another way you can solve the problem easier, or if there are some steps you can cut our or simplify.

Let’s look at our string reversal example and see if we can simplify the steps.

We should be able to immediately recognize that we can use a loop here to reduce the manual steps.  Our duplicate why’s for most of our steps tell us that we are doing the same thing over and over for each step, just with different data.


    1- Write “Zebra” down.

    2- Start at the last letter in the word and create a new empty word.

    3- Append the current letter to the new word

    4- If there is a previous letter, make the previous letter the current
       letter and start back at 3.

_Look how close we are getting to code at this point.  You should be tempted to actually write the code for this.  That is good, it tells you that you have solved and simplified the problem well.  Writing code should now become very easy._


## Write pseudo-code or comments

_Many times you can skip this step if you have a really good handle on the problem or your previous steps already created a detailed enough description of the solution that coding it is already a 1 to 1 translation_

_If you are a beginner or struggle with these kinds of problems, I would go ahead and take the time to do this step anyway though._

_What we want to do here is capture all the steps we created and now either put them into our editor as comments or write them as psuedo-code that we can translate to real code._

_By doing this, we can know exactly what the structure of the code we are going to write is going to look like which makes the job of filling in the actual code later trivial._

Let’s look at some psudeo-code for reversing a string.

    // NewWord = “”

    // Loop backwards through word to reverse

    //   NewWord += CurrentLetter

    // Return NewWord


## Replace comments with real code
This step should be extremely easy at this point.  If you have done all the other steps, this step involves no problem solving at all.

All we do here is take each comment and convert it into a real line of code.

Taking the string reversal, we might end up with something like this.

    String newWord =""
    for(int index = oldWord.Length – 1; index <= 0; index—)
    newWord += oldWord[index];
    return newWord;

1 for 1 translation of the comments we created above for real code.

If you struggle here, there are usually two possible reasons:

1- You didn’t break down the problem into small enough steps

2- You don’t know your programming language well enough to do the conversion

If you didn’t break the problem down enough, try going back to the second step and being as meticulous as possible.  Write out each and every single step.  I know it is a pain, but do it, believe me it will be worth the effort.

If you don’t know your programming language well enough to do the translation, you may need to brush up here on some basic constructs.  Any language you expect to be able to solve algorithm type problems in, you should know how to do the following things:

* Create a list
* Sort a list or array
* Create a map or dictionary
* Loop through a list, or dictionary
* Parse strings
* Convert from string to int, int to string, etc


**If you don’t know how to do all of these things.  Stop what you are doing now and learn them**. It’s not a very long list, and the benefits will be profound

##Optimize the real code

Sometimes this step isn’t necessary, but it’s worth taking a look at your code and figuring out if you can cut out a few lines or do something simpler.

This is also a good place to make sure all your variables are named with long meaningful names.  I cannot stress enough how important having good names for your variables and methods is for helping the person evaluating your code to understand what you were trying to do.  This is especially important when you make a mistake!

I won’t give an optimization for our trivial example of a string reversal, but a word of advice here is not to get too tricky.  Just try to mainly simplify your code and get rid of duplication.

## A few final tips
If you follow this template for solving algorithm type problem, you should do very well in programming interviews, but the key to doing so is having confidence in this process.

The only way you are going to have confidence in this process is to practice it.  It takes a good amount of faith to believe that spending 70% of your 30 minutes to solve a problem just thinking about the problem and not writing any code is the right approach, so make sure you have that faith when you need it.

I’ve talked about using TopCoder to become a better programmer before, and I still recommend it.  Codility.com is another great site I have recently been introduced to.

There is one important step I did not include in the outline above, because I didn’t want to make the process any more complicated than it needed to be.

Many times you will find that a problem itself involves multiple large steps or is very complicated.  In those instances, you will want to try and find a way to cut the problem directly in half and then following the process above for each half.

This method of tackling a problem is called “divide and conquer” and is quite effective.  A good way to know where to break a problem in half is to think about what part of the problem if already given to you would make solving the rest easy.
***

# Pretend Your Time is Worth $1,000/Hour and You’ll Become 100x More Productive

“Pretend your time is worth $1,000/hr. Would you spend five of them doing extra work for free? Would you waste one on being angry?” -Niklas Göke

You have very few hours here on on this earth.

Still, many people waste much of their time on pointless, low-quality activities that don’t help them reach their true goals — their mission.

The truth is, most people value their time at far, far less than it’s worth.

They say yes to things they have no business doing. They give away their talents, attention, and effort to others who take, take, take.

They spend hours watching low-quality television and social media when they should be productive and effective.

See, many people could be making a fortune (if they used their time well)…but instead, they give away their time in unproductive ways that leave them broke, unhappy, and stuck.

    But what if you placed a high value on your time?

How would that change you? Your life? Your family? Your future?

Imagine that an hour of your time is worth **$1,000**.

What would your life look like?

What people would you stop putting up with?

What problems would you stop wasting time on?

What things would you stop — and start — doing?

Your results would be incredible. You’d become exponentially more productive, focused, and effective.

“Most people have no clue what they are doing with their time but still complain that they don’t have enough.” -Grant Cardone, NYT best-selling author

    “Busyness” Isn’t a Badge of Honor; It’s a Sign of Weakness

“Being busy is a form of mental laziness.” -Tim Ferriss

It takes discipline to not become “busy.”
If you let it, your world and the people around you will take all your time. Your time is not unlike your paycheck; if you don’t budget for things, you’ll have nothing left over by the end of the month.

This is how lives are wasted — by doing thankless work for ungrateful takers that didn’t deserve your time in the first place.

We’re all busy — with work, our families, our friends. It’s not bad to be “busy.” But in the words of best-selling author Jeff Goins:

    “The most successful people I know are not busy. They’re focused.”

Are you focused, making tangible action steps towards what truly matters?

…Or are you just “busy?”

When you’re busy, you are on autopilot. You can’t see the hours slipping away, time you’ll never get back.

Wrote the ancient philosopher Seneca:

    “Indeed the state of all who are preoccupied is wretched, but the most wretched are those who are toiling not even at their own preoccupations…If such people want to know how short their lives are, let them reflect how small a portion is their own.”


***
# How to think like a programmer — lessons in problem solving
![](https://cdn-media-1.freecodecamp.org/images/1*HTRqXgr7CVtRBsyTxurQew.jpeg)

If you’re interested in programming, you may well have seen this quote before:

“Everyone in this country should learn to program a computer, because it teaches you to think.” — Steve Jobs
You probably also wondered what does it mean, exactly, to think like a programmer? And how do you do it??

Essentially, it’s all about a more effective way for problem solving.

In this post, my goal is to teach you that way.

By the end of it, you’ll know exactly what steps to take to be a better problem-solver.

Why is this important?
Problem solving is the meta-skill.

We all have problems. Big and small. How we deal with them is sometimes, well…pretty random.

Unless you have a system, this is probably how you “solve” problems (which is what I did when I started coding):

Try a solution.
If that doesn’t work, try another one.
If that doesn’t work, repeat step 2 until you luck out.
Look, sometimes you luck out. But that is the worst way to solve problems! And it’s a huge, huge waste of time.

The best way involves a) having a framework and b) practicing it.

“Almost all employers prioritize problem-solving skills first.
Problem-solving skills are almost unanimously the most important qualification that employers look for….more than programming languages proficiency, debugging, and system design.
Demonstrating computational thinking or the ability to break down large, complex problems is just as valuable (if not more so) than the baseline technical skills required for a job.” — Hacker Rank (2018 Developer Skills Report)
Have a framework
To find the right framework, I followed the advice in Tim Ferriss’ book on learning, “The 4-Hour Chef”.

It led me to interview two really impressive people: C. Jordan Ball (ranked 1st or 2nd out of 65,000+ users on Coderbyte), and V. Anton Spraul (author of the book “Think Like a Programmer: An Introduction to Creative Problem Solving”).

I asked them the same questions, and guess what? Their answers were pretty similar!

Soon, you too will know them.

Sidenote: this doesn’t mean they did everything the same way. Everyone is different. You’ll be different. But if you start with principles we all agree are good, you’ll get a lot further a lot quicker.

“The biggest mistake I see new programmers make is focusing on learning syntax instead of learning how to solve problems.” — V. Anton Spraul
So, what should you do when you encounter a new problem?

Here are the steps:

1. Understand
Know exactly what is being asked. Most hard problems are hard because you don’t understand them (hence why this is the first step).

How to know when you understand a problem? When you can explain it in plain English.

Do you remember being stuck on a problem, you start explaining it, and you instantly see holes in the logic you didn’t see before?

Most programmers know this feeling.

This is why you should write down your problem, doodle a diagram, or tell someone else about it (or thing… some people use a rubber duck).

“If you can’t explain something in simple terms, you don’t understand it.” — Richard Feynman
2. Plan
Don’t dive right into solving without a plan (and somehow hope you can muddle your way through). Plan your solution!

Nothing can help you if you can’t write down the exact steps.

In programming, this means don’t start hacking straight away. Give your brain time to analyze the problem and process the information.

To get a good plan, answer this question:

“Given input X, what are the steps necessary to return output Y?”

Sidenote: Programmers have a great tool to help them with this… Comments!

3. Divide
Pay attention. This is the most important step of all.

Do not try to solve one big problem. You will cry.

Instead, break it into sub-problems. These sub-problems are much easier to solve.

Then, solve each sub-problem one by one. Begin with the simplest. Simplest means you know the answer (or are closer to that answer).

After that, simplest means this sub-problem being solved doesn’t depend on others being solved.

Once you solved every sub-problem, connect the dots.

Connecting all your “sub-solutions” will give you the solution to the original problem. Congratulations!

This technique is a cornerstone of problem-solving. Remember it (read this step again, if you must).

“If I could teach every beginning programmer one problem-solving skill, it would be the ‘reduce the problem technique.’
For example, suppose you’re a new programmer and you’re asked to write a program that reads ten numbers and figures out which number is the third highest. For a brand-new programmer, that can be a tough assignment, even though it only requires basic programming syntax.
If you’re stuck, you should reduce the problem to something simpler. Instead of the third-highest number, what about finding the highest overall? Still too tough? What about finding the largest of just three numbers? Or the larger of two?
Reduce the problem to the point where you know how to solve it and write the solution. Then expand the problem slightly and rewrite the solution to match, and keep going until you are back where you started.” — V. Anton Spraul
4. Stuck?
By now, you’re probably sitting there thinking “Hey Richard... That’s cool and all, but what if I’m stuck and can’t even solve a sub-problem??”

First off, take a deep breath. Second, that’s fair.

Don’t worry though, friend. This happens to everyone!

The difference is the best programmers/problem-solvers are more curious about bugs/errors than irritated.

In fact, here are three things to try when facing a whammy:

Debug: Go step by step through your solution trying to find where you went wrong. Programmers call this debugging (in fact, this is all a debugger does).
“The art of debugging is figuring out what you really told your program to do rather than what you thought you told it to do.”” — Andrew Singer
Reassess: Take a step back. Look at the problem from another perspective. Is there anything that can be abstracted to a more general approach?
“Sometimes we get so lost in the details of a problem that we overlook general principles that would solve the problem at a more general level. […]
The classic example of this, of course, is the summation of a long list of consecutive integers, 1 + 2 + 3 + … + n, which a very young Gauss quickly recognized was simply n(n+1)/2, thus avoiding the effort of having to do the addition.” — C. Jordan Ball
Sidenote: Another way of reassessing is starting anew. Delete everything and begin again with fresh eyes. I’m serious. You’ll be dumbfounded at how effective this is.

Research: Ahh, good ol’ Google. You read that right. No matter what problem you have, someone has probably solved it. Find that person/ solution. In fact, do this even if you solved the problem! (You can learn a lot from other people’s solutions).
Caveat: Don’t look for a solution to the big problem. Only look for solutions to sub-problems. Why? Because unless you struggle (even a little bit), you won’t learn anything. If you don’t learn anything, you wasted your time.

Practice
Don’t expect to be great after just one week. If you want to be a good problem-solver, solve a lot of problems!

Practice. Practice. Practice. It’ll only be a matter of time before you recognize that “this problem could easily be solved with <insert concept here>.”

How to practice? There are options out the wazoo!

Chess puzzles, math problems, Sudoku, Go, Monopoly, video-games, cryptokitties, bla… bla… bla….

In fact, a common pattern amongst successful people is their habit of practicing “micro problem-solving.” For example, Peter Thiel plays chess, and Elon Musk plays video-games.

“Byron Reeves said ‘If you want to see what business leadership may look like in three to five years, look at what’s happening in online games.’
Fast-forward to today. Elon [Musk], Reid [Hoffman], Mark Zuckerberg and many others say that games have been foundational to their success in building their companies.” — Mary Meeker (2017 internet trends report)
Does this mean you should just play video-games? Not at all.

But what are video-games all about? That’s right, problem-solving!

So, what you should do is find an outlet to practice. Something that allows you to solve many micro-problems (ideally, something you enjoy).

For example, I enjoy coding challenges. Every day, I try to solve at least one challenge (usually on Coderbyte).

Like I said, all problems share similar patterns.

Conclusion
That’s all folks!

Now, you know better what it means to “think like a programmer.”

You also know that problem-solving is an incredible skill to cultivate (the meta-skill).

As if that wasn’t enough, notice how you also know what to do to practice your problem-solving skills!

Phew… Pretty cool right?

Finally, I wish you encounter many problems.

You read that right. At least now you know how to solve them! (also, you’ll learn that with every solution, you improve).

“Just when you think you’ve successfully navigated one obstacle, another emerges. But that’s what keeps life interesting.[…]
Life is a process of breaking through these impediments — a series of fortified lines that we must break through.
Each time, you’ll learn something.
Each time, you’ll develop strength, wisdom, and perspective.
Each time, a little more of the competition falls away. Until all that is left is you: the best version of you.” — Ryan Holiday (The Obstacle is the Way)
Now, go solve some problems!

And best of luck ?