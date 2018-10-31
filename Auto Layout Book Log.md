# Auto Layout Book Log
Paul Solt

My Progress Log on writing the [Auto Layout Book](http://bit.ly/AutoLayoutBook)

## Goal

* Restructure the outline
* 1,500 words
* I can do … 800 words in 12 minutes … what can I do in 90 minutes?
* Just get words down, thoughts down, refine it later

## October 31 2018 07:35:43

* Day 44: Wednesday
	* 3,593 words today, slow start, but I took off when I started a new section of the book. 
		* I'll need to go back and refactor a bit, but it's getting the core concepts down, and the headings which will help me organize later.
		* 1121 words (1st pomodoro at 11:00:48)
		* 1700 words (2nd pomodoro at 11:53:23)
		* 1951 words (3rd pomodoro at 12:00:00)
			* Researched preview bugs
		* 3,452 words (4th pomodoro at 13:15:49)
	* Bugs encountered
		* XCODE BUG: Multiple Preview Devices Slows Down Storyboard constraints dramatically
		* XCODE BUG: Cannot zoom into/out of a Storyboard file for Mac apps
		* XCODE BUG: Changing fonts on Accessiblity Inspector in iPhone Simulator Messages causes it to fail to render correctly when toggling between… it squashes messages.
		* 
	* Side tracked today 7am-10am … even after setting up my desk, coffee, and breakfast … Mac update sent me down the rabbit hole (again!)
		* I need to **disable WIFI/internet** when I write in the morning, it's too distracting when an update automatically starts.
		* I was a bit side tracked when Xcode automatically updated … and wanted to see the changes
			*  … that took me to the App Store, and then I read some bad/good reviews … so I decicded to write my Xcode 10 review
			* That lead to me posting a new blog post on Xcode 10 being the gold standard …
			* I probalby need to do a 10-20 things I love about Xcode 10 post with Gifs + Videos
	* Back is doing much better, I can sit for way longer, and move more!
	* Research
		* Safe Areas
			* View Controllers
			* Device bounds
			* Changing values in your own interfaces
		* Margins
			* Margins are the original boundary areas that came before Safe Areas
		* Guides
			* QUESTION: ARe these Guides entirely visual, or are they related to margins?
			* 

## October 30 2018 12:02:26

* Day 43: Tuesday
* 890 words today
* Spent a lot of time writing some new scripts to help track word count and edits
   *  7,077 Chapter 1 - Auto Layout 101.md
   * 25,536 Chapter 2 - Test Drive Auto Layout.md
   * 20,998 Chapter 3 - Auto Layout Fundamentals.md
   * **53,611 total**
	* Late start to writing due to sending out an email for my weekly email 
	* Played with iTerm2
	* Setup the iTerm2 to drop down from the top
	* Adding commands to my bash profile to give me word counts, so I can just type a command "words" to get stats on words changed, and total counts

			$ words
			    Words added: 890
			    Words removed: 0
			    Word diff: 890
			
			    7077 Chapter 1 - Auto Layout 101.md
			   25536 Chapter 2 - Test Drive Auto Layout.md
			   20998 Chapter 3 - Auto Layout Fundamentals.md
			   53611 total


	* Now I can see what kind of work changes I've done from the last commit
	* Editing is slower, so being stuck in editing due ot the Pin Tool exercise has been blocking progress … I'm going to skip rest for now, and keep moving to the rest of the outline
	* Updated to use iTerm2 from Terminal, playing with settings to better configure for my usage

## October 29 2018 10:54:18

Got stuck editing and changing text … wordcount isn't accurate since I removed text.

* Day 42: Monday
	* Wrote 179 words
	* Edited words in a complex area for adding constraints in Pin Tool
	* Didn't do as much writing because I've been stuck in this "editing" section and I need to be writing.
	* `wc -w C*.md` = wordcount for all "Chapter <numbers titles>.md"

   52,411 total

* Tomorrow: Go over how to update the layout from the simple method to use the baseline alignment after the majority of the constriants were set
* Go over how you can elverage stack views for the same layout

## October 28 2018 08:22:11

* Day 41: Sunday
	* ~750 words (lots of edits around the bottom sections)
		* Hard to trakc, need to track total WC before/after starting, otherwise it's not linear right now.
	* 3254 to bottom
	* Question: "`Right-click` + drag" technique … how do I format Right-click and drag? Is this the official name? docs talk about Control Click … but I feel that's not what the beginner is going to be using. Right-click is more descriptive, and there are multiple ways to click… 
	* Question: which tweet did I write after WWDC 2018? About Xcode 10, apparently it's hanging on the wall at Apple in the Swift hallway.
	* Is it "Storyboard" or "storyboard" or storyboard? or .storyboard?
	* 

## October 27 2018 09:23:19

* Day 40: Saturday
	* 776 words (1st pomodoro)
	* Started at 9:10am today
	* XCODE BUG: Constraint moves around the screen to top or bottom of the UI when trying to select it (edit second click misses)
	* "Align tool" for "Align Menu"
	* "constraint issue indicator" or "Auto Layout issue details pane"
	* Read the [Xcode Help Guide](https://help.apple.com/xcode/mac/10.0/#/devc8c2a6be1)


## October 26 2018 08:16:55

* Day 39: Friday
	* 1944 words
	* Researching compression reistance and hugging
	* Ways to define width
		* Equal width to another label
		* Leading and Trailing edges
		* Equal Leading edge
		* Equal trailing edge
	* Constraints are "associative?"
	* You don't need every combination, you just need to express a rule once, no reason to have duplicate rules that mean the same thing
	* Always try and simplify the rules ot the bare miniumu
		* Less errors
		* Easier to debug when issues arise
		* Less work, faster to design and layout
	* The bigger view becomes the Stuctural view
		* UITextField is taller than a default font UILabel
	* October 26 2018 15:32:23
		* Block UI
		* Resize to fit (makes constraints easier to add)

## October 25 2018 07:17:37

* Day 38: Thursday
	* 1107 words
	* Tons of research and a coulbe of Apple bugs in Xcode slowed progress ... trying to figure out best practice for baselines and alignment with the Pin Menu ... applying via exercises
	* Idea:
		* Write a script to search for all keywords and link to documentation
			* Can I search documentation based on keyword? easy link creation?
		* Write a script to make all instances of UILabel become `UILabel`
	* Question: Is it UILabels or UILabel's in the sentence: "8. Select the next two UILabels and UITextFields"?
		* and how would that work with linking to the documentation?
	* QUESTION: When should I use "UIButton" vs. button ... or label instead of "UILabel" or  image instead of UIImageView, or image view?
	* QUESTION: Should I use "Quotes" for Notes, or do I need some other kind of Markup for the book?
		* Mattt using a "liquid" %%info%% tag on NSHipster
	* Playing with size and height for a UITextField + UILabel alignment
		* QUESTION: Which alignment line should I use?
			* What's the difference?
		* TODO: Get the reader to think about bigger elements as "structural"
	* QUESTION: Why does the alignment in a UITextField seem wrong?
	* TIP: NEVER USE Reset to suggested constraints in practice, it's not multiple device aware, and adds constraints that do not work!

XCODE BUG: Reset to Recommended Constraints makes constraints that break on multiple devices, it's not adding "good" and "safe" constraints

XCODE BUG: UITextField text position clips and is offset from actual position on iPhone Simulator/Device

XCODE BUG: Baseline between TextField + Label, Top constraint set, and then Baseline set, Xcode states wrong thing "Missing Constraints: Need constraints for: Y Position"  .... but the solution is to remove the top constraint, because it conflicts with the baseline to the UITextField.

QUESTION: Shoudl I center align a Label and a TextField or should I baseline align?

October 25 2018 10:26:31

FAIL: Align tool to add constraints is causing duplicate constraints being added to the last in the row. ... had a duplicate view stacked on top of each toher ... that was confusing two "Last Name" labels



## October 24 2018 08:19:44

* Day 37: Wednesday
	* Starting after 8am, had a lot of stretches and a super tight knot this morning
	* 4,595 words (6th pomodoro) with exercises for keyboard shortcuts and selection
		* Tons of progress today after getting more sleep
		* I tried to move around more, and new positions so my back could relax without locking up as much
		* Tweaking and expanding upon my article for ways to add layout constraints ... got me going on additional navigation help in Storyboard
	* 3,034 words (4th pomodoro)
	* 971 words (1st pomodoro) on skipping rotation support
	* Questions
		* Should it be "Right-click" "right click" `right click` or `Right Click`?
		* Should I always use `UIButton` when I say button?
			* I should match this for all UIControls and UIViews
		* Pre-release the 7 ways to add constraints + clicking on the storyboard canvas
		* Should it be "Safe Area" or Safe Area or `Safe Area`
			* Where do I draw the line between code, proper name, and concept?
	* Apparently a leading constraint + center horizontally constraint is enough to make the UI fit edge to edge, but I still prefer having a leading and trailing constraint.

## October 23 2018 12:55:35

* Day 36: Tuesday
	* 1865 words (3 pomodoro's)
	* Added content on working with Stack Views (multiple methods)
	* Added post on content on colors + images from blog
	* Exploring examples with labels + content hugging/stretching
	* Wanted to write more, but back pain and constant long stretch breaks killed my energy after about 3
	* Found Keith's Auto Layout book launched 

## October 22 2018 15:25:38


* Day 35: Monday 
	* Started today looking at the chapter outline and trying to make some decisions on the amount of content.
	* I may need to extend release date, if I'm planning to market the book, I don't think I have enough time schedule to finish content, edit, and promote
	* Creating the outline took more time than I expected, and I'm still not happy with it, because it doesn't cover everything that I want, which is why this should be a series of books.
	* Currently I'm feeling pulled into too many directions with the contract work, meetings, visitors, and book
	* I need to simplify, and focus, make Monday's book day, and Tuesday's contract day, that way I can better focus

## October 21 2018 23:17:31

* Day 34: Sunday (Brick City Weekend)
	* 852 words (15 minutes)
	* Another long day, tons of activities ... late night writing.
	* Tomorrow I plan to get writing sooner, since this week I want to make sure that i"m making progress towards launching this book.
	* Writing earlier is very easy for getting things done, but I overslept because I didn't sleep well the night before due to back pain.
	
## October 20 2018 22:53:19


* DAY 33: Saturday (Brick City Weekend)
	* 787 words (10 min)
	* Family and friends visiting, lots of walking on campus, not really any time to write.

## October 19 2018 23:20:20


* Day 32: Friday
	* 1091 words (brain dump before bed)
	* Late night, Steph's birthday cooking workshop + friends in town for Brick CIty Weekend
	* Gabe cooked dinner for Steph

## October 18 2018 20:33:15


* Day 31: Thursday
	* 896 words (10 minutes)
		* Friends came in before I could finisher earlier tonight, so I wrote the last 500 words before getting in bed.
	* Spent all day working on contract work, friends coming in ... now
	* 400 words (10 minutes)
## October 17 2018 21:39:01

* Day 30: Wednesday
	* Total: 36,373 words
		* Chapter 1 - Auto Layout 101
			* 7,077 words
		* Chapter 2 - Test Drive Auto Layout
			* 25,536 words
		* Chapter 3 - Auto Layout Fundamentals
			* 3,760  words
	* 1069 words today (1 pomodoro)
		* Talked about demo + iterations (Creative Selection book by Ken Kocienda)
		* Wrote about styles of apps and content flows
		* Started to write about the 5 types of app layouts
	* 30 days in a Row of at least 750 words!
		* With the contract work and research on Swift, I haven't had as much time as I'd like to work on the book
		* I spent a lot more time working on the outline, but I havne't even written about half the things in the outline
		* Much of my time was spent on the beginning sections, which makes me wonder ... how should I proceed?
		* More writing?

## October 16 2018 21:48:34


* Day 29: Tuesday
	* 780 words (10-15 minutes)
	* Late start today ... been trying to finish contract work, taking time to research and implement with TDD + bluetooth

## October 15 2018 11:00:36

* Day 28: Monday
	* Stats Update
		* 3 chapters
			* 7,077 "Chapter 1 - Auto Layout 101.md"
			* 25,536 "Chapter 2 - Test Drive Auto Layout.md"
			* 1,952 "Chapter 3 - Auto Layout Fundamentals.md"
		* **34,565 words**
	* Command: 
		* `wc -w C*.md`
		* Word count of all the markdown files starting with "C"
	* 1773 words (1st pomodoro after extensive mind map + outline research)
		* One pomodoro writing and brain dump around size classes, designing for one device, layout for one device, and creative selection
		* Keep it simple explored
		* I spent a lot of time doing research this morning as I worked on fleshing out the updated Outline for Chapter 3, it feels like a lot of topics that I need to cram in one chapter, and I'm running out of days for this 30 day challenge. I really need to write, more, but I have a contract job to also work on
		* It's hard to work on more than 1 thing at a time! Especially when you write daily
	* Back is doing better, but not great, not flexible today, taking regular breaks with Super Easy Timer
	* Created the Chapter 3 mind map
	* May want to split book into more books?
	* Depending on how long this Chapter 2 or 3 becomes … we might want to restructure to make it easier to get started, but I feel that we still need to cover many of these topics (including debugging)
	* Responsive vs. adaptive vs. fluid vs. resizable
## October 14 2018 11:36:41

* Day 27: Sunday
	* 762 words (1st pomodoro in car)
	* 
	* Driving back from PA to Rochester
	* Hurt my back moving a bed, and I have hardly been able to move
	* Re-injured my back from when I hurt it snow shoveling heavy snow in March 2018 (hit curb with shovel)
	* Didn't sleep well, but trying to sit good in the car with some back support
## October 13 2018 07:31:29

* Day 26: Saturday
	* 507 words (1st pomodoro)
		* Spent a lot of time researching Auto Layout Demystified. 
			* I don't really like the examples, as they don't provide enough of a guide through the materials.
			* I'm trying to figure out if my book content is too long, or if it's a good length ~30,000+ words
		* Researching how to do percentage based layouts
			* 0.25 works, .25 doesn't when editing layout multipliers  .
		* BUG: Ratio of `.1` resets to 1

## October 12 2018 22:35:12

* Day 25: Friday
	* 867 words
		* I spent 15 minutes writing, late, time for bed.
		* I need to write first thing in the morning, it's really hard, but I slept in , and never got time to writing with all the family things going on here in PA.
	* Long day with family, visited my Grandma and made her smile and laugh (she has dementia)

## October 11 2018 10:40:11


* Day 24: Thursday
	* 1026 words (2nd Pomodoro)
		* Technical steps to make these adjustments on the Safe Areas
			* I always find this part a little hard to understand, and I feel like there's more to discuss, but I'm not sure exactly what that is
		* TODO: We can add some post-processing scripts to add insertion points like `[[2nd chapter]]` as replacement for %%Auto Layout 101 Chapter%%, or some kind of references (Does some piece of software exist?)
			* What is ObjC using?
			* What is NSHipster using?
			* Would this be Liquid?
	* 422 words (1st pomodoro)
		* Lots of research on the Safe Area view challenge
	* Driving home to PA (6 hours … in rain)
	* Writing while Steph drives … got to get my words in, I spent this morning working on TDD with mocking URLSession
	* 

## October 10 2018 07:27:06

* Day 23: Wednesday
	* 921 words (1st pomodoro)
	* I'm still not feeling like I've written enough for the book, there's so much to talk about, but maybe this book should be shorter and more approachable 
	* Should I split? I just need to keep writing … it might be more than 30 days of writing …

## October 9 2018 15:25:12

* Day 22: Tuesday
	* 1153 words (very technical instruction for adding constraints to labels)
	* Slow start today, got distracted writing email for audience, took away focus
		* Sent me down tangents for Jekyll blog hosting with Github like Mattt at <NSHipster.com>
	* If I have time, I'll try and write the remaining words tonight … need to get some progress … on being outside in sun, and then some Bluetooth / Unit tests!

## October 8 2018 08:01:00

* Day 21: Monday
	* 1760 words (2nd pomodoro)
		* Added more details, reworked some of the example by expelling it again
		* Tested out adding the constraints to make sure I'm giving the right advice.
	* 991 words (1st pomodoro) 
		* Went to bed at 11am, got up at 640am (more sleep!)
		* Feeling like I have more energy, I need to get to bed on time.
	* Progress Summary
		* Over the past 7 days (October 1st - October 7th) I wrote 8,852 words, which was under my target of 10,000 words.
		* I need to be writing 1400 - 1500 words per day to keep that target
		* Current total: 26,953  words
			* Chapter 1: 7,077 
			* Chapter 2: 19,876 
		* Chapter 2 may get split into parts, to make it more concise, there's a lot of teaching moments, but we also need a "speed coding" demo of adding constraints, instead of having this long drawn out instructions
		* 34 minutes to read 7000 words … 

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

