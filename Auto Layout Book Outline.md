# Auto Layout Book
Paul Solt
<Paul@SuperEasyApps.com>
9-18-2018

**Topic:** iPhone App UI Design with Auto Layout and Storyboards

My rough draft outline for the [Auto Layout Book](http://bit.ly/AutoLayoutBook). Chapters and ideas are subject to change.

NOTE:  You can send me an [email](Paul@SuperEasyApps.com) if you want something included.

## Chapter 1: Auto Layout 101 

1. Why
	1. Design language for modern software UI
	1. Size + position
	2. Examples of iPhone Sizes (Screenshots of an app)
	3. Accessibility (larger fonts)
	4. Responsive designs
	5. Resizable windows / split views / Air Play monitors
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

TODO: get the reader to describe on paper how Instagram UI should be displayed #AutoLayoutOnPaper

## Chapter 2: Test Drive Auto Layout

1. Real World Example
2. Design for one iPhone
3. Add constraints to the Tip Calculator app
	10. Centering Content in Container Views
	11. Equal width contraints
	12. Structural vs. accessory views
4. Undo/redo/restart
3. Breaking Constraints (unpredictable behavior)
	4. Common Errors
	5. Let's break it
4. Colors of Auto Layout
	5. Ambiguous
	6. Conflicting
4. Images
	14. Content mode
	15. Clipping
	16. Stretching
18. TODO: Challenge 1: Do it again from scratch
19. MOVE: Challenge 1a: connect the UI
19. DONE: Challenge 2: add iPhone X support (Safe Areas)
20. TODO: Challenge 3: Reset to suggested constraints (does it work?)
4. DONE: Add iPhone 8 Plus support (larger … button stretching)
5. TODO: Add iPhone SE support (smaller buttons 44pt?)

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
	2. Top to Bottom
	3. Structure/containers before accessory views
	3. Outside-in
	4. Pin Tool for Multiple Constraints
	5. Right-click and drag for Relationships
3. Practice Auto Layout Constraints
	4. Tip Calculator
	5. Calculator
	6. Instagram Story Editor


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

## Chapter 7Pms: Table Views and Scrollable Content

1. Table View Introduction
2. Dynamic content requires it, and almost every app uses table views
3. App's decomposed
4. Table Views
	5. UILabel multiline (behaviors)
		6. Gestures to add copy/paste options
	6. UITextView multiline (behaviors)
		7. Selection
		8. Disable scroll to create intrinsic content size, otherwise you need to give it a default size
	10. Scrollview input area that resizes until max size, then scrolls (Instagram post input window)
		11. Define a default size, or allow it to grow naturally, like the Messages app

## 30-Day Auto Layout Challenge

1. 30DaysAutoLayout
	2. Different challenges will reference different sections in the book
	3. Re-read a section the night before, so that you can complete the challenge the next day
2. Pinterest Mood board
3. Find what you like, mimic it
4. Tools
	5. Sketch (and plugins measure, )
	6. Xcode 10
	7. Apple SF Fonts (restrictions on usage)
	7. iOS device
	8. USB cable
	9. Pen and paper (pencil)
	10. People (friends to try your apps)

## Troubleshooting Auto Layout

1. When things don’t work like you expect
2. Fixing 9 common beginner mistakes 
3. Bad advice: When to ignore Xcode errors and warnings
4. Daily Log (Markdown)
5. Auto Layout table view cells
6. Diagnose Auto Layout Problems (Expert System to direct to further resources)
7. iOS App Tune Up (Offer for assistance)
	8. Fix the most glaring problems



FUTURE
17. Placeholder constraints??? When?

* Make UI static screen, but enable scroll if Dynamic Text increases (flag?)
* Decide what max text size you want to support
* Increasing button size (inset vs. larger frame)
	* Techniques and strategies
	* 
* Accessibility: Make the Images Resizable Vectors
	* In the Asset Catalog if you're using vector images, you can make the button graphics scale based on the system font size.
	* Test It with Accessibility Inspector