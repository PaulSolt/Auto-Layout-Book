# Auto Layout Book
Paul Solt
<Paul@SuperEasyApps.com>
9-18-2018

**Topic:** iPhone App UI Design with Auto Layout and Storyboards

Nonfiction > Computers > User Interfaces
Nonfiction > Computers > Programming > Mobile Devices


My rough draft outline for the [Auto Layout Book](http://bit.ly/AutoLayoutBook). Chapters and ideas are subject to change.

NOTE:  You can send me an [email](Paul@SuperEasyApps.com) if you want something included.

## Chapter 1: Auto Layout 101 

1. Why
	1. Design language for modern software UI
	1. Size + position
	2. Examples of iPhone Sizes (Screenshots of an app)
	3. Accessibility (larger fonts)
	4. Responsive designs
	5. Resizable windows / split views / slide overs / Air Play monitors
2. What
	5. Rules for positions/sizes
	6. Size + position
		1. Coordinate system demo (download app)
	 	2. Points vs. pixels
		3. Vector vs. pixels
			4. 1x, 2x, 3x
			5. PDF vectors
			6. Preserving vector data (scaling up for accessibility)
3. Paper Auto Layout
	10. #PaperAutoLayout Challenge
	11. Sketch Instagram Story Editor (2018) on paper
		12. Add rules for the distances (can you measure? xScope or best guess, or Photoshop inspect + count pixels / resolution)
		10. 3 Equal width buttons
		11. Instagram UI vs. Auto Layout constraints
4. Xcode Interface Builder (Quick Tour)
	6. Error Panels
		7. Issue Navigator
		8. Document Outline Error Panel
	10. Utilities Panel
	11. Canvas
	12. Console Output (Errors)
	13. Object Library (Xcode <=9 vs. Xcode 10+)
		14. Somewhat of a random change to the UI design
		15. Not well thought out, but it probably means we'll start seeing some other random (hopefully more coherent changes … a real window management system?)
		10. Option + Click button to "pin"
5. What is a constraint? 
	10. Constraints explained simply
	11. Constant
	12. Relation
13. Xcode is not a design tool
	14. Don't design in Xcode
	15. Implement designs
	16. Hire a designer

TODO: get the reader to describe on paper how Instagram UI should be displayed #AutoLayoutOnPaper

## Chapter 2: Test Drive Auto Layout

* Real World Example
* Design for one iPhone
* Add constraints to the Tip Calculator app
	* Centering Content in Container Views
	* Equal width contraints
	* Structural vs. accessory views
* Undo/redo/restart
* Breaking Constraints (unpredictable behavior)
	* Common Errors
	* Let's break it
* Colors of Auto Layout
	* Ambiguous
	* Conflicting
* Images
	* Content mode
	* Clipping
	* Stretching
* TODO: Challenge 1: Do it again from scratch
* MOVE: Challenge 1a: connect the UI
* DONE: Challenge 2: add iPhone X support (Safe Areas)
* TODO: Challenge 3: Reset to suggested constraints (does it work?)
* DONE: Add iPhone 8 Plus support (larger … button stretching)
* TODO: Add iPhone SE support (smaller buttons 44pt?)

## Chapter 3: Auto Layout Fundamentals



1. Layout for one device
	2. Keep it simple, get something working
	3. Design for iPhone 8 (or iPhone X)
	4. Add constraints 
	5. Iterate
		6. Tweak for other screen sizes (Repeat)
2. Types of layout
	7. Percentage-based layouts
	8. Fixed layouts
	9. Relative layouts
	10. "Responsive" -  might be a bad term to use
	11. **Resizable Layouts**
10. Building blocks
	11. Structure views
	12. Accessory views
	13. Regions
		14. Resizable Regions
		15. Fixed Regions
		16. 1 Resizable region per axis
		17. Multiple resizable regions requires a relationship (1:2 constraint)
13. Constraint 101
	14. Anatomy of a constraint
	13. Multiplier
	14. Priority 
	14. Multiple constraints 
	15. Internal constraints
		16. Intrinsic Content Size (Label is 251 content hugging)
		16. Content Hugging Priority
		17. Content Stretching Priority 
		18. Stack views
			19. Spacing constant set to … default canvas … makes alignment confusing …
15. Colors of Auto Layout
4. Size Classes + Rotation
	5. We won't be using in this beginner's book
	6. Many apps do not support rotation (Facebook or Instagram) 
	7. Unless it’s video content
	8. Simplify
	7. iPad vs. iPhone
	8. iPad Splitview
15. 7 Ways to add constraints
18. Intrinsic Content Size (other section?)
	19. Brief overview
19. Single screen vs. scrollable screen
	16. Different design considerations with layout
	17. Scrollable interface for super large fonts (edge case and more work)
20. Data driven UI vs. static content
21. Margins
22. Safe areas
23. Localization
24. Button sizes
	25. Apple’s iOS HIG
	26. Apple’s macOS HIG
27. Accessibility
	28. Dynamic Type
	29. Voice over
		30. UI testing
31. Preview
	32. Device > Simulator > Preview
	33. Test it
	34. Edge cases (sample data)
	35. UITests 
	36. Dark mode
15. Asset Catalog
	16. Adding images to Xcode
	16. Slicing
	17. Stretchable images
	18. Template images?
16. Hugging + Stretching Priorities 




## Chapter 4B: Storyboard Fundamentals (TODO: Did I do this?)

1. Selection
2. Editing
3. Navigation
4. Error panels

## Chapter 4: Layout

1. Layout
2. Design for One Device
3. Layout for One Device
4. Don't Design in Xcode
	5. Use Sketch for easier zoom in/out, number tweaking
	6. Layers are backwards order
	7. Layer control is harder
6. Adapt Designs to Xcode
	7. Why it's Different in Xcode
		8. San Fransisco Font
		9. Margins on Table View Cells change depending on device or orientation
		10. Gradients rendered different than design tools
7. Layout Building Blocks
	8. Structural views
	8. Centered Content Containers
		10. Single Element 
	9. Equal Width Buttons and Spacing
		10. Spacer Views
	12. Refactor Layouts for Usage
		13. Get an initial design
		14. Refactor the layout to support animations, experiences, or dynamic content
	16. Margins and Safe Areas
		17. Standard widths on iOS 12
			18. Equal Width Buttons
			19. Edges: 16 points
			19. Internal spacing: 8 points
			20. Sometimes: 0 points
	23. Layering Content
		24. UILabel on top of UIImage
		25. UITextField on top of UIImage
	27. Containing Complex UI
		28. Create .xib IBDesignable containers
			29. Simplify constraints by defining elsewhere
	32. Block UI into sections
		33. UIView Containers for percentage or fixed sizes
	35. Relative Layouts
		36. Leverage the position of one element to guide position of related
11. Iterative Design
	1. Version control + saving / backups
12. Layout Existing Designs
	13. Design files to Xcode Storyboard
		14. Sketch Measurements Plugin
		15. Working with designers
		16. Nudging views
	13. Tip Calculator (iPhone 8)
		14. Content Containers
		15. Equal width views
		16. Stylized UITextField
		17. Stylized UILabel
		18. Background Image Views
			19. Centering Content (Top View)
			20. Centering labels onto of background views
				20. Without arrow
				21. With Arrow
	20. Calculator (iPhone 8 Plus)
		21. Rough Layout Calculations
			22. Screen size / number of elements
			23. Space between
		22. Equal spaced buttons
		22. Equal width and height buttons
		23. Resizable Buttons
		24. Percentage based views
			25. Use math to calculate position on screen (height * .20)
	26. Instagram Story Editor (iPhone XS)
		27. Relative layout
		28. Camera / design tools overlay
30. Limitations of Storyboard files
	1. Custom Views + composition
	2. Simplifying constraints


## Chapter 5: Thinking with Auto Layout

1. Workflow (Review my 30 auto layout best practices) 
	1. Top to Bottom
	2. Structure/containers before accessory views
	3. Outside-in
	4. Pin Tool for Multiple Constraints
	5. Right-click and drag for Relationships
2. Practice Auto Layout Constraints 
	1. Tip Calculator
	2. Calculator
	3. Instagram Story Editor 

### 30-Day Auto Layout Challenge

1. 30 Days AutoLayout
	1. Different challenges will reference different sections in the book
	2. Re-read a section the night before, so that you can complete the challenge the next day
2. Pinterest Mood board
3. Find what you like, mimic it
4. Tools
	1. Sketch (and plugins measure, )
	2. Xcode 10
	3. Apple SF Fonts (restrictions on usage)
	4. iOS device
	5. USB cable
	6. Pen and paper (pencil)
	7. People (friends to try your apps)


## Chapter 6: Stack Views

10. Seeing Stack Views
	11. Centered Content
		12. One element
	13. Equally spaced (and centered)
		14. Two or more elements
	16. Embedded Stack Views (Inception)
	16. Equal widths and spacing
	17. Implicit auto layout constraints
18. Stack View Calculator Layout
	19. Redo the layout from [Layout chapter]
19. Stack View from App Screens
	20. [[IMAGE: Weather App + Stack Views for high level layout]]

## Chapter 7: Table Views and Scrollable Content

TODO: Reduce the scope to covering only the essentials of design, static and more custom prototype cells will be a topic for a future book.

1. Table View Introduction
2. Seeing Table Views
	3. Settings
	4. Maps Panel
	5. Facebook
6. Static Table Views (Storyboard only)
	7. Add layout constraints in Storyboard
	8. Quick and easy settings panels (Fast prototyping)
7. Dynamic Table Views
	8. Prototype Cells
	9. Xib Table View Cells
	10. Programmatic Table View Cells
11. Xcode 10 and TableView Storyboard Bugs
	12. Prefer Loading .xib
		13. Easier to change layout without touching main storyboard (better for teams)
		14. Less clicking to edit
		15. More predictable behavior
		16. Able to test resize/compression easily
		17. Test content resize with "fake data"
		18. Con: harder to see the "big picture", use a design file
20. Designing for Table Views
	21. Margins change sizes depending on device
	22. Pin to cell margins for proper iOS style
	23. Leverage automatic sizing for multiline labels and Dynamic Text
	24. Design interfaces that scale different fonts sizes
	25. Design in Sketch, implement in Xcode
26. Understanding Behavior
	27. The Rule of One
		28. One view can stretch in vertical or horizontal directions
		29. More than one, you'll need constraints establishing the relationship, otherwise it's ambiguous 
	31. Two vertical multiline labels
	32. Profile image with multiline labels
	33. Facebook post with an image
		34. Image settings
			35. Clipping
			36. Fixed width/height
	34. Different TableViewCells for different content
	35. One cell versus many cells
		36. Design for one interface
		37. One cell requires connecting constraints/stack views to change constraints or hide cells (Needs code)
		38. All need code, since you'll need new outlets for new content to layout properly
	40. Reserved names
		41. UITableView cell already defines names, you need to connect different names
	43. Hugging and Stretch for Automatic TableViewCells
		44. TableViewCells that use automatic height will relayout the UI to fit the content (if your constraints are correct)
		45. Different behavior for layout than you see in a standard UIViewController, which changes shape and has to stretch or compress
47. Xcode 10 Differences from Xcode 9
	48. Bugs: Images do not render when Storyboard first opened
	49. Changes: Font sizes or frames may be different for labels in Xcode 
19. Exercises
	20. Create a layout for a blog post
		21. Title
		22. Publish Date
		23. Author
		24. Body
26. Text Selection
	27. UILabel doesn't support selection
	28. Use UITextArea and disable edit if you want to enable selection
	29. Users may like to copy text, and the UILabel makes it impossible
	30. Disable scroll and it'll self size itself like a UILabel (documentation on scroll)



## Chapter 8 Troubleshooting Auto Layout

1. When things don’t work like you expect
	1. Start over from scratch
	2. Create a test Xcode project
	3. Reset your constraints and try again
	4. Block the design
	4. Clear the slate
		5. Clear constraints and fix your layout
	5. Set identifiers for UI elements (so you can read error messages)
	6. Use WTFAutoLayout.com 
	7. Review the fundamentals of constraints, priorities, and content hugging/compression resistance
	8. Use "Super Easy Auto Layout" (See chapter XX)
	9. Draw or Sketch designs outside of Xcode
2. Fixing 9 common beginner mistakes
	1. Text Clipping Issues
	2. Fixed height constraints on a font 
	3. Fixed width with a single line label
	4. Not using a Content View for UIScrollViews (See video)
	5. Conflicting constraints (rules that don't work together)
	6. Direct conflict
	7. Indirect conflict
	8. Ambiguous constraints (not enough rules)
	9. Multiple solutions
	10. Exercise the ambiguity
		1. LLDB
		2. Function call (hook up a button to test)
	11. Too many constraints (Over-constrained)
	12. Reduce to the minimum you require
	13. Layout rules are not multi-device safe (conflict on a different size class)
	14. Vertical and horizontal dimensions are not specified for a table view cell (default height + clipping)
	15. Content Hugging Errors (See the Rule of One Resizable View)
	16. Content Compression Errors (See the Rule of One Resizable View)
	17. Fixed Frame Layouts
	18. Can work for small widgets, but not full width/height view controllers
	19. Using Recommended Constraints (NEVER)
	20. Switching Size Classes (or rotating) before adding all the constraints (All or nothing)
6. Level up your development
	1. Daily Log (Markdown)
	2. Practice (Code Katas)
	3. Start the 30-Day Auto Layout Challenge
7. Auto Layout table view cells
8. Get Audited 
	1. Auto Layout Audit
	2. Accessibility Audit
	3. Usability Audit
9. Diagnose Auto Layout Problems (Expert System to direct to further resources)
	1. Take the quiz to figure out your problem

-----


FUTURE
17. Placeholder constraints??? When?

* Make UI static screen, "but enable scroll if Dynamic Text increases"(flag?)
* Decide what max text size you want to support
* Increasing button size (inset vs. larger frame)
	* Techniques and strategies
	* 
* Accessibility: Make the Images Resizable Vectors
	* In the Asset Catalog if you're using vector images, you can make the button graphics scale based on the system font size.
	* Test It with Accessibility Inspector



	21. Not using the Undo/Redo Keys
3. Improve your workflow
	1. Not using Inequalities for edge cases
	2. Not changing content hugging or compression resistance priorities
	3. Having a fallback scenario
	4. Not testing large fonts (Accessibility Inspector)
	5. Not testing long text strings (User generated content)
	6. Not testing different aspect ratio images
	7. Not testing large and small images
	8. Not using a representative data set to exercise all of your constraints
	9. Not logging errors to console/log file (SwiftyBeaver)
	10. Not backing up your work with Github
	11. Not communicating about UI changes with your team (Project + Storyboard merge conflicts)
		12. Xcode changes every open (Throw away changes you don't need)
		13. Github + Git
		14. Register for details about my Github for iOS Developers Course
4. Common Beginner iOS UI Errors + Crashes
	1. Some errors are unrelated to Auto Layout, but reside in the UI + code connection
	2. Missing function (unrecognized selector)
		1. Command + Shift + F for the "Selector name", add the missing function
	3. Not registering a Table View Cell with a table view
	4. Not setting the Table View Cell reusable identifier
	5. Unable to connect IBOutlets + IBActions: Not subclassing from the correct class type UITableViewCell, UICollectionViewCell or UIView
	6. Breakpoint "crash" - You added a break point
	7. Optional crash from deleted property connection - Reconnect the UI element to the code
	8. Wrong UI object connected to code
	9. Proper way to remove an outlet/connection (Delete from the button) 
	10. Fix your spelling mistakes correctly (Crash on launch)
5. Bad advice: When to ignore Xcode errors and warnings
