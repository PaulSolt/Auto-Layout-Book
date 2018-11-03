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




## Chapter 4B: Storyboard Fundamentals

1. Selection
2. Editing
3. Navigation
4. Error panels

## Chapter 4: Layout

1. Layout the Tip Calculator App
2. Layout the Instagram Story Camera
3. Layout Calculator
4. Workflow
	5. Layout for one iPhone
	5. Constraint for one iPhone
	6. Tweet for every iPhone
	7. Version control + saving / backups
5. Limitations of Storyboard files
6. Custom Views + composition
	7. Simplifying constraints

## Chapter 5: Thinking with Auto Layout

1. Table View Introduction
2. Dynamic content requries it, and almost every app uses table views
3. App's decomposed


## 30-Day Auto Layout Challenge

1. 30DaysAutoLayout
2. Pinterest Mood board
3. Find what you like, mimic it

## Troubleshooting Auto Layout

1. When things don’t work like you expect
2. Fixing 9 common beginner mistakes  
3. Bad advice: When to ignore Xcode errors and warnings
4. Daily Log (Markdown)
5. Auto Layout table view cells



FUTURE
17. Placeholder constraints??? When?
