# Auto Layout Book Log
Paul Solt

My Progress Log on writing the [Auto Layout Book](http://bit.ly/AutoLayoutBook)

## Goal

* Restructure the outline
* 1,500 words
* I can do … 800 words in 12 minutes … what can I do in 90 minutes?
* Just get words down, thoughts down, refine it later

## October 8 2018 08:01:00

* Day 21: Monday
	* 1760 words (2nd pomodoro)
		* Added more details, reworked some of the example by expelling it again
		* Tested out adding the constraints to make sure I'm giving the right advice.
	* 991 words (1st pomodoro) 
		* Went to bed at 11am, got up at 640am (more sleep!)
		* Feeling like I have more energy, I need to get to bed on time.
	* 

## October 7 2018 08:58:42

* Day 20: Sunday
	* 1191 words

## October 6 2018 15:43:21

* Day 19: Saturday 
	* 1066 words
		* A bit tired after a long 8 mile run at a faster pace than normal (9:30 pace) … normally I do 10:30 or 12:00 for the 8+ mile runs
	* Getting into breaking apart an Auto Layout error message
		* Thinking about how a tool like [WTFAutoLayout](https://github.com/johnpatrickmorgan/wtfautolayout) might work in conjunction with a UIStoryboard file … to pull in names of UI elements, which might help visualize what's right/wrong
		* [Sparse](https://github.com/johnpatrickmorgan/Sparse) is a simple parser-combinator library written in Swift.


## October 5 2018 07:30:05

* Day 18: Friday
	* 1099 words
		* Wrote about editing constraints, and a  new trick I learned using the ALT key for views on top of each other
		* Took some extra time to figure out where I left off … since there's some sections I wanted to revise, and tangents that made it hard to just pickup
		* Moving some sections down to work on the next time.

## October 4 2018 07:06:43

* Day 17: Thursday
	* 1314 words 
		* Great start this morning, trying to finish up the UI, and I dig into more gems
		* There's a lot of teaching moments in this UI, which I think it's going to make a lot more sense to readers
		* Learning why some things snap, and then how to resolve them is really important
		* Learning about the decisions you need to make is also important
	* 1591 words (combined)
		* Making edits, and researching how to properly add these constraints … turns out if you want it to match the size you just add all constraints, and after you add all 4 dimensions (if the layout is defined for the interface, it'll snap to fit)
		* Now if you don't want that behavior, you can hold ALT while holding shift (after a diagonal drag) and you can add all the constraints using the current layout positions!
			* NEAT … otherwise I was going to file a bug, because it's annoying that sometimes views will take on the actual value versus the canvas value
				* There's two thoughts here … one, you're trying to make a non-matching UI go where you want it to go
				* Two, you're trying to constrain a layout in place, and to do that you want to use the current canvas values.
				* For the most part when you add a single constraint, it wion't try to update your constraints, but when you add multiple it decides to behave differently
	* More research (3rd + 4th pomodoro's into XML parsing Storyboards)
		* FUTURE: Rename all the identifier programmatically to help diagnose layout problems
	* Debugging Auto Layout constraints … setting breakpoint doesn't give you enough steps, needs a better guide
## October 3 2018 07:16:03

* Day 16: Wednesday
	* 849 words
	* Investigated some of the behaviors of the constraints when you add and remove them (at the same time versus individually for a label)
	* Need to investigate intrinsic content size and custom views … I don't believe you can have the same behavior as the UISwitch, but I could be wrong.
	* Need to talk more about the negative and the positive values of constraints. By default the storyboard will add constraints in such as way that they always default to a positive value (by flipping the relationship)
		* Need a tutorial + image on how this works, and how to visualize the constraints … because the system fails to work well when you have a UITextField on top of a UIImageView (for styling purposes).
		* And then it becomes confusing to the user … their first occurrence of a negative constraint. 

## October 2 2018 12:27:39


* Day 15: Tuesday (Steph's Birthday)
	* 1066 words (first pomodoro)
	* Late start today because I got side tracked with writing an email on iOS jobs
	* Practiced typing today, I need to formalize what deliberate practice I'm going to work on … and how to measure … I'd like to apply it to Auto Layout, but I also feel like I need to research more deliberate practice techniques
	* Wrote about 200 words, editing some of yesterday's flow to introduce running the iPhone simulator sooner, and then checking … and then Preview.
* One thing I notice from typing practice is that it's more fluid and easier to type without as many errors … feels more natural. I should keep practicing, but I should move practice to a low energy time of day, rather than the morning. 
* Xcode 10.1 doesn't fix the issue that I thought it mentioned with the Control Drag, I don't see any difference in behavior from Xcode 10 … and it doesn't feel different.
	* The Diagonal drag is still the preference when you're designing user interfaces.

## October 1 2018 12:51:02


* Day 14: Monday
	* 2285 words in 2nd pomodoro (combined)
	* 1115 words in 1st Pomodoro (adding vertical constraints)
	* I've been writing daily for 2 weeks!
		* Crazy!
	* Feels good to make progress … over 15,000 words written for the first draft
	* Goal: 2-3 pomodoros … let's go!
	* Transcribing notes from the video still … this will probably make up most of the bookΩ
* Theres' only so much that you can type …



## September 30 2018 07:36:03


* Day 13: Sunday
	* At Steph's mom's house … hiding in the laundry room writing.
	* 901 words
		* Mentally distracted, hard to focus … not enough sleep

## September 29 2018 08:45:31

* Day 12: Saturday
* 1160 words 
	* I still haven't described how to add the constraints … everything has been supplemental to the constraint process
	* We've done the coloring, now we need to talk about tconstraining
	* Some research into "Reset to Suggested Constraints" not being screen aware (iPhone X is broken constraints)
		* Easy way to mess everything up!
	* Found more bugs in Xcode … growing list
	* Got a little distracted this morning, but we need to spend another session writing
	* A bit tired today, late night after frisbee … late coffee/kombucha (black tea)

## September 28 2018 10:26:56

* Day 11
* 3456 words (4 pomodoro's)
	* Finally dedicated 2 hours to write, instead of my "15 minutes" or "30 minute" sessions … when I have time I can write!
	* Good content, lots of ideas for workbook supplementals and video supplements
	* Brought in a reference to dropping support for rotation (new blog post idea) based on ATP #292 with Marco dropping support for iPhone rotation in [Overcast 4.1](https://marco.org/2018/03/13/overcast41)
* More words written, this chapter is getting long … just to explain how to add the top, bottom, leading, and trailing constraints 

## September 28 2018 07:45:42

* Day 11
* 1700 words after 2 pomodoros … this is going to be long
* Added more words … figured out my days were wrong. Not sure how that happened … but it didn't match my calendar.
* Trying to restructure how I teach this content … based on video, but also based on how to simply show some of the features.
	* Percentage based sizing as a challenge
* Show Canvas > Show Layout Rectangles / Show Bounds later … it's not as clear as changing the color of a view


## September 28 2018 07:08:33

* Day 11
* I need to spend more time writing … so I'm blocking off more of my day to focus on layout changes.

## September 27 2018 08:11:07


* Day 10
* Writing for 25 minutes at 7:50am
* 1147 words
* I'm watching my video that I recorded, and using it for inspiration on the topics that need to be discussed.
* I need to finish watching the video to figure out how to explain the step by step, and caveats for differences in Xcode 10 from Xcode 9 … since it's very different.

## September 26 2018 22:27:09


* Day 9
* 861 words
* Recorded a 49 minute video on adding constraints that I need to transcribe and make it the chapter notes.
* Today was off because I met with other iOS developers and didn't get a chance to finish my writing in the morning, like I have been enjoying.

## September 25 2018 08:05:46

* Day 8 
* 1303 words
* Installed Mojave yesterday
	* Playing with the dark theme
	* Super Easy Timer needs to be udpated to use the new dark theme APIs, so I can automatically switch the UI theme (3 themes included)
* I need to design my own theme for Multimarkdown + Xcode
	* I never seem to like the dark themes that other people make … so we'll have to investigate what colors will look good (especially for Multimarkdown)
* I need to record myself using the new Xcode 10 as I add constraints, and then turn that into a chapter
* Xcode 10.1 looks like it's going to make my "diagonal drag" unnecessary 

## September 24 2018 08:19:51

* Day 7
* 1558 words
* Setup a new private Github to track changes to the book manuscript
* Writing first thing in the morning (7:50am - 8:20am)
* Way easier to write on a fresh mind, and way more ideas
* Workbook ideas using "furniture arranging" to learn Layout
	* Instagram layout to adapt the design to the bigger screens
	* Or a simple button resizing example 
	* Cut out and layout the designs on the workbook iPhone 8 screen and the iPhone Xs and iPhone Xs Max screens.

## September 23 2018 19:37:14

* Day 6
* 888 words
* I'm exhausted today after being in the sun all morning and early afternoon playing ultimate frisbee
* I set the timer, wrote the first set of words, and then started a second and kept going.
	* It felt good to start making some more progress, even if the writing quality is low right now, it's more important that I start to think through the different concepts, so that I can start to piece together the information that a beginner is going to need to know


## September 22 2018 21:24:12

* Day 5
* 1249 words
	* Got into talking about my experiences demo'ing bomb dodge, and howimpratnt it is to do usability testing to catch issues before you invest tons of time into features
* I'm again tired, trying to write at the end of the day because of all the activities
	* Today I ran my fastest 5K race at 21:37 … close to a 7'00" pace … but I haven't looked at any of my stats yet
	* We went to the market, and some food fests around Rochester
* I don't really feel like writing, and I just want to get more sleep.
* Tomorrow I'm getting up early, to write, so I'll definitely start to dig more into things … and I'm probably going to move writing to my 1st hour, like I wanted to, but haven't been able to do because of a contract deadline.
	* That'll make it easier to sit and write, and not have to waste time … not writing the book.
* Also, I'm super behind on finishing the chapters … so these chapters may or may not be short… we'll see.

## September 21 2018 22:41:11

* Day 4
* 787 words
* Tired, have a 5K race tomorrow … setting a timer for 5 minutes and then going to bed
	* Did another 5 minutes … got to 620 … why not type a bit more … =)
	* Going for a 22:00 5K time … 7'00" pace is my target
* Spent all day on contract work … and just got back from a late night Ultimate Frisbee game
* Had some fun programming a simple App Store keyword tool using NSLinguistics and text … very fun ideas for some projects


## September 20 2018 22:01:52

* Day 3
* 798 words - not great writing, but it's a start, and it's getting me to put in time and focus
	* I need to start writing earlier on the day … the contract work is interrupting my flow, and it's harder than I thought it would be.
* Spent all day on contract work … behind where I need to be, figuring out how to call Swift code from Objective-C 
	* Trying to fix buggy logic



## September 19 2018 21:57:50

* Day 2
* 869 words 
* Inspired after watching "Dawn Wall" with Tommy Caldwell who scales the Yosemite "impossible" face called Dawn Wall.
	* 6 years working on a goal
		* Spring + Fall spent figuring out the traversals to make one unified climb
* Refactored the outline, it didn't feel right, but now I think I'm on the right track with the topics
* Updated sections, reordered to make more logical
	* Trying to make it as easy as possible to get something working
	* Then we'll explain more complexities … don't talk about what we don't need to talk about yet.

### New Section 1 Chapters

1. Auto Layout 101
2. Test Drive Auto Layout (Get in and do something)
3. Auto Layout Fundamentals
4. Layout  (You need more practice with layout before you constrain)
5. Thinking with Auto Layout (Paper prototyping? prep for design?)

## September 19 2018 17:24:33

* Started writing some ideas … busy day working on contract work and UI testing … still feels like docs aren't fleshed out … I have yet to find the updated Apple docs



## September 18 2018 21:58:07

* Day 1
* Wrote 804 words for Chapter 1
	* Starting point, but I'm starting to think that my daily word count is going to be closer to 2,000 words.
	* I didn't really get into the topic, and my outline doesn't quite flow
	* I'm going to cleanup Chapter 1 outline once more, and then hit the ground running
* Part of the process for writing … and doing this challenge is to push myself to think, eat, and breathe Auto Layout, so that I can write easier
* The more I consume the material, and refine my thoughts, the easier it will be to write this book
* Reading Essentialism has been amazing, habit's are what are going to make this book write itself, I just need to make sure I write daily … 
* I'm going to hang up a calendar that I can cross off each day I hit my word count … it's ok if I only write 50 words, as long as I continue the habit, it will continue to build, and my subconscious will be writing the book in my sleep
* I don't want this book to start off dry, I want to showcase real examples of Auto Layout in action, and then I want to break it down with a real world example
* I'm not here to talk about how constraints work, but how you can leverage constraints to make the UI you want


## September 18 2018 12:50 - 1:30

* Mind map for Chapter 1 (15 minutes)
* Talk through topic (7 minutes)
* Update outline

## September 18 2018 10:00 - 12:00

* Setup the [Auto Layout Book landing page](http://bit.ly/AutoLayoutBook).
* Announced the landing page to my email list, Facebook, and Twitter
* Setup a GoViral page to encourage social shares of the book before launch

